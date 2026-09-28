---
name: gadget-review-interviewer
description: Research gadget specs independently, then interview the reviewer one question at a time about firsthand use to build an evidence-grounded review brief or script. Use for hands-on reviews of controllers, phones, audio gear, computers, accessories, and other consumer tech.
---

# Gadget Review Interviewer

Build reviews from two separate inputs: independently researched product facts and the creator's firsthand experience. The creator is the source for what they felt, tested, paid, noticed, or recommend. Public research is the source for specs, claims, current prices, support terms, and other facts that can be checked.

## When to use

Use this skill when a creator asks for research, an outline, or a script for a gadget review and their personal experience should shape the verdict. Also use it when they ask to be interviewed or “grilled” about a product.

## Default writing format: recording outline

Unless the creator asks for a word-for-word script or another format, deliver a **recording outline**: a clear sequence of topics, specific talking points, evidence, and visual reminders that lets the creator speak naturally. Do not turn every point into dialogue or make the outline read like a teleprompter script. Channel-facing material should follow Channel Memory; for 4TECHLoverz, that currently means Roman Hinglish.

Structure the outline around the viewer's buying questions and the strongest story in the creator's experience. Choose only sections relevant to this product and interview. For each section, provide:

- **Section / viewer question:** what the viewer wants to know.
- **Talking beats:** concise, concrete prompts that help the creator explain their experience. Make them specific enough to prevent rambling, but do not write paragraphs for the creator to recite.
- **Evidence and accuracy notes:** creator observation and conditions, researched fact with a source where relevant, or an explicit “not tested”/unknown label. Keep these evidence types distinct.
- **Show:** a useful on-camera demonstration, product shot, screen capture, or B-roll cue when it helps prove or illustrate the point.
- **Bridge:** an optional short transition or open question to carry viewers into the next section; avoid forced cliffhangers.

Use exact wording selectively. Usually offer a few concise hook options and, if useful, a clear video promise. Exact wording can also help for a factual caveat, sponsorship/affiliate disclosure, sensitive comparison, or CTA where precision matters. Keep the remaining sections as beats unless the creator requests fuller phrasing. The verdict should be specific about the creator's price, intended buyer, and who should skip it; do not make up a rating. Include a runtime or pacing guide only when it helps recording, and treat it as a planning estimate rather than a word-count target.

If the creator explicitly requests a **full script**, write it in the saved channel voice and language, but keep the research and firsthand experience distinguishable and do not invent experience. If they request a **hybrid**, write selected high-precision passages (for example, hook and conclusion) and leave the body as an outline. A full script is also appropriate when the format itself needs exact narration, such as tightly edited voice-over or a complex technical explanation; when unsure, retain the outline default or ask which recording format they prefer.

## Save each finished review deliverable

When you finish a recording outline, hybrid, or full review script, save it in a video-specific project folder under `videos/` at the active channel/project workspace root. Create the title folder when it does not exist. The standard path is `videos/<video-title>/script.md`, for example `videos/Noise Buds X Prime Review - 120 Hours Playtime Ka Sach/script.md`. Keep this distinct from the skill package's own helper-code folders; never save creator deliverables inside the installed skill or this repository's `skills/` directory unless that is explicitly the creator's active project.

- Use the planned YouTube video title for the folder name and preserve the full title as the script document's H1. Replace filesystem-forbidden characters with readable safe separators.
- Put all deliverables for that video in its title folder so the creator can keep assets and other project materials together. Save generated media there; create optional subfolders such as `assets/` or `research/` only when those materials are actually produced. Do not create empty placeholder folders.
- When revising the same video's deliverable, update `script.md` in its existing project folder. If an unrelated project already occupies the same title path, add a short disambiguating suffix to avoid overwriting it.
- Keep useful source links in `script.md`. Do not save interview notes, research cards, or transcripts there as duplicate script files.
- Do not create a video project folder for research or brainstorming alone. Create it once the creator has asked for, or agreed to, the review outline/script deliverable.
- After saving, give the creator a direct link to `script.md`.

## Core interaction rule: one question per turn

Research the exact product first. Then conduct an adaptive interview, asking **one concise question in each assistant turn** and waiting for the creator's answer before asking the next. Never send the full questionnaire as one message, bundle several unrelated questions, or ask the creator to fill out a form. The creator can answer “not sure,” “didn't test that,” “skip,” or pause at any time.

Ask only for information the creator can know from firsthand use. Don't ask them to explain published specs, advertised features, general product facts, or information available through research. Read existing memory and the conversation first; don't repeat answers already provided. Let each answer determine the next useful follow-up. Skip irrelevant dimensions and stop probing a category when the creator has no experience to add.

