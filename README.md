# YouTube Creator Skills

**Practical, channel-aware workflows for the work behind a YouTube video.** Research the channel and product, learn the creator's real experience, then shape ideas, scripts, packaging, and production around the channel's approved memory.

This repository contains focused Agent Skills you can install individually or together. The skills are designed to work with Codex and other agents supported by the [Vercel Skills CLI](https://github.com/vercel-labs/skills).

## Skills in this repository

| Skill | What it helps with |
|---|---|
| [`youtube-channel-manager`](skills/youtube-channel-manager/SKILL.md) | Channel setup and memory, channel research, content ideas, product concepts, scripts, titles, thumbnails, marketing, and channel-aware video-generation briefs. |
| [`gadget-review-interviewer`](skills/gadget-review-interviewer/SKILL.md) | Product research followed by an adaptive, one-question-at-a-time interview about the creator's hands-on experience, leading to a grounded review brief or script. |

### YouTube Channel Manager

Start with a channel URL. The skill finds recent uploads, studies public channel evidence, and drafts a profile for the creator to review. A creator can optionally provide up to three “gold standard” videos. The skill saves persistent channel memory only after approval.

With approved memory in place, it can help with:

- Video, Short, and series ideas grounded in viewer needs and channel fit.
- Product research and review scripts that distinguish sourced facts from creator experience.
- Titles, thumbnails, descriptions, comparisons, and marketing copy.
- Channel-specific HyperFrames briefs and production plans.
- Local transcript generation when YouTube captions are unavailable, with model, coverage, and review status recorded separately from channel memory.

### Gadget Review Interviewer

This skill researches product specifications and public claims itself. It then asks the creator one question per turn about what they actually experienced: time owned, real use, comfort, performance, connectivity, battery, issues, price paid, ratings, and verdict. It adapts its questions to the product and answers already given; it does not hand the creator a long questionnaire or ask them to repeat specifications available online.

## Memory-first, evidence-led

When `CHANNEL_MEMORY.md` is available, it guides the workflow: research priorities, intended audience, question phrasing, tone, language, script style, disclosures, and production constraints. Relevant transcript and style references inform voice without being copied mechanically.

If no memory exists, the channel manager researches public evidence and presents a proposed profile for approval before saving setup files. Public observations, inferences, and unknown private details are labeled separately. Internal manager memory and research notes are kept in English; channel-facing content follows the creator's approved language and style.

For review work, the creator is the source for firsthand observations. Manufacturer claims, independent testing, public anecdotes, and creator experience stay clearly distinguished. Untested features and uncertain details are labeled instead of guessed.

## Install

Install both skills globally for Codex:

```bash
npx skills add ITZSHOAIB/youtube-creator-skills --skill youtube-channel-manager --skill gadget-review-interviewer --agent codex --global
```

Install just one skill:

```bash
npx skills add ITZSHOAIB/youtube-creator-skills --skill youtube-channel-manager --agent codex --global
npx skills add ITZSHOAIB/youtube-creator-skills --skill gadget-review-interviewer --agent codex --global
```

To install for another agent, replace `codex` with its supported agent name. To install into the current project instead of globally, omit `--global`. See the [Skills CLI documentation](https://github.com/vercel-labs/skills) for supported agents and options.

## Try it

After installing, start a conversation with a task such as:

- “Set up a channel manager for this YouTube channel: `https://youtube.com/@yourhandle`.”
- “Help me research and script a review of this controller. Interview me about my experience one question at a time.”
- “Use my channel memory to pitch three video ideas for this month's uploads.”

For a hands-on review, the agent researches the product before asking about firsthand use. For channel setup, the agent researches the channel and asks for approval before creating durable memory or transcript-reference files.

## Repository layout

```text
skills/
├── youtube-channel-manager/
│   ├── SKILL.md
│   ├── references/
│   └── scripts/
└── gadget-review-interviewer/
    └── SKILL.md
```

Each skill has its own `SKILL.md` and can be installed independently. The channel manager includes supporting references and a local ASR helper for transcript fallback.
