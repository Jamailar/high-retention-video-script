---
name: high-retention-video-script
description: Create, revise, or audit high-retention product videos, app tutorials, launch explainers, creator education videos, social ads, case stories, reviews, and walkthroughs. Grounded in the HKRR and clock theories publicly explained by 影视飓风, it starts from the creator's real material, point of view, speaking samples, audience tension, and available proof; develops one strong content proposition and package; writes a natural spoken draft; then uses HKRR and a 12-point stimulus clock to strengthen retention without flattening the creator's voice. Delivers one concise, production-ready HTML package with a readable word-for-word script, A-roll/B-roll timeline, capture checklist, circular clock, and evidence-based QC.
---

# High Retention Video Script

## Objective

Turn the user's actual knowledge, lived stake, creator voice, audience evidence, product truth, references, and production constraints into a video that feels worth saying and worth watching.

The order matters:

`raw material -> viewer job and format -> one core result or point -> title and hook -> human rough draft -> HKRR and clock -> timed AV script -> capture -> edit -> QC`

HKRR and the stimulus clock are design and diagnosis tools. They must strengthen a real piece of content; they must never generate twelve equal blocks of explanatory copy or turn the video into a feature tour.

## Theory Attribution

The conceptual foundation of this Skill is the HKRR theory and the 12-point clock theory publicly explained in 影视飓风 content, including the Douyin material published by the account `飓风世界`. This repository is an independent implementation for AI-assisted script design and production planning; it is not an official 影视飓风 project and does not imply endorsement.

The default handoff is one self-contained HTML file. It can generate a simplified shooting PNG locally. Create an optional capture CSV only when another operator explicitly needs sortable data.

## Non-Negotiable Rules

1. Start from what the viewer needs to see, understand, decide, or complete, not from empty output fields.
2. Classify the video job and architecture before ideation. A utility tutorial defaults to result-first demonstration; never force it into a confession, failure story, conflict, or dramatic reversal.
3. One video carries one core result, claim, task, or change. Other points are proof or support.
4. Use the creator's exact experiences, opinions, details, uncertainty, and habitual language when relevant and sourced. Never invent personal history or verbal quirks to make a direct tutorial feel "human."
5. A polished creator-led script requires creator-voice evidence. Without it, deliver a clearly labeled provisional draft and ask for a read-through, voice note, transcript, or corrections. This does not require inserting autobiography into a screen-led tutorial.
6. The hook is a truthful sample of the strongest content. For a tool tutorial, show the usable result immediately and explain it only after the viewer can see it.
7. HKRR must all be designed: Happiness, Knowledge, Resonance, and Rhythm. Rhythm includes the 12-point clock and micro pacing.
8. Write the human rough draft before mapping HKRR. A clock point may be a look, pause, artifact, proof reveal, sound change, or visual reset; it does not require a new explanatory sentence.
9. Important claims require visible proof. Reduce unsupported wording rather than hiding the gap in editing instructions.
10. Write for the mouth and the screen. Read the script aloud and show what the words cannot efficiently explain.
11. Final production instructions must be simpler than the reasoning that created them.

## Required References

For a full concept, script, rewrite, or production package, read these before drafting. For a narrow audit, load the references governing the audited surface plus `output-specs-and-qc.md`. Before generating HTML, always read the HTML template.

- `references/context-intake-and-source-use.md`: unstructured intake, creator evidence, sources, and assumptions.
- `references/product-script-taxonomy.md`: product type, video job, trust mode, proof strategy, and format fit.
- `references/ideation-packaging-and-titles.md`: angle, title, cover, first frame, package selection, and hook contract.
- `references/story-script-and-spoken-copy.md`: one-point story design and natural spoken drafting.
- `references/human-voice-and-editorial-audit.md`: creator interview, AI-pattern diagnosis, drop-off audit, and human rewrite gates.
- `references/clock-theory.md`: HKRR design and the mandatory 12-point stimulus clock.
- `references/timing-pacing-and-retention.md`: read-through timing, energy, micro pacing, and platform fit.
- `references/creator-production-system.md`: capture planning, audio-first assembly, and production feasibility.
- `references/output-specs-and-qc.md`: concise HTML contract, execution tables, validation, and scores.
- `assets/video-script-package-template.html`: required self-contained final layout.

## Working Modes

| Mode | Use when | Result |
| --- | --- | --- |
| `create` | Starting from an idea, product, material dump, or reference | Complete concept and production package |
| `revise` | A script or package exists | Exact diagnosis, revised script, compact change record |
| `package` | Content is real but title, cover, or hook is weak | Three package routes internally; selected contract for the user |
| `audit` | User wants a retention, voice, or production review | Line-specific risks and prioritized fixes |
| `learn` | Published performance data exists | Timestamp-linked diagnosis and reusable creator learnings |

## Audience-First, Human-Sounding Workflow

Complete the gates in order. Internal candidate lists and diagnostic tables may remain in working memory or temporary files. The final HTML exposes decisions and evidence, not private chain-of-thought.

### Gate 0: Gather Material And Voice

When context is thin, ask one broad question:

