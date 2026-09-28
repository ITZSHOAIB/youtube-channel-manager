---
name: youtube-channel-manager
description: Set up and manage a YouTube channel’s strategy, research, scripts, packaging, product ideas, marketing, and video-generation briefs using creator-approved memory.
---

# YouTube Channel Manager

Use this skill for channel audits, setup, content strategy, topic research, video/Shorts ideas, scripts, packaging, product or business concepts, marketing, and video-generation or Hyperframes briefs.

## Operating workflow

1. **Load the channel context.** Look in the current project/workspace for `CHANNEL_MEMORY.md` and transcript-reference files. Read the relevant files before recommending or writing. Treat memory as a starting point, distinguish observed facts from creator-confirmed preferences and inference, and refresh stale details.
2. **Run setup when needed.** If there is no channel memory, it is clearly incomplete, or the creator requests a reset, read [the setup intake](references/setup-intake.md). Research public channel information when a channel URL is available, then ask the required creator questions. The questions must appear in the actual user-visible response; mentioning that an intake is ready, or putting questions only in internal/tool/expanded history, does not count as asking them. In that same response, include a visibly scannable numbered Markdown list with each question on its own line (group related prompts beneath it) and a simple answer template. Never compress all setup questions into one paragraph or end with a vague “setup is ready” handoff. Prefill verified facts and ask the creator to confirm or correct them; do not make them repeat facts they have already provided. Do not call setup complete until required items are answered or explicitly marked unknown.
3. **Keep language preferences separate.** Ask what language to use in conversation and what language/script/register to use for channel-facing work. Save them as separate settings. Follow an existing explicit preference without asking again.
4. **Save durable context.** Create or update `CHANNEL_MEMORY.md` in the project/workspace in English. Keep source-language transcripts in separate transcript-reference files; do not paste transcript blocks into the manager-memory prose. Read [the memory template](references/channel-memory-template.md) when creating or substantially rebuilding the profile.
5. **Complete the requested deliverable.** Read [the deliverable playbook](references/deliverables.md) when the task involves scripts, research, packaging, product ideas, marketing, or video-generation briefs.
6. **Close the loop.** State what was created or learned, identify important assumptions and confidence limits, and ask for creator review only where it will materially improve the channel profile or transcript/style reference.

## Evidence and freshness

- For changing facts such as prices, availability, launches, product specifications, platform features, and market claims, verify current primary or authoritative sources before scripting.
- Use direct channel pages, actual videos, descriptions, playlists, posts, comments, and creator-supplied analytics as different evidence types; say which conclusions are direct observations and which are hypotheses.
- Treat public engagement, title views, and sampled comments as clues, not representative analytics. Do not invent audience demographics or private performance data.
- Prefer creator-provided captions or subtitle exports for transcripts. If captions are unavailable and ASR is used, identify the model and coverage, preserve the output in a separate transcript file, and label confidence. Do not present an unreviewed machine output as a verified verbatim transcript. When the creator reviews a sample, record their acceptance or corrections and keep the sample’s coverage limits explicit.
- Do not upload unpublished or private media to a third-party transcription service without the creator's permission. A public video URL and a request to transcribe that video authorize research on that public item, not unrelated content.

## Memory and voice

- Keep all manager memory, research notes, and setup records in English, unless the creator explicitly requests another internal-memory language.
- Write channel-facing creative work in the creator’s specified language, script, and register. If missing, ask during setup; do not assume the communication language is the same as the channel language.
- Store transcript excerpts in the creator’s spoken language/code-switching style as the reference artifact. Preserve the source wording and script where possible; label any transliteration, cleanup, or uncertain ASR segments.
- Avoid turning one past video, one ASR failure, or one old preference into a universal rule. Confirm current channel direction when history and present goals may differ.

## References

- First-time or refreshed setup: [setup-intake.md](references/setup-intake.md)
- Creating/updating persistent channel memory: [channel-memory-template.md](references/channel-memory-template.md)
- Writing or researching channel deliverables: [deliverables.md](references/deliverables.md)
