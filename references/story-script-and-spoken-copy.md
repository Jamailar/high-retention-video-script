# Story, Script, And Spoken Copy

Use this reference after the core result or point and presentation architecture are selected. It turns real material into a natural direct explanation, workflow, argument, test, or story, then into a retention-designed and executable audiovisual script.

## Research Basis

This workflow combines:

- concrete lesson -> story -> hook development and speakability pressure tests from the open Indy Hall video-script skill: https://gist.github.com/alexknowshtml/6a1e4d336a6d51c6231bd6bd9a3f0d17
- platform-specific hook, section, demonstration, and read-aloud guidance from the open `creator-stack`: https://github.com/kenneth-liao/ai-launchpad-marketplace/tree/main/creator-stack/skills
- production-script discipline from local dialogue-video workflows: one visible beat per row, meaningful reaction/silence beats, and timing from actual speech
- local writing, copy, strategy, and voice-analysis workflows: start from a real human tension, translate facts into felt value, preserve author voice, and judge every line by strategy and execution
- content diagnosis, hook-as-content-sample, script-flow, resonance, and AI-pattern review principles independently adapted from `dontbesilent2025/dbskill`: https://github.com/dontbesilent2025/dbskill

Frameworks are selection tools. Do not force every video into the same three-act template.

## One Lesson And One Change

Before outlining, write:

```yaml
single_lesson: one actionable or perspective-changing sentence
viewer_change:
  before: what the viewer currently believes, feels, understands, or does
  after: what the viewer should believe, feel, understand, or do
proof_that_earns_change: the strongest available demonstration, result, story, or evidence
```

If the lesson requires “and” to join unrelated outcomes, split the video or choose one primary promise.

## Narrative Architecture Selector

Choose the architecture from the viewer's question and proof, not creator preference.

| Architecture | Use when | Recommended progression |
| --- | --- | --- |
| Tutorial / workflow | Viewer wants to complete a task | result preview -> broken current way -> method -> setup only when needed -> real input -> guided steps -> result -> failure/objection -> reuse -> first action |
| Problem / mechanism / proof | Viewer sees a symptom but not the cause | pain -> false assumption -> mechanism -> demonstration -> implication -> action |
| Case story / transformation | A specific person, project, or moment proves the lesson | consequence or vivid moment -> prior state -> conflict -> decision -> change -> evidence -> lesson -> invitation |
| Experiment / challenge | A clear question can be tested | question/stakes -> rules -> attempt -> complication -> result -> limitation -> takeaway |
| Comparison / review | Viewer is making a decision | decision tension -> criteria -> test 1 -> test 2 -> tradeoffs -> fit by audience -> verdict |
| Launch / reveal | New product or capability is the news | broken state -> result/reveal -> method -> strongest use case -> proof -> limitation -> CTA |
| Argument / myth correction | Existing belief blocks action | familiar belief -> contradiction -> evidence -> counterargument -> revised frame -> consequence |

Keep 3-5 main sections for most videos. Long videos may have more chapters, but each chapter still needs a viewer question, proof, and state change.

## Section Spine

Build the content progression before full dialogue. A tutorial section may advance task completion without creating conflict.

| field | requirement |
| --- | --- |
| `section` | Short functional name |
| `section_function` | Result, definition, instruction, mechanism, proof, limitation, payoff, or action; use setup/complication only for a narrative architecture |
| `viewer_question` | What the viewer actively wants answered here |
| `state_before` | Current belief, emotion, understanding, or intent |
| `exit_risk` | Boredom, confusion, disbelief, mismatch, overload, or satisfaction too early |
| `event_or_point` | What actually happens or is learned |
| `proof` | What makes the beat believable |
| `state_after` | Observable change caused by the beat |
| `earned_next_question` | Why the next section now matters |

Reject a section when `state_before` and `state_after` are effectively the same. Context that does not change state must be compressed, visualized, moved later, or removed.

## Question-Payoff Ledger

Open loops are promises, not decoration. Track them explicitly.