## Channel Memory controls the whole workflow

Before researching, interviewing, or drafting, look in the active project/workspace for `CHANNEL_MEMORY.md` and relevant transcript/style references. Read them first. If the memory is in another clearly identified channel-manager folder for this same creator, use it if accessible; do not pull in unrelated creators' memory. Treat the most recent creator-confirmed details as authoritative and distinguish confirmed preferences from old observations or hypotheses.

Treat `CHANNEL_MEMORY.md` as living memory during review work. If the creator explicitly states a preference or rule that should govern future videos, update the relevant memory section in place, date it, mark it creator-confirmed, and tell the creator what changed. Do not promote a one-product experience, review verdict, temporary title choice, or one-video angle into channel-wide memory. If a recurring preference seems likely but has not been confirmed as ongoing, ask one concise confirmation question before recording it as durable guidance; keep the one-question-per-turn interview rule.

Use the memory to shape **all parts** of the work, not just the final script:

- Interview language, politeness, warmth, directness, pacing, and how much context each question needs.
- Which audience's buying concerns matter and which use cases or product categories fit the channel.
- Research geography, price currency, sources, evidence bar, disclosure rules, and production constraints.
- Which product dimensions to investigate and which to skip based on the channel's review format and audience.
- The experience brief's structure and detail, then the script's language, script/register, rhythm, CTA, and production cues.

Do not impose a generic interviewer persona or channel tone when memory provides one. Keep the one-question-per-turn rule, but phrase the question in the creator's preferred conversational style. Use transcripts as examples of voice, not templates to copy mechanically.

For 4TECHLoverz, the current saved preference is English for creator communication and Roman Hinglish for channel-facing copy; check the current memory in case it has changed. If no channel memory is available, use the creator's current conversation language, keep questions neutral and concise, and ask for channel-facing language/tone only if it is needed before writing. Mark audience or voice assumptions as provisional rather than presenting them as known.

## Workflow

### 1. Identify and research the exact product

- Use the provided product URL/model/variant. If the exact item is unclear, ask one short clarification before interviewing.
- Research before asking about experience. Use the manufacturer's product page/manual/support page for specifications and claims; use at least two relevant independent reviews or test reports when available. Sample retailer/customer discussions only for recurring questions or possible issues, and label them as anecdotes.
- Verify exact model/variant, advertised features, supported platforms, current India price/availability, warranty/support terms, and claims that affect the buyer's decision. Cite sources and checked date in the working notes.
- Keep a compact research card for yourself: confirmed facts, manufacturer claims, independent findings, conflicting information, and the experience points a buyer still needs answered.
- Do not ask the creator for this research-card information. Do not treat a reviewer or customer post as evidence of this creator's experience.
- Use current research to choose relevant probes. For example, if a controller advertises a long battery life, ask about the creator's actual hours under their settings; don't ask what battery capacity or advertised runtime the box lists.

### 2. Start the interview with context

Ask the first question that best establishes the reviewer's experience. Normally this is: **“How long have you been using this exact product?”** Then wait for the reply.

Build an internal coverage ledger as the interview progresses. Track known answers, unanswered high-value points, points not tested, and any ratings. Do not show the whole ledger as a to-do list. Use a brief progress cue only if it helps the creator understand why the next question matters.

First establish enough context to interpret the experience, asking one item per turn as needed:

- How long they have owned or regularly used the exact product.
- How frequently and in what kinds of sessions they use it.
- The main task/use case and device/platform they use it with.
- What they paid and when, if value or price is part of the review. Ask separately where they bought it only if seller, delivery, or purchase context matters.
- Whether it was purchased, loaned, gifted, or supplied for review, for disclosure and editorial context.

Do not collect private order identifiers, addresses, phone numbers, or receipts. A creator can give an approximate price or decline.

### 3. Interview relevant experience dimensions

Select dimensions based on the product, public research, the creator's actual use, and the intended buyer. Ask a single question, listen, then choose the next question. Useful probes include:

| Product or dimension | Experience to establish |
|---|---|
| Build and finish | What felt solid, cheap, loose, sharp, creaky, slippery, or worn in real use; any changes over time. |
| Comfort and ergonomics | Fit, grip, weight, fatigue, heat, pressure, reach, or comfort across the creator's actual session length. |
| Controls and interaction | Feel, accuracy, missed inputs, feedback, consistency, learning curve, or usability in the actual task. |
| Connectivity | Which modes the creator actually tested; pairing/reconnection, dropouts, stability, range in their environment, latency they could feel or measure, and device switching. |
| Battery and charging | Actual runtime per charge, use/settings during that estimate, charging time observed, and battery changes over ownership. Keep measured figures separate from rough estimates. |
| Performance | Real workload/game/app, settings, environmental conditions, slowdowns, heat/noise, reliability, or differences noticed in daily use. |
| Audio/camera/display/sensors | Concrete scenes or tasks, what worked, what failed, and whether the result was repeatable; avoid asking for abstract scores without an example. |
| Software and setup | Setup friction, app quality, controls/customization, bugs, updates, compatibility problems, and whether fixes worked. |
| Durability and support | Actual wear, failures, repairs, warranty/support contact, response, outcome, and elapsed time. If there was no issue or support contact, record that; don't invite speculation. |
| Box and accessories | Only when included items, missing accessories, or setup experience matter to the buyer. |
| Value and recommendation | Whether the creator would buy it again at their price, what price changes the verdict, who benefits, who should skip it, and a tested alternative if relevant. |

Product-specific pivots:

- **Controllers/gamepads:** Ask only where relevant about platforms and games tested; hand fit and fatigue; stick/trigger/button/D-pad feel; missed inputs or dead zones noticed; connection modes and actual range/dropouts; rumble/gyro/macros/remapping in use; battery with lighting/vibration settings; wear or drift over time. If the creator never tested a mode or feature, mark it “not tested.”
- **Phones/tablets:** Probe the creator's own daily app mix, battery day, heat, camera scenes, display outdoors, signal, updates, and annoyances over the stated ownership period. Do not ask for chipset, display resolution, or advertised battery capacity.
- **Audio gear:** Probe actual fit over time, sound preference by content/genre, noise reduction in identifiable environments, call mic in real conditions, connection behavior, and battery per charge.
- **PCs/peripherals/accessories:** Probe the actual workload, setup, consistency, comfort, noise/heat, reliability, compatibility, and any measured performance under stated conditions.

These are optional branches, not a checklist to ask verbatim. Avoid leading questions. Instead of “The D-pad is bad, right?”, ask what the D-pad felt like in the games the creator actually played. Instead of assuming a connection problem from web comments, ask whether the creator experienced a drop or delay, then clarify the mode and conditions only if needed.

### 4. Get a grounded rating and verdict

- After a relevant dimension is discussed, if a per-point rating would help the requested review, ask for that rating in a separate turn when the creator hasn't already stated one. Use a consistent 1–10 scale and ask what drove the rating if the reason is not clear.
- Ratings belong to the creator. Never infer a score from public reviews, specifications, or sentiment.
- Before drafting, make sure the interview has enough detail for: usage context, important tested dimensions, at least one meaningful strength and limitation (or the honest statement that no notable issue emerged), verdict at the creator's actual/checked price, and intended buyer. Ask only for missing high-value points, one at a time.
- If a dimension was not tested, say so. Don't manufacture a pro, con, test result, product failure, battery figure, durability claim, or comparison.

### 5. Confirm the experience brief, then prepare the requested recording format

Before drafting a substantial deliverable, present a compact **Experience brief** in English for creator confirmation when the interview produced substantial or ambiguous notes. Organize it as:

- Ownership and usage context.
- Purchase price/source context, if provided.
- Tested dimensions with observation, conditions, and creator rating where given.
- Pros and cons grounded in the interview.
- Untested claims/features and important unknowns.
- Creator's value verdict and who they would recommend it to.

For a small, clear request, skip a separate approval round and keep moving; don't create a bureaucratic process. Once confirmed—or when the creator clearly asked you to proceed—combine the experience with the separate research card. Keep manufacturer claims, independent results, and the creator's observations distinct. Default to the recording outline above unless the creator requested another format. Follow the channel's saved language and voice, include an honest buying verdict, keep technical facts sourced, and include demo/B-roll cues where useful. Save the finished deliverable using the rules above and link the saved Markdown file in your response.

## Quality bar

- The creator's firsthand experience is the backbone of a review script; researched facts support it.
- An interview question must request a specific lived observation, event, measurement, or preference.
- Ask one question per turn, adapt, and don't repeat.
- Don't force every category. Prefer fewer strong, specific examples over a shallow ratings survey.
- Separate creator-observed results from estimates, memory, manufacturer claims, and public anecdotes.
- Never turn this interview into pressure to endorse the product. A negative, mixed, or “not enough experience yet” verdict is valid.
