# Channel deliverable playbook

Read only the section relevant to the current request. The creator’s memory controls language, tone, format, and sponsor constraints.

## Ideas and strategy

- Start from the viewer’s task, channel fit, current demand/search intent, creator strengths, and production constraints.
- Separate timely opportunities from evergreen formats. For current market topics, verify date, geography, official product/version, and current competition.
- For each idea, state the audience problem, core promise, evidence/demo needed, format, and why it fits. Rank ideas by fit, evidence, production effort, and likely viewer value; label hypotheses.

## Research

- Browse when facts can change or when the creator asks for research. Prefer manufacturer/platform documentation, original datasets, direct channel evidence, and reputable reporting.
- Record source links and checked dates. Separate company claims, independent tests, creator experience, and inference.
- For comparisons or purchasing advice, verify exact models/variants, local prices/availability, and meaningful alternatives close to scripting/publishing time.
- For platform/how-to content, verify the current interface and official help documentation; version changes can invalidate steps.

## Scripts

- Build around a strong viewer question, a clear promise, demonstrations/evidence, trade-offs, and a useful next step/verdict.
- Preserve the creator’s approved spoken rhythm, word choice, and code-switching from transcript references. Do not invent catchphrases or overfit to a single clip.
- Keep spoken lines natural and easy to say. Avoid padding, unsupported certainty, spec-dump sequences, and generic engagement requests.
- Distinguish “manufacturer claims,” observed test results, and personal opinion. Give conditional recommendations: who benefits, who should skip, and why.
- Provide production cues only when useful: b-roll, screen recording, product close-ups, on-screen proof, pause points, and edit notes.

## Titles, thumbnails, captions, and descriptions

- Pair searchable subject terms with a clear benefit, decision, or honest curiosity hook.
- Make thumbnail and title promise the same thing the video proves. Avoid fabricated urgency, misleading product images, or unsupported superlatives.
- Check readability at mobile size; use the saved visual identity and authentic brand assets where available.
- Localize in the channel’s saved language and script. Preserve official product/model spellings and search terms where useful.
- Descriptions should prioritize useful details, tested variants/prices with dates, sources, chapters/links, and required affiliate/sponsor disclosures.

## Product and business concepts

- Present new products/offers as hypotheses until audience evidence or a small validation test supports them.
- Prefer a small validation loop: audience problem, existing alternatives, willingness-to-pay signal, prototype/landing test or poll, success threshold, and next decision.
- Keep sponsored/affiliate incentives explicit and editorial judgement independent.

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

Favor one well-supported treatment over a long menu of concepts. If the request is exploratory or a major creative choice is still ambiguous, show the plan for feedback before coding. If the request is already clear, use sensible defaults from channel memory and keep moving; do not turn video production into another questionnaire. If a material claim lacks proof or an asset/license is unclear, flag that specific blocker.

#### Intro and channel identity principles

- Open on the viewer’s subject, question, or most compelling visual. Add branding where it strengthens recognition without holding up the promised content.
- Design the ident from the channel’s actual logo, colors, typography, host/voice relationship, and energy. A creator’s format and taste outrank a trendy motion preset.
- Keep recurring intros consistent enough to be recognized, but let topic-specific openings vary. Do not reuse the same animation as a substitute for the hook.
- For a channel trailer, show what viewers will actually get; avoid vague “welcome to my channel” copy.
- Narration is optional. Use the creator’s own supplied recording or an explicitly approved voice method; never clone a real voice without permission. For this channel, all video copy/narration should follow saved Hinglish preferences.

#### HyperFrames handoff and review

The Channel Manager owns the story, channel fit, language, source selection, claims, and creative boundaries. HyperFrames owns the implementation details: composition structure, time-based HTML, supported animation/runtime conventions, technical checks, and render commands. Put the creative contract in `composition-brief.md`; specify the must-show/must-not-change points but do not prescribe low-level selectors or runtime internals.