```text
把你认为可能有用的东西一次性发来，不用整理。产品资料、文件路径、参考视频、旧稿、评论、截图、录屏、数据、你自己说话或写作的样本、真实经历、不同意的观点和禁忌都可以。我先整理哪些能用，再和你确认这条视频到底要说什么。
```

Search provided files, workspace material, knowledge sources, and accessible references before asking narrow questions. Build an internal evidence pack containing:

- verified facts, claims, proof, assets, permissions, and constraints
- the creator's stake when it affects credibility or selection; keep it internal when the viewer only needs a direct demonstration
- 3-5 voice fingerprints from user-owned language when available
- audience situation, exact language, current workaround, desired result, objection, and proof threshold
- reference structures worth adapting and distinctive wording that must not be copied
- facts, inferences, assumptions, missing context, and `do_not_claim` items

Classify context as `sufficient`, `partial`, or `weak`. Ask again only for blocking gaps. Do not manufacture anecdotes to make partial context look complete.

**Gate condition:** at least one real result, demonstration, source, test, event, or defensible point can carry the video, and the provenance of every important claim is known.

### Gate 1: Find The Content Worth Watching

Diagnose before packaging. First choose the architecture from the viewer's job:

| Viewer job | Default opening | Default progression | Do not force |
| --- | --- | --- | --- |
| Utility introduction / activation tutorial | Finished result in the first beat, normally 0-8 seconds; if a cited proof/source is itself useful, show the result in the next beat | result/proof -> one-sentence definition -> real input -> guided workflow -> output -> limitation -> action | backstory, confession, conflict, reversal |
| Launch / reveal | Product or capability reveal | result -> mechanism -> strongest use -> proof -> limitation -> CTA | founder biography before value |
| Education / mechanism | Useful insight or demonstration | answer/proof -> explanation -> application -> consequence -> action | artificial personal failure |
| Case / experiment / review | Consequence, question, or decision evidence | use the matching case, test, or comparison architecture | generic product tour |

Then reduce the material to:

- **viewer tension:** the unsaid frustration, desire, conflict, or decision already present
- **viewer job:** what the viewer came to understand, judge, or complete
- **creator stake:** why this creator is credible or invested, only when it changes trust or meaning
- **core result or point:** one sentence that defines the useful payoff
- **mechanism or change:** what the viewer will understand differently
- **content engine:** a result-led demonstration, workflow, comparison, test, teardown, argument, or story selected for this video job
- **proof engine:** what can repeatedly be shown
- **stance:** whose side the video is on and what easy answer it refuses

Generate 3-5 meaningfully different angles only when needed. Select the direction with the strongest combination of relevance, proof, visual engine, emotional force, and production feasibility. Do not confuse “covering everything” with depth.

**Gate condition:** the video can be explained as “one useful result or point carried by one fitting proof engine,” not a list of features or theories. A utility tutorial must not require the viewer to wait through setup or creator drama before seeing the result.

### Gate 2: Build A Truthful Package

Create title, cover or first frame, hook, and payoff from the selected content. The hook must contain:

- the identifiable topic
- a concrete reason to continue
- immediate credibility, conflict, or proof

Explore title families internally, then keep three genuinely different finalists for selection or testing. The selected title must be speakable, specific, credible, and fully payable by the footage. The first frame adds information rather than repeating the title. The opening confirms the promised video has begun, then creates progress.

Reject a hook that only greets, announces an agenda, stacks pain and promises, asks a fake viewer question, gives away the whole answer, or works only because the cover explains it.

**Gate condition:** a cold viewer can identify the topic, reason to stay, and source of credibility from the opening itself.

### Gate 3: Write The Human Rough Draft

Write a complete rough spoken draft before adding timestamps, HKRR labels, or clock marks.

1. Follow the selected architecture. For a utility tutorial, use `result -> what it is -> how to use it -> output -> limitation -> action` and keep the product or screen visible.
2. Use 3-5 functional sections. They may be instructional steps; they do not need conflict or story turns.
3. Start from a concrete result, action, judgment, or useful answer, not a category definition or creator origin story.
4. Add creator fingerprints only where they improve clarity, trust, or natural delivery. Do not insert a failure, confession, or reversal merely to sound human.
5. Preserve useful asymmetry: fragments, short reactions, occasional longer thought, hesitation, or qualification when natural.
6. Prefer specific nouns, verbs, screens, objects, and consequences over abstract labels.
7. Give only the context needed to perform or understand the next step.
8. Read it aloud. Mark every place the mouth resists or the viewer could ask “so what?”

Do not polish with synonyms. Fix weak content by adding a real detail, opinion, conflict, action, or proof; otherwise delete it.

**Gate condition:** the draft delivers the selected viewer job without architecture mismatch. A tool tutorial shows its result before explanation, contains no decorative drama, and still uses the user's real product, material, constraints, and language.

### Gate 4: Apply HKRR And The 12-Point Clock

Now design all four elements around the existing draft:

