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
- **When captions are missing or unusable:** first verify whether subtitle/caption text is actually accessible; a visible YouTube Transcript control that yields no text is not a transcript. For creator-owned videos, prefer original local media/audio if available. Otherwise, when the creator has asked you to analyze/transcribe the public video, retrieve/process only that video and run an appropriate open-source ASR model locally (for example, Faster-Whisper); do not upload it to a hosted transcriber.
- Select an ASR model suited to the spoken language/accent. Reuse a channel-approved model when available. For this channel, the creator accepted a partial output from `collabora/faster-whisper-small-hindi` running CPU int8; earlier generic Faster-Whisper `base`/`small` outputs on the same sample were poor. Treat this as a channel-specific proven starting point, not a universal default.
- If no accepted transcript reference exists, transcribe a 30–60 second representative sample first. Preserve the original wording/script (Hindi/Hinglish, including code-switching), show it for accuracy review when exact voice matters, and correct only with the creator’s review or clearly marked cleanup. Do not automatically run full-video transcripts for every upload during setup.
- State model, spoken-language setting, sample/full coverage, timestamps, and review status. Keep raw or lightly normalized output in its own transcript-reference file in the creator’s spoken language/style; keep analysis and metadata in English.
- Do not paraphrase or silently repair uncertain words while labeling a transcript verbatim. Put corrections/normalization in a separate layer or clearly mark them.
- Ask the creator to review an initial sample when accuracy or voice fidelity is important; update the memory from accepted/corrected examples, not from unreviewed ASR alone.
