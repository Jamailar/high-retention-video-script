# Mature Creator Production System

Use this reference to turn the selected concept into an executable shoot and edit. The process may be complex internally, but the creator should receive one coherent script package.

## Source-Informed Principles

- YouTube's official guidance separates appeal, engagement, and satisfaction; it treats ideation, title/thumbnail packaging, an expectation-matching intro, storytelling, and retention analytics as one system. Source: https://support.google.com/youtube/answer/16559650
- YouTube retention reporting distinguishes intros, top moments, spikes, and dips, and supports revising exact moments rather than applying generic “make it shorter” advice. Source: https://support.google.com/youtube/answer/9314415
- YouTube supports testing up to three titles, thumbnails, or combinations for eligible long-form videos and chooses on watch time. Source: https://support.google.com/youtube/answer/16391400
- TikTok Creative Codes recommends hook/body/close, early value, vertical safe framing, deliberate sound, and attention devices such as movement, text, transitions, and scene changes. Source: https://ads.tiktok.com/business/library/Creative_Codes_One_Pager.pdf
- Open creator skills add useful operating discipline: research before packaging, multiple options and selection, voice profiles, reference-video teardown, read-aloud QA, beat timing, explicit assets, and performance-based revision. Sources: https://github.com/kenneth-liao/ai-launchpad-marketplace/tree/main/creator-stack/skills, https://github.com/charlie947/social-media-skills, https://github.com/blacktwist/social-media-skills
- Open product-video and talking-head skills reinforce one-message selection, format/trust matching, exact beat sums, one-breath lines, and production-ready shot specifications. Source: https://github.com/sanky369/vibe-building-skills/tree/main/skills/creative

Treat these as decision standards, not promises that a pattern guarantees performance.

## End-To-End Operating Order

### 1. Intake And Evidence

- Receive unstructured user materials.
- Search accessible files, knowledge, product surfaces, transcripts, references, and creator history.
- Build audience, creator voice, proof, asset, constraint, and performance evidence packs.
- Separate facts, inferences, assumptions, missing context, and unsupported claims.

### 2. Brief And Classification

- Primary viewer and viewing moment
- Product type and conversion job
- Trust mode and delivery format
- Platform, runtime, aspect ratio, sound/caption needs
- One completion promise
- Proof threshold and production constraints

### 3. Angle Lab

- Generate 3-7 distinct audience angles.
- Score evidence, relevance, visual engine, novelty, emotion, platform fit, risk, and feasibility.
- Select one primary direction and one backup.

### 4. Package Lab

- Write at least 12 rough titles across multiple families.
- Build three title + thumbnail/first-frame + hook + payoff finalists.
- Score the complete package and select one primary plus two test variants.
- Verify title, visual, hook, and script promise form one contract.

### 5. Story Design

- Choose a narrative architecture.
- Define one lesson and 3-5 main sections.
- Build the viewer-state spine and question-payoff ledger.
- Place proof close to claims and progressive rewards across the story.

### 6. HKRR And Clock Design

- Plan Happiness, Knowledge, Resonance, and Rhythm before full dialogue.
- Map 12 proportional marks with strong 12/3/6/9 stimuli.
- Assign viewer question, exit risk, state change, payoff, energy, proof, and audiovisual behavior to every mark.

### 7. Spoken And Audiovisual Script

- Draft beats first.
- Write complete natural spoken lines second.
- Attach A-roll, B-roll, screens, artifacts, captions, sound, and edit behavior third.
- Preserve creator voice and remove generic AI phrasing.

### 8. Read-Through And Timing

- Estimate language duration.
- Time a real read when possible.
- Add pauses, reactions, gestures, UI latency, result holds, and edit handles.
- Cut repetition before increasing delivery speed.
- Reconcile line timing with exact edit ranges.

### 9. Capture Engineering

Create one authoritative capture checklist. Every row includes:

- stable shot ID
- A-roll, B-roll/screen, B-roll/live, audio, or existing asset type
- exact content or complete spoken line
- source or location
- start state, action, and end state
- framing or screen region
- target usable duration and minimum takes
- deterministic filename
- privacy, rights, and masking requirement
- priority and observable acceptance criterion

