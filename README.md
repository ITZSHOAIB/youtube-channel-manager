# YouTube Creator Skills

**Practical, channel-aware workflows for the work behind a YouTube video.** Research the channel and product, learn the creator's real experience, then shape ideas, scripts, packaging, and production around the channel's approved memory.

This repository contains focused Agent Skills you can install individually or together. The skills are designed to work with Codex and other agents supported by the [Vercel Skills CLI](https://github.com/vercel-labs/skills).

## Skills in this repository

| Skill | What it helps with |
|---|---|
| [`youtube-manager`](skills/youtube-manager/SKILL.md) | Channel setup and memory, channel research, content ideas, product concepts, scripts, publishing, and video-production briefs. |
| [`review-grill`](skills/review-grill/SKILL.md) | Product and digital-service research followed by an adaptive, one-question-at-a-time interview that saves the creator's firsthand experience in a structured review brief. |

### YouTube Manager

Start with a channel URL. The skill finds recent uploads, studies public channel evidence, and drafts a profile for the creator to review. A creator can optionally provide up to three “gold standard” videos. The skill saves persistent channel memory only after approval.

With approved memory in place, it can help with:

- Video, Short, and series ideas grounded in viewer needs and channel fit.
- Product research and review scripts that distinguish sourced facts from creator experience.
- Research-backed, copy-ready YouTube publishing packages with titles, descriptions, tags, and rights-aware music options.
- Titles, thumbnails, descriptions, comparisons, and marketing copy.
- Script production cues, including script-matched music direction and rights-aware track suggestions.
- Channel-specific HyperFrames briefs and production plans.
- Local transcript generation when YouTube captions are unavailable, with model, coverage, and review status recorded separately from channel memory.

### Review Grill

This skill fits hands-on reviews of consumer products and digital services, from controllers and phones to apps and subscriptions. It researches specifications, current claims, pricing, and terms itself, then asks the creator one question per turn about firsthand use and what they would tell a buyer. It saves a structured `review-brief.md` with the creator's experience, key unknowns, and useful research sources kept distinct. It does not write scripts or publishing assets.

For a complete review video, use YouTube Manager to turn the brief into the requested recording outline or script and copy-ready publishing package. Review Grill can also be used by itself when the creator only wants to capture their product experience for later.

## Memory-first, evidence-led

When `CHANNEL_MEMORY.md` is available, it guides the workflow: research priorities, intended audience, question phrasing, tone, language, script style, disclosures, and production constraints. Relevant transcript and style references inform voice without being copied mechanically.

Channel memory is maintained as the creator confirms durable preferences and decisions over time. Skills update confirmed guidance in place, keep one-video details with that video's project files, and ask before turning an inference into a permanent creator preference.

If no memory exists, the channel manager researches public evidence and presents a proposed profile for approval before saving setup files. Public observations, inferences, and unknown private details are labeled separately. Internal manager memory and research notes are kept in English; channel-facing content follows the creator's approved language and style.

For review work, the creator is the source for firsthand observations. Manufacturer claims, independent testing, public anecdotes, and creator experience stay clearly distinguished. Untested features and uncertain details are labeled instead of guessed.

## Install

Install both skills globally for Codex:

```bash
npx skills add ITZSHOAIB/youtube-creator-skills --skill youtube-manager --skill review-grill --agent codex --global
```

Install just one skill:

```bash
npx skills add ITZSHOAIB/youtube-creator-skills --skill youtube-manager --agent codex --global
npx skills add ITZSHOAIB/youtube-creator-skills --skill review-grill --agent codex --global
```

To install for another agent, replace `codex` with its supported agent name. To install into the current project instead of globally, omit `--global`. See the [Skills CLI documentation](https://github.com/vercel-labs/skills) for supported agents and options.

## Try it

After installing, start a conversation with a task such as:

- “Set up a channel manager for this YouTube channel: `https://youtube.com/@yourhandle`.”
- “Interview me about my experience with this controller and save a review brief. Then help me turn it into a YouTube review video.”
- “Use my channel memory to pitch three video ideas for this month's uploads.”

For a hands-on review, Review Grill researches the product and saves an experience brief after interviewing the creator. YouTube Manager uses that brief for scripts and publishing assets. For channel setup, the agent researches the channel and asks for approval before creating durable memory or transcript-reference files.

## Repository layout

```text
skills/
├── youtube-manager/
│   ├── SKILL.md
│   ├── references/
│   └── scripts/
└── review-grill/
    ├── SKILL.md
    └── references/
        └── experience-probes.md
```

Each skill has its own `SKILL.md` and can be installed independently. The channel manager includes supporting references and a local ASR helper for transcript fallback.
