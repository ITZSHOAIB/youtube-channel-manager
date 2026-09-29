# Video production and HyperFrames

Read when planning or building video assets. Follow channel memory for creator-specific style, tools, language, and licensing constraints.

## Video-generation and Hyperframes briefs

- Specify the video’s purpose, duration, aspect ratio/platform, pacing, shots, transitions, sound/music direction, and on-screen text language/script.
- Identify the exact product/version/era and any reference assets required for logo, host, or product fidelity.
- Clearly distinguish genuine product footage/screen capture from illustrative or generated shots. Never imply generated visuals are captured evidence or a real test.
- Include a shot-by-shot sequence with timestamps only when it helps production; otherwise use a concise scene brief.

### Channel-aware video production

For an actual video build, use a staged workflow inspired by strong project-to-video skills: inspect source material, choose a specific creative angle, storyboard, hand off a production brief to HyperFrames, then validate and render. Adapt every stage to the channel’s creator-approved memory, audience, visual identity, language, and supplied “gold standard” references. This workflow applies across channel genres and video types; it is not a startup-launch template.

#### Choose the right video job

Identify what the requested asset needs to do before choosing a style:

- Channel trailer or channel introduction: communicate the channel promise, target viewer, and reason to subscribe.
- Recurring episode intro/ident: establish recognition quickly without delaying the episode’s actual hook.
- Outro or CTA: reinforce the next useful action while preserving the creator’s natural subscriber relationship.
- Segment bumper or transition: distinguish recurring sections without disrupting pacing.
- Short-form hook/teaser: earn attention immediately and make one clear promise.
- Product review, tutorial, comparison, explainer, or story video: show the real subject, viewer problem, proof, and conclusion.
- Other channel-specific format: derive the structure from the actual script, examples, and creator goal.

Do not impose one duration, aspect ratio, joke, transition style, or story arc on every format. A recurring bumper should not become a long generic intro; a review should not be forced into a promo. Fit runtime and layout to its publishing slot and purpose.

#### Inspect before planning

Read the approved `CHANNEL_MEMORY.md` and any relevant transcript/style references. Inspect the actual source for this video (script, product/version, screenshots, footage, data, or reference URL) and the channel’s approved visual assets. If no memory exists, use the setup workflow first. If creator-selected gold-standard videos are available, treat them as taste references; compare them with recent uploads and do not assume popularity equals desired style.

Capture only evidence needed to make a specific video: the promise, strongest hook, 1–3 moments worth showing, essential claims/proof, visual palette/type/logo treatment, on-screen language, and CTA. Do not expose private customer data, account details, unreleased information, keys, or credentials from inspected material.

#### Make a channel-specific creative plan

Before writing composition code, draft a compact `video-plan.md` or a storyboard in chat with:

- Objective and publishing placement (for example, recurring long-form bumper, channel trailer, or vertical Short).
- Intended viewer and one central promise or feeling.
- Creative angle and opening hook, specific to the channel/topic.
- Format, aspect ratio, target duration, and safe-area assumptions.
- Beat-by-beat scenes: what is shown, what copy is read, and the evidence/assets required.
- Channel-fit tone and taste interpretation, grounded in approved references—not a generic preset or genre stereotype.
- On-screen and spoken copy in the channel’s saved publishing language/script; technical direction can remain in English.
- Audio role and licensed/local asset plan, CTA, and explicit exclusions (claims, visuals, pacing, music, humor, or sponsor treatment).

When a track recommendation is part of the request, read [music-and-licensing.md](music-and-licensing.md) and follow the channel's saved attribution preferences.

Favor one well-supported treatment over a long menu of concepts. If the request is exploratory or a major creative choice is still ambiguous, show the plan for feedback before coding. If the request is already clear, use sensible defaults from channel memory and keep moving; do not turn video production into another questionnaire. If a material claim lacks proof or an asset/license is unclear, flag that specific blocker.

#### Intro and channel identity principles

- Open on the viewer’s subject, question, or most compelling visual. Add branding where it strengthens recognition without holding up the promised content.
- Design the ident from the channel’s actual logo, colors, typography, host/voice relationship, and energy. A creator’s format and taste outrank a trendy motion preset.
- Keep recurring intros consistent enough to be recognized, but let topic-specific openings vary. Do not reuse the same animation as a substitute for the hook.
- For a channel trailer, show what viewers will actually get; avoid vague “welcome to my channel” copy.
- Narration is optional. Use the creator’s own supplied recording or an explicitly approved voice method; never clone a real voice without permission. Follow channel memory for all video copy and narration.