Order the table for efficient shooting, not edit chronology, when batching cameras, locations, people, app states, or props saves work.

### 10. Edit Engineering

Create one authoritative edit timeline. Every row includes:

- exact time and clock mark
- viewer job and HKRR role
- A-roll IDs with intended in/out use
- B-roll IDs with intended in/out use
- complete voiceover, dialogue, sync sound, music, pause, or silence
- exact on-screen text
- cut, crop, zoom, speed, transition, comparison, caption, and sound action
- observable acceptance criterion

Do not create separate AV, beat, and edit tables that the editor must reconcile.

### 11. Audio-First Assembly

For presenter, voiceover, interview, or dialogue-led work:

1. capture or place clean primary audio
2. remove false starts, repeated meaning, and accidental dead gaps
3. preserve intentional breath and reaction timing
4. fit A-roll and B-roll to the meaning of the audio
5. add music, sound effects, transitions, and motion after intelligibility works
6. generate captions with an existing ASR tool and correct them against the final audio

For visual-first product reveals or motion pieces, the beat and sound design may lead, but timing still needs exact arithmetic and inspectable result holds.

### 12. Test Capture Or Test Cut

Run a short test when any of these is uncertain:

- speaker pacing or tone
- screen latency, loading, or cursor clarity
- phone readability or subtitle safe area
- generated visual consistency
- product result visibility
- audio quality, room noise, or dialogue handoff
- whether a cardinal stimulus actually feels stronger than neighboring marks

Test the riskiest 15-30 seconds first. Do not record the entire production to discover that the core proof is unreadable.

### 13. Red-Team, Deliver, And Learn

- Run package, audience, HKRR, timing, proof, production, privacy, and platform checks.
- Revise deficiencies before handoff.
- Deliver one HTML package and optional capture CSV. Let the HTML generate the simplified shooting PNG locally on demand so it always reflects the approved script and current capture progress.
- After publishing, map available performance data back to the planned package, viewer journey, HKRR marks, and edit timestamps.

## Internal Working Structures Versus User-Facing Output

The workflow may use internal notes or temporary tables for:

- source ledger
- angle candidates
- 12 rough titles
- package score calculations
- story spine
- question-payoff ledger
- speech timing measurements
- shot-ID validation

Do not expose each as a separate file. Summarize the approved decisions inside the final HTML. The user-facing source of truth remains:

1. `video-script-package.html`
2. optional `capture-list.csv`

## Tooling Boundary

Use mature existing tools for deterministic media work:

| Need | Use existing capability | Do not self-build |
| --- | --- | --- |
| Media probe, transcode, concat, frame/audio extraction | `ffmpeg` / `ffprobe` or the repo's existing media wrapper | A new codec or transcoder |
| Speech-to-text and caption timing | Existing transcription tool or a proven Whisper implementation | Ad-hoc timing from guessed text length only |
| Programmatic video rendering | Remotion and its established composition/timing APIs when code-rendered video is requested | A custom rendering engine |
| NLE editing | Existing editor or project format chosen by the creator | A new editor inside this skill |
| Reference-video acquisition | Platform-compliant existing downloader/API when authorized | Scraping logic invented inside the script workflow |
| Browser/app recording | Existing screen recorder and automation only when needed | Simulated proof that does not reflect the real product |

Self-designed work belongs in audience insight, angle selection, package decisions, story architecture, HKRR, clock design, spoken copy, and production direction. The script skill orchestrates these decisions; it does not become a media-processing framework.

## Production Readiness Standard

A package is ready only when:

- the shooter can capture every must-have row without clarification
- the speaker can perform every line naturally within its range
- the editor can build the timeline using exact source IDs and instructions
- every important claim has visible or audible proof
- the title/visual/hook promise is progressively and fully paid
- all 12 clock marks have meaningful stimulus jobs
- 12/3/6/9 are structurally stronger than neighboring marks
- every HKRR element scores at least 3/5
- privacy, rights, safety, and compliance risks are explicit
- the final CTA is proportionate to trust earned and executable now

If any required source, result, speaker, permission, product state, or proof is unavailable, mark the package blocked or reduce the claim. Do not bury the problem in an “editor note.”
