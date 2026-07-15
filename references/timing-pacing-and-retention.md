# Timing, Pacing, And Retention

Use this reference after the section spine exists and before production tables are finalized. Timing is not guessed from paragraph length. Pacing is not “cut faster.” Retention comes from the interaction of promise, payoff, comprehension, proof, emotional contrast, speech, visuals, sound, and stimulus distribution.

## Research Basis

- YouTube identifies intro retention, top moments, spikes, and dips as evidence for what held, confused, or lost viewers, and recommends moving compelling later moments earlier when appropriate. Source: https://support.google.com/youtube/answer/9314415
- YouTube's official recommendation guidance separates appeal, engagement, and satisfaction, and requires the opening to deliver on title/thumbnail expectations. Source: https://support.google.com/youtube/answer/16559650
- TikTok Creative Codes uses hook/body/close, early value, native production, sound, movement, text, transitions, and scene changes as attention tools. Source: https://ads.tiktok.com/business/library/Creative_Codes_One_Pager.pdf
- Local dialogue-video production practice estimates speech before generation, preserves breathing and reaction time, builds dialogue edits from audio, and rejects repeated lines or dead gaps.
- Open product-video and talking-head skills provide useful production heuristics: one message, exact beat sums, first-second hooks for fast social, one-breath lines, and explicit CTA holds. Source: https://github.com/sanky369/vibe-building-skills/tree/main/skills/creative

Treat numerical guidance as a starting estimate. The creator's actual timed read and published viewer data outrank generic heuristics.

## Two Rhythm Layers

### Macro Rhythm: 12-Point Stimulus Clock

The clock controls where attention, belief, emotion, and payoff are refreshed across the whole runtime.

- 12/3/6/9 are structural big stimuli.
- The other eight points are smaller refreshes.
- Finish closes the primary promise and action.
- Each mark must change viewer state; louder sound alone is not a valid change.

The clock is mandatory. See `clock-theory.md` for the full fields and HKRR integration.

### Micro Pacing: Inside Each Clock Segment

Micro pacing controls how the beat is experienced:

- speech rate and sentence length
- pause, breath, reaction, and silence
- information density
- visual change and eye guidance
- sound onset, release, and contrast
- demonstration latency and result holds
- cut timing and transition clarity

Good macro rhythm cannot rescue unreadable micro pacing. Fast micro pacing cannot rescue an empty macro clock.

## Runtime Budget

Start from the platform and viewer job, then derive the amount of content. Do not write freely and force the result into a duration later.

| Runtime | Typical use | Clock interval | Content discipline |
| --- | --- | --- | --- |
| 15-30s | single result, ad, reveal, one tip | about 1.25-2.5s per mark | one message, one proof path, minimal setup |
| 30-60s | short tutorial, story, comparison | about 2.5-5s per mark | one lesson, usually no more than two main points |
| 1-3min | case-driven tutorial or explainer | about 5-15s per mark | 3-5 sections, progressive proof |
| 5-10min | detailed tutorial or review | about 25-50s per mark | multiple demonstrations, objections, chapter-level clock marks |
| 10min+ | deep dive, documentary, course | proportional macro marks plus micro beats inside each | chapter architecture and repeated local question-payoff loops |

The 12 marks are proportional attention landmarks, not a demand for exactly 12 shots or sentences.

## Speech Estimation

Use these only for first-pass budgeting:

### Mandarin Chinese

- restrained or emotional delivery: about `150-190` Chinese characters per minute
- clear tutorial delivery: about `190-250` characters per minute
- energetic burst: about `240-300` characters per minute, not sustained for a full explanatory video

Do not count punctuation as spoken content. Dense numbers, English terms, UI labels, and unfamiliar names slow delivery.

### English

- conversational explanation: about `130-160` words per minute
- energetic short burst: up to about `170-190` words per minute when comprehension remains high

### Beat Allowance

Add time for:

- `0.3-0.8s` thought or reaction pauses when meaningful
- `0.8-1.5s` tail or edit handle around a visible beat when the shot needs room
- UI loading, cursor travel, typing, product response, gesture, and result inspection
- final CTA or product frame held long enough to read, usually at least 2 seconds for short-form

Keep a `10-15%` natural-performance margin. Do not solve an overlong script by asking the speaker to rush everything.

## Read-Through Protocol

The timed read is the source of truth.

1. Read in the intended performance style, not as quickly as possible.
2. Record the take or use a timer per section.
3. Mark every stumble, forced breath, unclear emphasis, and dead stretch.
4. Add real pause, gesture, UI, and result-hold durations.
5. Compare actual section times with planned ranges.
6. Cut repeated meaning first.
7. Replace written explanation with visible proof where possible.
8. Split one-breath failures.
9. Re-read until every section fits without rushing.

Record in the decision summary:

```yaml
timing_method: estimated | timed_read | asr_aligned
spoken_units: characters_or_words
planned_duration:
measured_read_duration:
visual_action_allowance:
timing_margin:
final_duration:
remaining_timing_risk:
```

When a real read is not possible, state that timing is estimated and require a table read before production.

## Energy Curve

Assign every clock mark an energy level from 1-5:

- 1: deliberate stillness, reflection, or simple orientation
- 2: calm explanation or setup
- 3: steady progress and normal demonstration
- 4: strong contrast, proof, emotional turn, or acceleration
- 5: structural peak, decisive reveal, major result, or high-stakes moment

Rules:

