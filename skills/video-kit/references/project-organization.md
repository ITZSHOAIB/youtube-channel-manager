# Video project organization

Use the active channel workspace as the root: the folder containing its `CHANNEL_MEMORY.md` (or the clearly identified video project root if no memory file exists). Keep all durable channel memory at that root and each video's working files inside one project folder.

## New project path

For new projects, use:

```text
<channel-workspace>/videos/<year>/<month>/<video-title>/
```

Use the local year and two-digit month when the project folder is first created, not the planned publish date. This keeps a growing archive grouped by year and month while preserving a title-named folder for every video. Use the creator's planned/recommended video title for the final folder name; replace filesystem-forbidden characters with readable separators. Keep the full human-readable video title as the H1 inside `script.md`.

Before creating a folder, search for an existing project matching the video title, product/topic, or supplied `review-brief.md`. Reuse a matching older `videos/<video-title>/` folder in place. Do not move or rename existing project folders just to fit the dated convention. If two distinct videos have the same title, add a short distinguishing date or topic suffix to the later folder.

## Files in a project

```text
<video-title>/
├── review-brief.md       # Review Grill; only for hands-on reviews
├── script.md             # Video Kit outline, hybrid, or full script
├── publishing.md         # Video Kit upload copy and publishing notes
├── research.md           # Optional; only for substantial research that outgrows source notes
├── assets/               # Optional; create only when media/assets are saved
└── production/           # Optional; production plans or editable video project
```

- Review Grill saves or updates `review-brief.md` in the same folder Video Kit uses. If an existing brief is elsewhere in the channel workspace, use it and move/copy it only when the creator requests consolidation.
- Video Kit saves `script.md` and `publishing.md` beside the review brief. Keep source URLs and checked dates with the relevant claims; create `research.md` only if the notes are substantial.
- Put generated or collected media in `assets/` and create it only when needed. Keep HyperFrames planning and editable source under `production/` (for example, `production/video-plan.md` and `production/hyperframes/`). Do not create empty placeholder directories.
- Avoid duplicating the same script, review brief, or upload package under a separate global `scripts/` tree. A video folder is the source of truth for that video's materials.
- For a brainstorming-only response, do not create a project folder. Create one once the creator requests saved research, a review brief, a script/outline, a publishing package, or production files.
