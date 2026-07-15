# Output Specs And QC

Use this reference when turning approved creative decisions into the final package. The internal process may be complex; the user-facing result must be easy to read, approve, shoot, and edit.

## User-Visible File Policy

Default output:

- one self-contained HTML: `video-script-package.html`
- optional CSV only when a second operator explicitly needs sortable capture data

Do not output separate strategy, source, title, beat, clock, AV, capture, edit, and score documents. Raw research, discarded alternatives, and detailed reasoning remain internal or in one collapsed source appendix.

## Information Hierarchy

The creator should be able to answer these questions in order:

1. What video am I making?
2. What exactly do I say, show, and cut at each time?
3. How are HKRR and the stimulus clock shaping the viewing experience?
4. Which assets do I need to capture?
5. What must be fixed before shooting?

If the HTML answers a strategy question but makes any action harder to find, simplify it.

## HTML Contract

Use `assets/video-script-package-template.html`. Keep all CSS, JavaScript, icons, and fonts local or system-provided. The document must remain readable without JavaScript; interactions only enhance progress and export.

### 1. Summary

Show:

- selected title
- one-sentence premise or completion promise
- runtime and platform
- context status and voice status
- HKRR total
- capture and edit progress
- one compact decision strip: core result or point, video job, viewer tension, proof engine

Do not show title ideation worksheets or long strategy prose.

### 2. Word-For-Word AV Script

This is the primary and only expanded script/edit table. Use no more than five visible columns:

| Column | Required content |
| --- | --- |
| `done` | Persistent local edit checkbox |
| `time_and_clock` | Exact in/out, clock mark, stimulus size, dominant HKRR role |
| `spoken_line` | Complete, speakable line, dialogue, silence, or sync-audio instruction |
| `picture` | A-roll and B-roll shot IDs plus the exact visible action or state |
| `edit_cue` | Concise cut, hold, sound, text, crop, speed, or transition instruction |

Rules:

- Put the complete spoken text in the table. Never replace it with a summary.
- Keep each row to one performance or editorial beat; do not force one row per clock point.
- Clock points may span one or several rows.
- A-roll/B-roll IDs must resolve to the capture checklist.
- On-screen text must be short and should not duplicate full subtitles.
- The row must be understandable without consulting a separate viewer-journey or edit table.

### 3. HKRR And Rhythm

Show four compact HKRR cards. Each card contains only:

- intended viewer effect
- exact execution or timestamp evidence
- score from 0-5

For Rhythm, name both the 12-point distribution and the important micro-pacing behavior.

Show one mandatory circular 12-point clock:

- `12/3/6/9` use stronger coral markers
- the other eight points use smaller neutral markers
- Finish stays in the center
- every point displays mark, exact trigger time or time range, HKRR role, and a compact stimulus/payoff phrase around the circumference
- do not add a duplicate clock-point list or table below it
- a point may be a spoken idea, visual proof, reaction, silence, sound change, or transition

Show one proportional A-roll/B-roll timeline directly before or after the clock. It is a visual overview, not a second edit table.

### 4. Capture Checklist

Use no more than five visible columns:

| Column | Required content |
| --- | --- |
| `done` | Persistent local capture checkbox |
| `id_type_priority` | Stable ID, A-roll/B-roll/audio/existing asset, must/should/optional |
| `capture` | What must visibly or audibly happen |
| `direction` | Start state -> action -> end state, framing/region, target duration/takes |
| `output` | Deterministic filename, privacy/rights note, observable acceptance criterion |

Do not split each attribute into its own column. Keep the instructions concrete enough that another person can capture the asset without interpreting the script.

### 5. Final QC

Keep the visible audit compact. Show:

- voice status and creator fingerprints used
- first exact drop-off risk and whether it was repaired
- strongest remaining generic or AI-pattern risk, or `none`
- H/K/R/Rhythm scores with one evidence phrase each
- proof or production blockers
- one highest-priority revision before shooting

Do not show a 35-row checklist. Internal checks still apply, but only the decision-changing result belongs in the HTML.

## Interactions

Keep only interactions that reduce production effort:

- persistent local completion state
- capture and edit progress
- unfinished-only filtering
- print / PDF
- reset progress with confirmation
- generate a simplified shooting PNG locally with Canvas
- preview and save the PNG; keep the preview long-pressable on mobile

Do not add tabs, carousels, focus modes, synchronized selectors, score filters, decorative animation, or editing controls.

## Shooting PNG