- Cardinal marks should usually create a stronger state change than adjacent marks, but not every cardinal mark needs energy 5.
- Do not keep more than two consecutive marks at energy 5; contrast is required for peaks to register.
- Use a lower-energy hold after dense information when comprehension needs time.
- Silence or stillness can be a strong stimulus when it changes expectation.
- Energy follows meaning. Avoid raising music, adding zooms, or accelerating cuts when the story has not earned it.

## Information Density

Control three loads separately:

1. **Verbal load:** new terms, clauses, numbers, instructions.
2. **Visual load:** simultaneous objects, UI regions, captions, motion, comparisons.
3. **Decision load:** choices or implications the viewer must evaluate.

Do not peak all three at once. When the voice introduces a new mechanism, simplify the screen. When a complex result is visible, shorten the spoken line and hold the frame.

One edit segment should usually advance one primary idea. Secondary HKRR effects may coexist, but comprehension still needs a clear hierarchy.

## Functional Attention Refreshes

Choose a refresh because of the current exit risk.

| Exit risk | Useful refresh |
| --- | --- |
| Disbelief | real artifact, live result, before/after, limitation |
| Confusion | simpler sentence, diagram, replay, cursor highlight, pause |
| Boredom | new question, concrete example, contrast, scene change |
| Emotional distance | audience quote, specific moment, consequence, identity cue |
| Overload | summary frame, silence, lower-energy hold, one key phrase |
| Satisfaction too early | show a deeper consequence, tradeoff, or next problem genuinely earned by the first answer |
| Repetition | cut the beat or convert it into new proof |

Music, transitions, movement, captions, zooms, speed ramps, and sound hits are execution devices. They are not retention reasons by themselves.

## Platform Adaptation

### Douyin / TikTok / Reels / Shorts

- start on action, result, conflict, or recognizable pain
- design for 9:16 and UI-safe text placement
- keep product, speaker, or proof visually identifiable at mobile size
- use sound deliberately but keep meaning understandable with captions
- shorten setup, reduce main points, and make each clock mark visibly distinct
- use the first frame as part of the hook, not as a static poster inserted before the video

### YouTube / Bilibili Long-Form

- title and thumbnail create the package; the first 30 seconds must validate it
- begin promised content quickly, then earn deeper context
- use chapter-level questions and local payoffs inside each macro clock segment
- make demonstrations inspectable; do not montage away the evidence
- prepare genuinely different package variants when testing is available

### Website / Landing Page / Product Page

- assume partial attention and possible muted autoplay
- show product/result early and make captions sufficient for orientation
- prioritize the single conversion job over creator-channel rituals
- hold CTA and product identity long enough to act

### Internal Training / Course

- comprehension and transfer outrank aggressive novelty
- use the clock for examples, practice, checks, and state changes rather than constant sensory interruption
- include prerequisites, failure modes, and an observable completion task

## Audio-First Assembly

For presenter, narration, interview, or dialogue-led video:

1. capture or place the clean spoken spine
2. cut repeated lines, false starts, and dead gaps
3. preserve deliberate breaths and reactions
4. align B-roll and screen proof to meaning, not arbitrary beat counts
5. place music and sound after speech intelligibility and proof timing work
6. verify captions against the final audio, preferably with ASR plus human correction

For dialogue handoffs, `0-0.25s` is a normal tight transition, `0.3-0.8s` can support thought or reaction, and pauses over 1 second should be deliberately scripted.

## Retention Review After Publishing

Use available data, not invented platform averages.

### Map Metrics To Script

| Signal | Possible meaning | Required review |
| --- | --- | --- |
| Low click choice / weak appeal | package is unclear, irrelevant, or uncompetitive | compare title-thumbnail hypotheses and audience fit |
| Early drop | package mismatch, weak relevance, repeated title, slow setup, poor first image | inspect first 30 seconds or first 25% for short-form |
| Gradual decline | payoff density or clarity is weakening | inspect question-payoff spacing and information load |
| Dip | boredom, confusion, mistrust, repetition, or production problem | align exact timestamp with line, visual, and clock mark |
| Spike / replay | high value, emotional resonance, share moment, or confusion | inspect comments and context before labeling it positive |
| Strong saves | reusable knowledge or reference value | identify Knowledge design worth repeating |
| Strong shares/comments | identity, emotion, utility, controversy, or social currency | identify Resonance/Happiness trigger and audience language |
| CTA drop | action is too large, late, generic, or disconnected | compare trust earned with requested action |

### Learning Loop

1. Compare the video with the creator's own similar videos.
2. Diagnose the first meaningful deviation from the planned viewer journey.
3. Separate package failure from script, production, and CTA failure.
4. Write a timestamped revision hypothesis.
5. Define a limited test with success and failure criteria.
6. Update the creator profile only after repeated evidence.

Do not infer causality from one data point. State sample size and confidence. A spike may mean delight or confusion; a click increase with lower watch time may mean the package overpromised.

## Pacing QC

Before production, verify:

- exact runtime arithmetic works
- a timed read exists or is explicitly required
- package promise is acknowledged immediately
- first tangible payoff arrives by clock point 3
- central mechanism arrives by point 6
- no important loop lacks a payoff
- energy changes across the clock rather than staying flat or maxed
- no long stretch contains only abstract explanation
- speech and visuals do not peak in complexity at the same time
- result frames remain visible long enough to inspect
- pauses are intentional, not empty
- every visual or audio refresh has a viewer-state purpose
