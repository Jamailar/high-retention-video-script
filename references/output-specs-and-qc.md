# Output Specs And QC

Use this reference when turning approved creative decisions into the final package. The internal process may be complex; the user-facing result must be easy to read, approve, shoot, and edit.

## User-Visible File Policy

Default output:

- one self-contained HTML: `video-script-package.html`
- optional CSV only when a second operator explicitly needs sortable capture data

Do not output separate strategy, source, title, beat, clock, AV, capture, edit, and score documents. Raw research, discarded alternatives, and detailed reasoning remain internal or in one collapsed source appendix.

## Information Hierarchy

The creator should be able to answer these questions in order:

1. What video am I making, and what must I fix before shooting?
2. What exactly do I say, and what does the viewer see, at each time?
3. What do I shoot at each camera position, and when is a shot good enough?
4. How are HKRR and the stimulus clock shaping the viewing experience?

If the HTML answers a strategy question but makes any action harder to find, simplify it.

## HTML Contract

Use `assets/video-script-package-template.html`. It is data-driven: copy the file and replace **only** the JSON inside `<script type="application/json" id="video-script-data">`. Everything the creator sees (header, opening 3 seconds, script, capture cards, HKRR, clock, A/B track, QC, teleprompter, field-sheet PNG) is rendered from that one object, so the same fact is never written twice and cannot drift.

Remove `"example": true` from the copied JSON. Never write the two characters `</` inside the JSON; write `<\/` instead. Keep all CSS, JavaScript, fonts, and the embedded Beav icon local.

The page follows the creator's real sequence, one view at a time:

1. **逐字稿 (read and edit)**: the opening-3-seconds card, then every beat with its spoken line first and picture/text/edit cue under it. A teleprompter reads the same lines full-screen.
2. **拍摄 (shoot)**: capture cards grouped as "A-roll by camera position" and "B-roll / screen / assets". An A-roll card lists every line recorded at that position, so the creator can shoot all of them in one sitting. Each B-roll card shows where it is used.
3. **节奏 (rhythm)**: the core decision, four HKRR cards, the 12-point clock, the proportional A/B track, the pre-shoot QC, and a collapsed sources appendix.

### Data Object

```json
{
  "id": "stable-package-id",
  "title": "selected title",
  "promise": "one-sentence premise or completion promise",
  "runtimeSeconds": 72,
  "platform": "抖音 · 竖屏 9:16",
  "voice": { "status": "verified | provisional", "label": "已按你的口吻 / 待你读一遍", "note": "fingerprints used, or what is still unverified" },
  "core": { "point": "one core result or point", "tension": "viewer tension", "proof": "proof engine" },
  "fixFirst": "the one revision to make before shooting (omit when none)",
  "script": [
    { "id": "S01", "start": 0, "end": 4, "clock": "12", "hkrr": "K+H",
      "line": "complete speakable line", "delivery": "optional short delivery note",
      "a": "A01", "b": ["B01"], "picture": "what the viewer sees",
      "text": "short on-screen text", "cue": "cut / hold / sound instruction" }
  ],
  "shots": [
    { "id": "A01", "type": "A | B | screen | audio | asset", "priority": "must | should | optional",
      "what": "what must visibly or audibly happen", "where": "location",
      "start": "start state", "action": "action", "end": "end state",
      "framing": "framing / height / distance / light", "takes": "takes or duration",
      "file": "deterministic filename", "accept": "observable acceptance criterion", "privacy": "rights or privacy note" }
  ],
  "hkrr": {
    "H": { "score": 4, "effect": "intended viewer effect", "evidence": "timestamped execution" },
    "K": { "score": 5, "effect": "", "evidence": "" },
    "R": { "score": 3, "effect": "", "evidence": "" },
    "Rh": { "score": 4, "effect": "12-point distribution plus micro pacing", "evidence": "" }
  },
  "clock": [ { "mark": "12", "time": "0:00", "role": "K+H", "label": "compact stimulus or payoff" } ],
  "finish": { "time": "1:12", "label": "how the promise is repaid and the action lands" },
  "qc": {
    "dropOff": { "time": "0:15", "risk": "first exact drop-off risk and whether it was repaired" },
    "aiPattern": "strongest remaining generic or AI-pattern risk, or 无",
    "blockers": "proof or production blockers",
    "verdict": "one-line HKRR verdict"
  },
  "sources": { "used": "", "missing": "", "assumptions": "", "doNotClaim": "" }
}
```

Rules:

- `script` is the single source of truth for words and edit order. Put the complete spoken text in `line`; never summarize it. One row is one performance or editorial beat; rows are continuous (`start` equals the previous `end`) and the last `end` equals `runtimeSeconds`.
- Give `clock` on the row where that clock point fires. A point may be a look, pause, proof reveal, sound change, or cut; it does not need a new sentence.
- `a` is the A-roll shot recording the voice for that row; `b` lists the shots covering it. Every ID must exist exactly once in `shots`. A must-have shot that no row uses must be `audio` or `asset`.
- `clock` has exactly 12 items in order 12, 1, … 11. `12/3/6/9` are drawn as big stimuli. `finish` sits in the center.
- `text` is short on-screen text (two lines of about 8–10 Chinese characters at most), never a full subtitle.
- Omit empty fields rather than writing `—`.
- The page validates itself: placeholders left behind, missing shot IDs, discontinuous times, runtime mismatch, unused must-shots, duplicate IDs, and a clock without 12 points appear in a red "数据检查" note and in `window.videoScriptCheck`. Open the file (or run it headless) and deliver only when that list is empty.

## Interactions

Keep only interactions that reduce production effort; the template already has them:

- three-view switch (逐字稿 / 拍摄 / 节奏), remembered per package
- teleprompter: full-screen lines, auto-scroll with speed control, mirror mode, tap or space to pause
- persistent capture and edit checks, capture progress with remaining must-shots, "只看没拍的", reset with confirmation
- tapping a shot ID in the script jumps to its capture card
- field-sheet PNG generated locally with Canvas; long-press to save on mobile
- print / PDF prints all three views in order

Do not add more tabs, carousels, editing controls, score filters, or decorative animation. Light and dark follow the system.

## Shooting PNG

The field sheet is generated from the same data, not a screenshot. It contains the title, platform, runtime, capture progress, HKRR total, the opening-3-seconds line, the 12 clock points, and every capture card with its done state, start → action → end, framing, takes, and filename.

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