#### HyperFrames handoff and review

Video Kit owns the story, channel fit, language, source selection, claims, and creative boundaries. HyperFrames owns the implementation details: composition structure, time-based HTML, supported animation/runtime conventions, technical checks, and render commands. Put the creative contract in `composition-brief.md`; specify the must-show/must-not-change points but do not prescribe low-level selectors or runtime internals.

Honor the channel memory’s technology constraints. If it requires open-source-only tooling, use local open-source dependencies, local rendering, and creator-provided or clearly licensed assets. Do not substitute hosted or metered services. If the constraints cannot be met, state the limitation before proposing another service.

Build in a dedicated project folder and preserve editable source. Follow current official HyperFrames skills/CLI, then preview, run current structural/runtime/layout checks, inspect key frames, and review the render for readable copy, correct language/script, timing, audio, and final-frame/poster quality. Render final delivery only after preview approval unless the user clearly authorized a final render in the request. Report exactly which checks and exports succeeded; never claim an MP4 exists if only a brief or source project was created.

Create only useful artifacts for the job. Depending on scope, those may be `video-plan.md`, `composition-brief.md`, the editable HyperFrames project, rendered video, a selected poster/thumbnail, and channel-language share copy. Do not create all artifacts for a brief-only or concept-only request.

Workflow inspiration: the staged inspect → plan/storyboard → HyperFrames handoff → validate/render structure in [`latent-spaces/brag`](https://github.com/latent-spaces/brag). Adapt the process, not its startup-only premise, fixed runtime, humor-first angle, tone presets, assets, or audio defaults.

### Building with HyperFrames through a coding agent

HyperFrames is an HTML-to-video framework: the agent authors an editable composition with HTML/CSS/JavaScript and supported seekable animation patterns, then the CLI previews, checks, and renders it. Use channel memory for strategy, scripts/copy, and brand context; Video Kit owns the creative brief. When asked to build the actual video, use the official HyperFrames plugin/skills and their current authoring contract rather than inventing framework syntax from memory.

Honor explicit creator technology constraints recorded in channel memory or given in the current request. If the creator requires open-source HyperFrames tooling only, treat that as a hard constraint: use the open-source HyperFrames project/CLI with local rendering and open-source local dependencies; do not use hosted HyperFrames MCP, cloud rendering, HeyGen-hosted generation, paid/metered image, video, voice, or music providers, or closed-source media services. Prefer Chromium over proprietary Chrome where the workflow permits. The Codex plugin package may itself be open source, but do not assume every provider or network-backed capability it exposes meets the creator's constraint.

- Official setup for coding agents: `npx hyperframes skills update` installs/updates the core skills. The official repository also includes a Codex plugin; if the creator prefers Codex’s plugin UI, check the current official install guide and use the plugin’s bundled launcher/skills. Do not install both a plugin and duplicate standalone skills without a reason.
- The current CLI prerequisites are Node.js 22+ and FFmpeg. Verify the current machine with `npx hyperframes doctor`; requirements and commands can change, so check current official docs if this guidance is stale.
- Typical local flow: `npx hyperframes init <project>`, open the project folder in the coding agent, build with `/hyperframes`, preview with `npx hyperframes preview`, run `npx hyperframes lint` and `npx hyperframes check`, then render after the creator approves the preview. Use the official workflow’s equivalents if it has changed.
- Keep the project editable and source assets inside this video's `production/` folder. Preserve exact product/model details and channel assets. Put spoken and on-screen copy in the creator’s saved language/script; keep technical project notes in English.
- Use creator-provided assets, assets created with open-source local tools, or media with a compatible open license. Verify the license for each asset; the framework's open-source license does not grant rights to third-party images, fonts, music, or footage. If an open-source-only workflow cannot meet a requirement, explain the gap and ask before proposing a non-open-source alternative.
- If HyperFrames is unavailable in the current agent or rendering environment, provide a ready-to-use brief and state the specific missing prerequisite instead of claiming an MP4 was generated.

Official references: [HyperFrames quickstart](https://github.com/heygen-com/hyperframes/blob/main/docs/quickstart.mdx), [HyperFrames repository and agent setup](https://github.com/heygen-com/hyperframes), [CLI requirements and workflow](https://github.com/heygen-com/hyperframes/blob/main/packages/cli/README.md).
