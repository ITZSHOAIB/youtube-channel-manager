---
name: youtube-channel-manager
description: Set up and manage a YouTube channel’s strategy, research, scripts, packaging, product ideas, marketing, and video-generation briefs using creator-approved memory.
---

# YouTube Channel Manager

Use this skill for channel audits, setup, content strategy, topic research, video/Shorts ideas, scripts, packaging, product or business concepts, marketing, and video-generation or Hyperframes briefs.

## Operating workflow

1. **Load the channel context.** Look in the current project/workspace for `CHANNEL_MEMORY.md` and transcript-reference files. Read the relevant files before recommending or writing. Treat memory as a starting point, distinguish observed facts from creator-confirmed preferences and inference, and refresh stale details.
2. **Run low-friction setup when needed.** If there is no channel memory, it is clearly incomplete, or the creator requests a reset, read [the setup intake](references/setup-intake.md). Ask only for the channel URL/handle if it is not already available. Find the latest three videos yourself from the channel. The creator may optionally name or link up to three “gold standard” videos that represent the desired direction. Research first, draft the channel profile from evidence, and ask the creator to approve or request changes before creating any memory or transcript-reference files. Never make the creator fill out the full profile questionnaire. Never create durable setup files before approval; a temporary ASR sample may be generated for review and must be removed if not approved. If no URL is available, ask for it directly; do not infer a channel from a folder name. The required URL request must be visible to the user, not buried in internal/tool/expanded history.
3. **Keep language preferences separate.** Reuse explicit language preferences from the conversation or existing memory. Otherwise infer the channel language/script/register from current videos, use the user's current conversation language for replies, label those as provisional in the proposed profile, and invite corrections in the single approval step. Do not ask a separate language questionnaire during initial setup.
4. **Save durable context.** Only after the creator approves the proposed profile, create or update `CHANNEL_MEMORY.md` in the project/workspace in English. Keep useful source-language transcript references in separate files; do not paste transcript blocks into manager-memory prose. Create additional Markdown files only when they hold useful, sourced material for future work. Read [the memory template](references/channel-memory-template.md) when creating or substantially rebuilding the profile.
5. **Complete the requested deliverable.** Read [the deliverable playbook](references/deliverables.md) when the task involves scripts, research, packaging, product ideas, marketing, or video-generation briefs/builds.
6. **Close the loop.** State what was created or learned, identify important assumptions and confidence limits, and ask for creator review only where it will materially improve the channel profile or transcript/style reference.

## Evidence and freshness

- For changing facts such as prices, availability, launches, product specifications, platform features, and market claims, verify current primary or authoritative sources before scripting.
- Use direct channel pages, actual videos, descriptions, playlists, posts, comments, and creator-supplied analytics as different evidence types; say which conclusions are direct observations and which are hypotheses.
- Treat public engagement, title views, and sampled comments as clues, not representative analytics. Do not invent audience demographics or private performance data.
- Prefer creator-provided captions or subtitle exports for transcripts. If YouTube captions/transcript text are missing or unusable, follow the runnable local ASR fallback in [the deliverable playbook](references/deliverables.md), including provisioning open-source dependencies when absent. Do not stop at a missing preinstalled tool. Start with a short representative sample when no accepted reference exists, and never send video/audio to a third-party transcription service without permission. Identify model and coverage, preserve useful output in a separate transcript file after setup approval, and label confidence. Do not present unreviewed machine output as verified verbatim text; record creator review/corrections and sample limits.
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