The PNG is a field sheet, not a screenshot. Generate it from approved HTML data and include:

- selected title, premise, runtime, platform, and capture progress
- compact H/K/R/Rhythm execution guidance
- circular clock with all point labels around the circumference
- every capture row and completion state
- embedded Beav icon and name

No network requests or external rendering libraries.

## Internal Decision Records

Keep these in working memory or temporary files unless requested:

- raw source ledger
- angle candidates and rejection reasons
- twelve rough titles and package alternatives
- question-payoff ledger
- viewer-state journey table
- line-by-line AI-pattern audit
- full validation checklist

The final HTML may include one collapsed source/context appendix with used sources, missing context, assumptions, and unsupported claims to avoid.

## Voice And Content Hard Gates

Do not mark the script production-ready when:

- no real core result, point, or viewer task can be stated in one sentence
- the selected architecture conflicts with the viewer job, especially when a utility tutorial delays its result for setup, biography, pain, or reversal
- the content is primarily a feature or framework list
- creator-led copy lacks creator evidence and is not labeled provisional
- any personal event, opinion, or result was invented
- the hook cannot identify topic, reason to stay, and credibility without the cover
- a full paragraph could fit an unrelated product unchanged
- an unresolved high-risk drop-off point remains
- a 20-30 second stretch contains only abstract explanation

## HKRR Score

Score each element from 0-5:

| Score | Meaning |
| ---: | --- |
| 0 | absent |
| 1 | named but not designed |
| 2 | present as a token moment |
| 3 | usable and supported by at least one real beat |
| 4 | strong, repeated with variation, and integrated with the selected proof/content engine |
| 5 | shapes the full viewing experience without feeling imposed |

For each element record exact timestamp evidence, remaining deficiency, and one revision action. `Rhythm` cannot score above 2 without a complete 12-point distribution and meaningful micro pacing.

Hard gate: revise when any element is below 3 or the total is below 15/20.

## Cold-Viewer QC

Answer these questions before delivery:

| Area | Pass condition |
| --- | --- |
| Package | Title, first frame, hook, and payoff promise the same video |
| Opening | Topic, reason to continue, and credibility/proof are identifiable cold |
| Core | One useful result, point, or task survives after deleting every feature name |
| Architecture | Progression matches the viewer job; a utility tutorial shows the result before explanation and avoids decorative drama |
| Creator | Creator-led opinion/story copy uses sourced fingerprints; a direct screen-led tutorial does not invent autobiography |
| Speech | Lines fit the creator's mouth and timed range |
| Proof | Strong claims have adjacent visible evidence |
| Density | Repeated meaning and unnecessary background are removed |
| Variation | Sentence shapes, emotional energy, and HKRR roles do not become uniform |
| Clock | All 12 points exist; 12/3/6/9 create larger state changes |
| Production | Every shot ID resolves; each capture has an acceptance condition |
| Action | The ending closes the promise and gives one proportionate next step |

## AI-Pattern QC

Use `human-voice-and-editorial-audit.md`. At minimum, inspect:

- repeated sequencing language
- repeated “not X but Y” reversals
- fake viewer questions and self-answers
- uniform sentence openings, lengths, and paragraph conclusions
- generic feature-tour paragraphs
- abstract labels without concrete actions
- over-complete objection handling
- an emotion curve with no pause, doubt, reaction, or release
- invented anecdotes or audience language

Patterns are evidence, not automatic failures. Preserve them when supported by the creator's real voice and the local passage works aloud.

## Timing And Source Validation

- Actual read-through timing overrides estimates.
- Include pauses, UI latency, result holds, and 10-15% edit handles.
- The last script row must end at the declared runtime.
- Clock points must progress in order and cover the runtime. Use exact trigger timestamps when points mark stimulus changes; use ranges only when a beat genuinely occupies the interval.
- Every A/B-roll ID in the script must exist exactly once in the capture list.
- Every must-have capture must appear at least once in the script or be explicitly justified as setup/audio.
- Missing proof is a blocker or a reduced claim, never an implied edit fix.

## Revision Priority

Fix in this order:

1. empty or competing core point
2. architecture mismatch or delayed viewer value
3. absent real evidence, creator truth when relevant, or invented specificity
4. weak content/proof engine
5. package-content mismatch
6. logic gap or unpaid question
7. generic, repetitive, or unspeakable lines
8. weak HKRR rotation or clock distribution
9. timing and production ambiguity
10. surface wording and polish

Do not spend time polishing a sentence that belongs to a section the viewer does not need.