| field | definition |
| --- | --- |
| `loop_id` | Stable identifier |
| `question` | Exact viewer question |
| `opened_at` | Timestamp or clock mark |
| `why_it_matters` | Viewer stake |
| `partial_payoff` | Useful early answer, proof, or progress |
| `fully_paid_at` | Timestamp or clock mark |
| `proof` | Evidence that closes the question |
| `next_question` | New question earned by the answer |

Rules:

- Keep no more than two meaningful loops unresolved at once.
- Confirm the package promise immediately; do not make the viewer wonder whether they clicked the correct video.
- Provide progressive value before full closure.
- A new loop should usually arise from an answer, not from withholding basic context.
- Close every important loop before the CTA unless the video explicitly continues as a series.
- Never use repeated “wait until the end” language to compensate for weak middle sections.

## Progressive Payoff Pattern

Use the clock as a payoff scaffold:

- **12:** establish relevance, stakes, and package truth.
- **3:** first tangible reward or proof.
- **6:** central method, mechanism, or decisive explanation.
- **9:** larger transformation, second proof, consequence, or compounding value.
- **Finish:** full closure and one credible next action.

This is not a command to hide the answer until 9 or finish. Early payoffs build trust; later payoffs deepen value.

## Four-Pass Drafting

The order is deliberate. Do not start by assigning twelve clock points and then filling them with sentences.

### Pass 1: Human Rough Draft

Write the complete thought as the creator would explain it to one intelligent friend. Do not add timestamps, HKRR labels, or edit fields yet.

The draft must contain:

- one concrete result, answer, action, event, test, or decision appropriate to the selected architecture
- one workflow, demonstration, comparison, argument, test, or story that carries proof
- one honest limit or tradeoff when material; a failed attempt is optional, never compulsory
- only the background required for the next instruction or idea

Use 3-5 functional turns. In a tutorial, each turn should complete or clarify the next part of the viewer's task. In a story, each turn may instead cause or answer the previous dramatic question. Preserve natural fragments and uneven sentence lengths when supported by voice evidence.

### Direct Utility Tutorial Standard

For a product introduction, app walkthrough, or activation tutorial:

1. Show the finished result before explaining the process.
2. Define the tool in one sentence.
3. Demonstrate the real entry point, input, and workflow.
4. Repeat the result in inspectable detail after the viewer understands how it was made.
5. State the human, technical, privacy, or fit boundary plainly.
6. End with one executable first action.

Do not manufacture an emotional arc. Satisfaction can come from seeing progress, clarity, a clean output, a solved task, or a useful distinction. Resonance can be one precise recognition of the viewer's situation; it does not require a performed struggle.

### Pass 2: Story And Retention Design

Write only:

- section function
- viewer state and question
- payoff and proof
- HKRR role
- clock mark
- planned visual engine

Map these decisions onto the rough draft. Cut, move, or convert weak material into pictures. Do not add explanatory text merely to fill a missing clock point; a stimulus can be visual, sonic, emotional, or silent.

### Pass 3: Spoken Rewrite

Rewrite the complete lines the creator will actually say after the story and retention design are sound. Use:

- one thought per sentence
- concrete subjects, verbs, objects, results, and moments
- the audience's real vocabulary where evidence exists
- contractions, natural fragments, and pauses that match the creator's voice
- specific details before abstract interpretation
- direct explanation only when demonstration alone would be ambiguous

Write the line for the ear. Readability on a page is not enough.

Run the exact drop-off and AI-pattern audit in `human-voice-and-editorial-audit.md`. Rewrite from source details and creator intent rather than decorating generic lines with filler.

### Pass 4: Audiovisual Draft

For every spoken group, attach:

- A-roll performance or speaker
- B-roll, screen action, object, result, diagram, or existing asset
- exact on-screen text, if needed
- sync sound, music, sound effect, or deliberate silence
- edit transition or hold
- proof purpose and viewer-state purpose

Do not add B-roll merely to cover a cut. It must prove, clarify, contrast, orient, or refresh attention.

## Spoken Line Standard

Every line should pass these checks:

1. **One breath:** a normal speaker can deliver it comfortably. Split long clauses.
2. **One job:** it primarily advances story, proof, emotion, instruction, transition, or action.
3. **Concrete:** replace abstractions with a screen, action, object, decision, number, or consequence.
4. **Front-loaded:** place the useful or surprising part before explanatory padding.
5. **Distinct:** it does not restate the previous line, title, or on-screen text.
6. **Speakable:** no formal connective exists only because the line was written.
7. **Showable:** the planned picture can support or meaningfully contrast it.
8. **Trustworthy:** wording does not outrun the evidence.

Common rewrites:

- “接下来我们将进行安装” -> “先装上它。”
- “通过该功能可以实现内容整理” -> “把这些散乱素材拖进来，它先替你理清。”
- “综上所述” -> state the actual conclusion
- “它显著提升效率” -> show the old time, new time, or exact work removed

Do not mechanically add filler words such as “其实”, “你看”, or “说实话”. Use them only if the creator's real samples support them and they perform a conversational function.

## Creator Voice Calibration

When voice samples exist, extract:

- average sentence and paragraph length
- short/long sentence alternation
- preferred openings and transitions
- ratio of “I” experience to “you” instruction
- humor, directness, warmth, formality, and emotional restraint
- repeated phrases worth preserving
- phrases, rhetorical patterns, or tones the creator avoids
- evidence and story habits in the creator's best-performing work

Use 3-5 representative samples when available. Preserve exact phrases only when the creator owns them or supplied them. Do not mimic another creator's distinctive wording; adapt the structural technique.

Extract at least three usable creator fingerprints for a polished creator-led script:

- a real event or failed attempt
- a stated opinion, preference, or disagreement
- a concrete detail only this creator would choose to mention
- an honest limitation, doubt, or change of mind
- a repeated phrase or sentence habit confirmed across samples

Place fingerprints where they improve explanation, trust, or story, not as decorative personality. A direct tutorial does not need a personal anecdote in the opening, middle, and ending. If voice evidence is missing, mark creator-led copy provisional and request a read-through correction before production.

## Proof Adjacency

Place proof close to the claim it supports.

- Product result claim -> show the actual result.
- Speed claim -> show timing or a clearly described test.
- User pain claim -> cite real audience language or mark it as an inference.
- Quality claim -> show comparison criteria, output detail, or limitation.
- AI capability claim -> show source input, intermediate artifact, output, and revision or failure behavior.

Avoid a long gap between claim and proof. If proof appears later, signal what will verify the claim and provide a smaller early confirmation.

## Visual Writing

Ask of every beat:

- What is the first readable image?
- What changes on screen?
- Where should the eye look?
- What must remain visible long enough to understand?
- Which image carries information so the voice can be shorter?
- Is the result shown at inspectable scale rather than as atmosphere?

For UI videos, specify observable state transitions. For physical products, specify tactile action and conditions. For talking-head videos, specify expression, gesture, eyeline, framing, and when the product or artifact enters frame.

## CTA Design

The CTA completes the viewer journey. It should be:

- one action, stated once
- proportionate to trust earned
- connected to the promised result
- possible now
- specific enough to verify completion

Good tutorial CTA: collect three real source items and run the demonstrated workflow. Weak CTA: “follow for more” when the video promised activation.

## Script Pressure Test

Before timing:

- Can the lesson be stated in one sentence?
- Does a concrete story, test, or workflow prove it?
- Does every section change viewer state?
- Are the package and first beat clearly connected without repetition?
- Is the first major reward delivered by clock point 3?
- Are questions answered before attention debt accumulates?
- Does each important claim have nearby proof?
- Does the wording sound like this creator when read aloud?
- Does the draft contain at least three sourced creator fingerprints rather than generic personality cues?
- Can any full paragraph be pasted into another product video unchanged? If yes, replace it with a sourced detail, opinion, action, or proof.
- Where is the first exact sentence or visual a cold viewer may leave, and has that risk been repaired?
- Can every planned picture be captured or sourced?
- Does the ending close the primary promise and produce one action?