Honor the channel memory’s technology constraints. When it specifies open-source-only HyperFrames (as the 4TECHLoverz memory currently does), use local open-source tooling/dependencies, local rendering, and creator-provided or clearly licensed assets. Do not invoke hosted rendering, hosted HyperFrames MCP, HeyGen generation services, or metered media providers for that channel. If the applicable constraints cannot be met, state the limitation before substituting another service.

Build in a dedicated project folder and preserve editable source. Follow current official HyperFrames skills/CLI, then preview, run the current structural/runtime/layout checks, inspect key frames, and review the rendered file for readable copy, correct Hinglish text, timing, audio, and final-frame/poster quality. Render final delivery only after preview approval unless the user clearly authorized a final render in the request. Report exactly which checks and exports succeeded; never claim an MP4 exists if only a brief or source project was created.

Create only useful artifacts for the job. Depending on scope, those may be `video-plan.md`, `composition-brief.md`, the editable HyperFrames project, rendered video, a selected poster/thumbnail, and Hinglish share copy. Do not create all artifacts for a brief-only or concept-only request.

Workflow inspiration: the staged inspect → plan/storyboard → HyperFrames handoff → validate/render structure in [`latent-spaces/brag`](https://github.com/latent-spaces/brag). Adapt the process, not its startup-only premise, fixed runtime, humor-first angle, tone presets, assets, or audio defaults.

### Building with HyperFrames through a coding agent

HyperFrames is an HTML-to-video framework: the agent authors an editable composition with HTML/CSS/JavaScript and supported seekable animation patterns, then the CLI previews, checks, and renders it. Keep the YouTube Channel Manager responsible for the channel strategy, Hinglish script/copy, brand memory, and creator-facing production brief. When asked to build the actual video, use the official HyperFrames plugin/skills and their current authoring contract rather than inventing framework syntax from memory.

Honor explicit creator technology constraints recorded in channel memory or given in the current request. If the creator requires open-source HyperFrames tooling only, treat that as a hard constraint: use the open-source HyperFrames project/CLI with local rendering and open-source local dependencies; do not use hosted HyperFrames MCP, cloud rendering, HeyGen-hosted generation, paid/metered image, video, voice, or music providers, or closed-source media services. Prefer Chromium over proprietary Chrome where the workflow permits. The Codex plugin package may itself be open source, but do not assume every provider or network-backed capability it exposes meets the creator's constraint.

- Official setup for coding agents: `npx hyperframes skills update` installs/updates the core skills. The official repository also includes a Codex plugin; if the creator prefers Codex’s plugin UI, check the current official install guide and use the plugin’s bundled launcher/skills. Do not install both a plugin and duplicate standalone skills without a reason.
- The current CLI prerequisites are Node.js 22+ and FFmpeg. Verify the current machine with `npx hyperframes doctor`; requirements and commands can change, so check current official docs if this guidance is stale.
- Typical local flow: `npx hyperframes init <project>`, open the project folder in the coding agent, build with `/hyperframes`, preview with `npx hyperframes preview`, run `npx hyperframes lint` and `npx hyperframes check`, then render after the creator approves the preview. Use the official workflow’s equivalents if it has changed.
- Keep the project editable and source assets inside its project folder. Preserve exact product/model details and channel assets. Put spoken and on-screen copy in the creator’s saved language/script (for this channel, Hinglish); keep technical project notes in English.
- Use creator-provided assets, assets created with open-source local tools, or media with a compatible open license. Verify the license for each asset; the framework's open-source license does not grant rights to third-party images, fonts, music, or footage. If an open-source-only workflow cannot meet a requirement, explain the gap and ask before proposing a non-open-source alternative.
- If HyperFrames is unavailable in the current agent or rendering environment, provide a ready-to-use brief and state the specific missing prerequisite instead of claiming an MP4 was generated.

Official references: [HyperFrames quickstart](https://github.com/heygen-com/hyperframes/blob/main/docs/quickstart.mdx), [HyperFrames repository and agent setup](https://github.com/heygen-com/hyperframes), [CLI requirements and workflow](https://github.com/heygen-com/hyperframes/blob/main/packages/cli/README.md).

## Transcript references

- Prefer creator-provided subtitle files or verified platform captions.
- **When captions are missing or unusable:** first verify whether subtitle/caption text is actually accessible; a visible YouTube Transcript control that yields no text is not a transcript. For creator-owned videos, prefer original local media/audio if available. Otherwise, when the creator has asked you to analyze/transcribe the public video, retrieve/process only that video and run an open-source ASR model locally; do not upload it to a hosted transcriber. Do not stop at “ASR tool unavailable” before checking available runtimes and attempting local setup.
- Select an ASR model suited to the spoken language/accent. Reuse a channel-approved model when available. For this channel, the creator accepted a partial output from `collabora/faster-whisper-small-hindi` running CPU int8; earlier generic Faster-Whisper `base`/`small` outputs on the same sample were poor. Treat this as a channel-specific proven starting point, not a universal default.
- If no accepted transcript reference exists, transcribe a 30–60 second representative sample first. Preserve the original wording/script (Hindi/Hinglish, including code-switching), show it for accuracy review when exact voice matters, and correct only with the creator’s review or clearly marked cleanup. Do not automatically run full-video transcripts for every upload during setup.
- **Runnable workflow:** use the skill's `scripts/transcribe_youtube.py` helper. It downloads only the requested video's audio to a temporary directory using `yt-dlp`, applies the requested time clip with Faster-Whisper, writes a separate Markdown reference with URL/model/coverage/review status, then removes the temporary audio. The default model is the creator-accepted Hindi fine-tune, `collabora/faster-whisper-small-hindi`; default language/device/compute settings are Hindi, CPU, and int8. Pass a local media path as the positional source instead of a URL to use creator-provided audio/video.
- Check for an existing usable Python 3.9+ runtime first, including a bundled workspace runtime exposed by the current agent. If a dependency-discovery tool such as `mcp__codex_app__load_workspace_dependencies` is available, call it; add the returned Node directory to PATH for yt-dlp when needed. If packages are absent, bootstrap them rather than reporting the tool unavailable. On Windows, run the skill's `scripts/setup_local_asr.ps1 -Source <video-url> -Output <temporary-review-path>` helper from the project root; it creates `.youtube-channel-manager/asr-venv` inside the project, installs the open-source dependencies there, and generates the sample. Pass `-PythonExe <bundled-python-path>` or `-NodeExe <bundled-node-path>` when those runtimes are not on PATH. During setup, use an OS temporary path for `-Output`, show the returned text with the proposed profile, then remove the temporary transcript if setup is declined. On macOS/Linux, create a project-local venv with the available `python3 -m venv .youtube-channel-manager/asr-venv`, install `faster-whisper` and `yt-dlp[default]`, then invoke the Python helper through that venv, also writing setup samples to a temporary path. Faster-Whisper uses bundled PyAV decoding and does not require a system FFmpeg binary. For YouTube retrieval, yt-dlp may require a supported JavaScript runtime for current YouTube challenges; reuse an installed Node.js/Deno runtime or install an open-source runtime locally if needed. The model weights download on first run and are cached by Hugging Face; keep those weights in the normal user cache, not in channel memory. Do not install system-wide when a project-local environment works.
- During setup, attempt dependency provisioning and one sample automatically when captions fail; don't require the creator to install a transcriber manually. If the machine has no Python/runtime, package/model download is blocked, or YouTube retrieval fails, report the concrete command/error and a direct alternative such as asking for the creator's audio or subtitle file. Do not claim a transcript was generated when only setup instructions were prepared.
- State model, spoken-language setting, sample/full coverage, timestamps, and review status. Keep raw or lightly normalized output in its own transcript-reference file in the creator’s spoken language/style; keep analysis and metadata in English.
- Do not paraphrase or silently repair uncertain words while labeling a transcript verbatim. Put corrections/normalization in a separate layer or clearly mark them.
- Ask the creator to review an initial sample when accuracy or voice fidelity is important; update the memory from accepted/corrected examples, not from unreviewed ASR alone.
