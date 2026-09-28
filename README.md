# YouTube Channel Manager

A reusable Codex/agent skill for setting up and managing a YouTube channel: channel research, creator onboarding, persistent memory, content strategy, scripts, packaging, product ideas, marketing, and video-generation briefs.

## Install

With the [Vercel Skills CLI](https://github.com/vercel-labs/skills):

```bash
npx skills add ITZSHOAIB/youtube-channel-manager
```

To install globally for Codex and choose the skill explicitly:

```bash
npx skills add ITZSHOAIB/youtube-channel-manager --skill youtube-channel-manager --agent codex --global
```

When no complete `CHANNEL_MEMORY.md` exists, the skill asks only for the channel URL; latest-three and top-three video links are optional. It researches the public channel itself, presents an evidence-labeled profile draft for approval, and creates memory/transcript-reference files only after approval.

## Language policy

Internal channel memory and research notes are in English. Channel-facing creative output follows the creator's requested language; transcript references preserve the creator's spoken style.

## Contents

- `SKILL.md` — entrypoint and workflow
- `references/setup-intake.md` — first-run/refresh questionnaire
- `references/channel-memory-template.md` — persistent memory schema
- `references/deliverables.md` — research, scripts, packaging, products, and video-generation guidance
- `agents/openai.yaml` — Codex skill interface metadata
