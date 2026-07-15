# Human Voice And Editorial Audit

Use this reference before polishing a spoken draft and again before delivery. It prevents a complete framework from producing empty, uniform, machine-like copy.

## Research Basis

This workflow independently adapts useful diagnostic ideas from the open `dontbesilent2025/dbskill` repository, especially its content, hook, script-flow, resonance, spread, and AI-pattern review skills: https://github.com/dontbesilent2025/dbskill

The source repository is licensed CC BY-NC 4.0. Reuse the general editorial questions and workflow principles with attribution; do not copy its prose, proprietary examples, or distinctive checklists into commercial output.

## The Core Distinction

Human-sounding copy is not copy with slang added. It has evidence of a mind at work:

- a specific reason for speaking
- a judgment that could be disagreed with
- selective attention rather than encyclopedic coverage
- concrete memory, action, object, screen, consequence, or proof
- uneven but intentional rhythm
- limits, uncertainty, or tradeoffs where they are real

AI-sounding copy often fails because it is too complete, too smooth, and too evenly distributed. Fix the source and thought, not only the wording.

Human-sounding also does not mean story-shaped. A concise tutorial can sound human through selection, specificity, direct judgment, useful omissions, and natural speech. Never add a confession, struggle, reversal, or creator origin merely to satisfy a “human voice” pattern.

## Creator Evidence Gate

A production-ready script should use at least three sourced creator fingerprints. A fingerprint may be:

- a real event the creator experienced
- an opinion or preference stated by the creator
- a concrete detail only the creator would know
- an admitted failed attempt, limitation, doubt, or change of mind
- a repeated phrase, sentence habit, or degree of directness from 3-5 samples

Mark the provenance internally. Do not invent any fingerprint.

If the user has not supplied enough evidence, ask one compact follow-up that invites natural speech:

```text
先别给我标准答案。像跟朋友讲一样说说：这件事为什么让你想拍？你最不满意或最意外的那一刻是什么？你真正相信、但别人未必同意的判断是什么？手里哪段画面或结果能证明它？
```

If the user prefers to proceed without answering, label the script `provisional_voice` and request a read-through correction before shooting.

## Content Reality Test

Before line editing, answer in one sentence each:

| Test | Passing answer |
| --- | --- |
| Why now? | A real trigger, event, result, conflict, or decision |
| Why this creator? | Experience, access, proof, or a defensible perspective |
| One point? | One claim or change that can survive deleting the feature list |
| Whose side? | A specific audience tension or unfair burden the video recognizes |
| What can be shown? | A recurring artifact, action, comparison, screen, result, or source |
| What changes? | A belief, feeling, understanding, decision, or action by the end |

If these answers are vague, do not optimize the hook. Return to material and angle selection.

These answers guide selection; they do not all belong in the spoken script. In a utility tutorial, “why this creator” and “why now” may remain internal while the opening shows the result.

## Draft Without The Framework

Write the first complete spoken version without timestamps, HKRR labels, score targets, or twelve clock blocks.

Use these rules:

1. Write what the creator would say after the camera has been recording for ten minutes, not their formal introduction.
2. Let each paragraph do one job: reveal, test, explain, react, prove, decide, or invite.
3. Use a real action or detail whenever a sentence becomes abstract.
4. Keep useful incompleteness. The creator does not need to pre-answer every possible objection.
5. Vary sentence shapes because the thought varies, not because a rhythm formula demands it.
6. Do not force a moral or perfect conclusion onto every paragraph.

Only after the draft works as speech should HKRR and the clock strengthen its distribution.

## Exact Drop-Off Audit

Do not say “the middle is weak.” Locate the first exact sentence, transition, or visual where the viewer may leave.

### Pass 1: Logic Continuity

Flag a line when:

- it assumes knowledge the viewer has not received
- it states a conclusion before the reason or proof
- it changes topic without carrying a question forward
- it contradicts the title, hook, previous line, or visible result
- it creates an open loop that never pays off

For each flag write: `exact line -> viewer's unanswered question -> smallest repair`.

### Pass 2: Information Density

Flag a section when:

- several lines restate one meaning
- a list of features replaces a decision or story
- background arrives before the viewer needs it
- explanation continues after the proof already made the point
- every useful fact is included merely because it was researched

Repair in this order: delete, combine, move proof earlier, convert explanation to picture, then add only the missing bridge.

### Pass 3: Spoken Fluency

Flag a line when:

- it is difficult to say in one comfortable breath
- its key word arrives too late
- it contains stacked qualifications or abstract nouns
- it uses formal written verbs where a concrete spoken verb exists
- three adjacent sentences share the same opening, length, or syntax

Around 28-30 Chinese characters is a useful warning threshold, not a ban. A longer sentence can stay when the creator naturally uses it and the breath works.

## AI-Pattern Diagnostic

These are clues, not forbidden words. Mark exact evidence and explain why it damages this script.

### Structure Patterns

- every paragraph follows claim -> explanation -> perfect conclusion
- repeated “first, next, finally” scaffolding
- dense “not X but Y” reversals
- manufactured reader questions immediately answered by the narrator
- symmetrical lists that exist because the framework had fields
- uniform emotional intensity with no stillness, uncertainty, or reaction
- a canned pain -> promise -> feature -> CTA sequence

### Language Patterns

- generic claims that could describe any product
- repeated sentence openings and evenly sized sentences
- translation-like phrasing built around “as, regarding, based on, carry out”
- excessive labels such as “core logic,” “underlying essence,” or “value proposition” without a visible action
- synonym replacement that makes the sentence less like the creator
- transitions that announce structure instead of continuing thought

### Content Patterns

- a fake personal story or fake customer voice
- every objection is preemptively answered
- all researched knowledge is dumped into the script
- no creator preference, tradeoff, uncertainty, or cost
- features are named without showing why the viewer should care now
- the hook is more dramatic than the actual material

## Rewrite Method

For each high-risk line:

1. State what the creator is genuinely trying to mean.
2. Find the source detail, action, proof, or opinion that supports it.
3. Write the shortest speakable sentence that preserves that meaning.
4. Let the picture carry any remaining explanation.
5. Read the previous line, revised line, and next line aloud as one passage.

Do not “humanize” with random filler, typos, trendy slang, fake self-deprecation, or forced emotion.

## Practical Guardrails

Use these as review signals rather than mathematical scoring:

- No three consecutive spoken lines should feel built from the same syntax.
- Avoid more than one prominent “not X but Y” reversal per minute unless it is the creator's natural pattern.
- Avoid more than two explicit sequence markers in a short video unless the content is a numbered tutorial.
- Every 30-45 seconds should include at least one concrete action, artifact, proof, reaction, or visual change.
- Name a feature only when it is visible, necessary for the decision, or directly tied to a consequence.
- Include at least three sourced creator fingerprints in a polished creator-led video.
- Preserve at least one honest limitation or tradeoff when it materially affects trust.

## Final Voice Verdict

Record a compact verdict in the final HTML:

```yaml
voice_status: verified | provisional | mismatched
creator_fingerprints_used:
  - timestamp and sourced detail
first_drop_off_risk:
  - timestamp, exact line or visual, reason
generic_line_check:
  - strongest remaining line that could fit another product, or none
priority_rewrite:
  - one concrete change before shooting
```

A script is not production-ready when `voice_status` is `mismatched`, when invented biography remains, or when a high-risk drop-off point is unresolved.
