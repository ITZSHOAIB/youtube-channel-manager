# Low-friction channel setup

Use this workflow when a channel has no complete `CHANNEL_MEMORY.md` or the creator asks to rebuild it. The goal is to do the research for the creator, present a sourced draft for approval, and only then write persistent files.

## 1. Ask for the minimum input

- If the channel URL/handle is already present in the current conversation or workspace, do not ask for it again. Start research.
- If it is missing, ask for the **YouTube channel URL or @handle**. This is the only required setup input.
- Optionally invite the creator to share links for their **latest three videos** and **top three videos** if they have particular examples in mind. Make clear these are optional; otherwise identify recent uploads and publicly popular videos yourself.
- Do not ask the previous long list of setup questions. Do not ask for analytics, audience demographics, language, goals, workflow, or sponsor rules as a prerequisite.

Example first message when no URL is known:

> Send me the YouTube channel URL or @handle. If you want, also share links to the latest three videos and/or top three videos you want me to study; those links are optional. I’ll research the channel, draft its profile with evidence and confidence labels, and show it to you for approval before saving any files.

## 2. Research and draft the profile independently

Use the public channel URL to research as much as is reasonably accessible:

- Channel name, description, links, playlists, visible branding, and current activity.
- The latest three uploads, including Shorts where clearly part of the active channel mix.
- Up to three publicly most-viewed/popular videos, identifying the selection as public-view based rather than private YouTube Studio performance. If this list is unavailable, state how examples were selected.
- Titles, thumbnails, descriptions, format, hooks, CTAs, and recurring content topics.
- Available transcripts/captions for a small representative sample (prefer recent videos and/or one popular example) to understand language, delivery, tone, and how the creator addresses subscribers. Preserve Hinglish/Hindi source wording when making transcript references. Label ASR output, coverage, and confidence.
- Public comments/posts when available, as anecdotal evidence only.

Build a proposed profile covering the memory template’s useful sections: channel positioning, content pillars and formats, audience hypothesis, language and voice, subscriber relationship, packaging, goals, production constraints, commercial rules, guardrails, and open questions. Do not invent private facts. For goals, demographics, analytics, production constraints, or sponsor rules that cannot be established publicly, propose a conservative inference only when evidence supports one; otherwise mark them “unknown—not publicly verifiable.”

In the draft, distinguish:

- **Observed:** directly visible in the public channel/videos.
- **Inferred:** a plausible interpretation of public evidence, with confidence (high/medium/low).
- **Unknown:** requires creator/private analytics input and is not safely inferable.
- **Creator-confirmed:** explicitly supplied or approved by the creator.

Treat public view counts as popularity clues only. Never describe them as the channel’s actual top-performing videos according to Studio unless the creator supplies analytics.

## 3. Ask for one confirmation, not a second questionnaire

Present a concise but useful **Proposed channel profile** in the user-visible reply. Summarize the evidence and list the drafted answers for the profile categories, marking inferences and unknowns. Include representative source video links and research date. Do not hide the profile or approval request in tool output or expanded history.

End with one clear choice:

> Do you approve this profile so I can save `CHANNEL_MEMORY.md` and the useful transcript references, or what would you like changed?

Do not turn every unknown into a question. The creator can approve with unknowns retained, approve with corrections, or request revisions. If they request changes, revise the proposed profile and seek approval again. **Do not create or overwrite setup memory/transcript files before explicit approval.**

## 4. Save only after approval

After approval:

- Create/update `CHANNEL_MEMORY.md` in English using `references/channel-memory-template.md`.
- Create separate transcript-reference Markdown files only for representative transcripts that materially preserve voice or are useful for future work. Keep the transcript in its original Hindi/Hinglish wording and label source, URL, coverage, transcript method, confidence, and whether the creator reviewed it.
- Add a research/evidence Markdown file only if source notes are too extensive to keep usefully in the memory’s evidence section. Avoid empty folders and unnecessary files.
- Mark public inferences and unknown private details clearly. Record approval date and any corrections as creator-confirmed.
- Report the created files and note any important items left unknown. Do not ask the creator to repeat facts already provided.