- **Happiness:** surprise, relief, humor, satisfaction, delight, or a visible small win
- **Knowledge:** method, mechanism, demonstration, decision rule, or usable insight
- **Resonance:** the viewer's pain, identity, desire, fear, frustration, or self-recognition
- **Rhythm:** the full distribution of big/small stimuli plus sentence cadence, silence, density, cuts, sound, and visual change

Map the full runtime proportionally to 12 points. `12/3/6/9` are structural big stimuli; the other eight refresh attention; Finish repays the promise and lands the action. Alternate HKRR effects like a clock cycle. A big point changes belief, emotion, trust, or intent; louder music alone does not qualify.

For each point record only what production needs: exact time, HKRR role, stimulus or payoff, and visible/audible execution. When the map forces filler, change the map or runtime instead of adding words.

**Gate condition:** all four elements are present, the cardinal points are meaningfully stronger, and no 20-30 second stretch is only abstract explanation.

### Gate 5: Rewrite And Run The Drop-Off Audit

Integrate the retention design into the spoken draft, then inspect exact lines in three passes:

1. **Logic:** Does each sentence earn the next one? Is a conclusion missing its reason or proof?
2. **Density:** Is any section repeating one meaning, listing features, or front-loading background?
3. **Speech:** Is the sentence comfortable in one breath and natural in this creator's mouth?

Run the AI-pattern audit from `human-voice-and-editorial-audit.md`. Treat patterns as diagnostic clues, not a banned-word style recipe. Flag exact lines and rewrite from creator evidence. Preserve intentional repetition or formality when it belongs to the creator.

**Gate condition:** the audit names no unresolved high-risk drop-off point, no invented personal detail, and no paragraph that could be pasted into any product video unchanged.

### Gate 6: Time And Convert To Production

Perform a real read-through when possible; actual time overrides character estimates. Include breaths, pauses, UI latency, reactions, result holds, and 10-15% edit handles.

Create two authoritative surfaces:

1. **Word-for-word AV timeline:** done, exact time/clock, complete spoken line, A-roll/B-roll shot IDs and visual action, concise edit/audio cue.
2. **Capture checklist:** done, shot ID/type/priority, what to record, start-action-end, filename/privacy, observable acceptance criterion.

Build the audio spine first. Every edit source ID must resolve to one capture row. Add B-roll only to prove, clarify, contrast, or refresh attention.

### Gate 7: Cold-Viewer QC And Deliver

Review the result as someone who did not attend the planning conversation:

- Would the target viewer choose it from title and first frame?
- Does the opening architecture match the viewer's intent, or is a direct tutorial wasting time on setup, biography, pain, or reversal?
- What is the first exact sentence or visual where they may leave, and why?
- Is the creator saying something they actually mean, or performing a framework?
- Does each section create emotion, understanding, recognition, or movement?
- Are HKRR roles rotating rather than clustering into one long lecture?
- Can a shooter and editor act without asking what a row means?

Score H, K, R, and Rhythm from 0-5 with exact timestamp evidence, deficiency, and one revision action. Revise before delivery when any element is below 3, the total is below 15, a creator-voice final lacks voice evidence, a major claim lacks proof, a timed line does not fit, or an edit source lacks a capture row.

## Final HTML Contract

Use `assets/video-script-package-template.html`. Keep it offline, self-contained, concise, and readable in this order:

1. `summary`: selected title, one-sentence premise, runtime, platform, context/voice status, HKRR total, and progress.
2. `script`: the primary word-for-word AV timeline. This is the script and edit source of truth, with no duplicate edit table.
3. `rhythm`: compact HKRR cards, proportional A/B timeline, and mandatory circular 12-point clock. Every point shows mark, exact time, HKRR role, and stimulus around the circumference.
4. `shoot`: one simplified capture checklist with no more than five visible columns.
5. `qc`: compact creator-voice, cold-viewer, HKRR, proof, and production diagnosis with one priority revision.

Keep detailed sources collapsed. Do not show discarded angle lists, twelve title drafts, a question-payoff ledger, a viewer-journey table, separate AV/edit tables, or raw score worksheets unless the user explicitly asks. Those are working methods, not the shooting interface.

Preserve only interactions that reduce work: persistent completion checks, unfinished-only filtering, progress, print, reset, and local generation/save of a simplified shooting PNG. Keep the Beav gradient, embedded icon, and name unless another brand is requested.

The PNG includes title, premise, runtime/platform, compact HKRR guidance, the circular clock, and every capture row. It is a field sheet, not a screenshot of the full HTML.

Return no more than 1-2 user-facing files.

## Revision And Learning

When performance data exists, align package, script timestamps, and stimulus points with metrics actually available. Diagnose the first place viewer behavior diverges from the planned state change. Classify the cause as package mismatch, relevance loss, weak content, payoff debt, proof failure, confusion, pacing, production quality, or CTA friction. Preserve reusable creator learnings, but treat one video's result as a hypothesis rather than a law.

## Long HTML Write Rule

For a long package, copy the template, replace one uniquely anchored section at a time, then validate the complete file. Remove every `{{PLACEHOLDER}}`, delete unused template rows, verify section IDs, timestamp continuity, clock times, shot-ID resolution, local interactions, offline assets, and readable final copy before handoff.
