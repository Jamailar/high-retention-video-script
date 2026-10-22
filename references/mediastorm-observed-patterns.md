# MediaStorm-Observed Patterns

Use this reference when drafting, rewriting, or auditing a script that should hold attention the way strong long-form explainers do. It adds craft patterns observed in 影视飓风's published videos and public talks to the HKRR and clock workflow. It does not replace the gates in `SKILL.md`.

## Provenance

- **Public methodology:** HKRR and the clock theory as explained by 影视飓风 / Tim in public videos, interviews, and the `飓风世界` Douyin material. The public account of the clock theory says the team clock-mapped Bilibili videos above 10M plays and found strong moments spread evenly around the dial rather than clustered at the start.
- **Community transcript analyses (MIT):** `imfangli/mediastorm-copywriter` (structure observed across 19 recent 影视飓风 video transcripts) and `phaseddd/PhasedddSkill` (`tim-mediastorm`) (Tim-style elevation and pacing notes). We learned from their observations and rewrote everything here in our own words and for our own workflow.
- No official 影视飓风 script Skill was publicly available when this was written (checked 2026-10-22). This is not an official 影视飓风 project and implies no endorsement.

Treat every pattern below as a tool. Apply it only when it serves the selected viewer job and sounds like this creator. A utility tutorial still opens with the result.

## 1. Opening: Hook, Then Raise The Stakes

The first sentence carries the hook. The next 2-3 sentences explain why the topic matters beyond itself, then the video starts moving. Optionally preview the 2-3 questions the video will answer, but only if every question is paid off later.

Hook families that recur in the observed videos:

| Family | Shape | Example direction |
| --- | --- | --- |
| Object first | A specific thing on screen and one strange fact about it | 「这台灯只要 99 块，但它的显色比我工作室那盏还准。」 |
| Counter-intuitive question | A question whose obvious answer is wrong | 「为什么越贵的耳机，反而越容易被说难听？」 |
| Viewer situation | A moment the viewer has lived | 「你是不是也遇到过：照片拍完，回家一看全糊了。」 |
| Extreme scene | The most extreme version of the topic | 「零下 30 度，手机电量 3 分钟掉光。」 |
| Person first | One person's choice or result | 「他用一台旧手机，拍完了整部片子。」 |
| Series ritual | The recurring line or format of a series | Only for an established series with a real ritual |

Reject a stake-raising line that is a generic "this matters to everyone" claim. It must name a concrete consequence, group, or scale.

## 2. The Point Unit

Build each main point from the chain below. Not every link is required; never skip straight from claim to the next claim.

`phenomenon -> number -> everyday conversion -> analogy -> concrete example or demo`

- **Number:** one figure, with its source. Do not stack figures.
- **Everyday conversion:** turn the number into something the viewer can feel (「相当于每天少睡 40 分钟」).
- **Analogy:** one familiar comparison, and only when the mechanism is genuinely hard to see.
- **Example or demo:** the visible proof, which goes to the shot list.

## 3. Pacing Engines

- **Self-answered question:** roughly every 100-150 spoken characters, the narrator asks the question the viewer is about to have, then answers it at once with something concrete. This is different from a fake engagement question: the answer arrives in the same breath, and it moves the explanation forward.
- **Real turn:** every few points, a genuine 「但是」 that complicates what was just said (a limitation, a counter-case, a cost). Decorative reversals fail the drop-off audit.
- **Honest uncertainty:** saying 「这个我们也没测准」 or 「目前没有公开数据」 keeps trust and gives the viewer a reason to stay for the test. Never fake uncertainty for effect.
- **Density marker:** about one clear excitement point per ~500 spoken characters, matching the clock's even distribution. If a 500-character stretch has none, add proof, a turn, or a visual reset, not adjectives.

## 4. Long Video As A Chain Of Short Videos

For anything longer than about two minutes, design each section so it could stand alone: its own mini-hook, its own payoff, and a handoff line that opens the next question. Map the strongest section payoffs onto the 12/3/6/9 cardinal points. A section that only makes sense as setup for a later section is the first place viewers leave.

## 5. Sponsor And Commercial Segments

When the video contains a sponsor or the creator's own product, tie it to the question the video is already asking, place it after a payoff rather than before one, and keep the claim inside what the footage proves. A commercial segment that needs its own new topic is a drop-off point; mark it in `qc.dropOff`.

## 6. Optional Elevation (升华)

Use only when the creator actually holds the larger view and the content supports it. Four steps, each one sentence or two:

1. **Anchor:** the concrete thing the video just proved.
2. **Ask upward:** the larger question that thing points to.
3. **Bridge:** why this case answers part of the larger question.
4. **Land:** return to something concrete the viewer can do, see, or decide.

Skip it entirely for utility tutorials and product walkthroughs. An elevation that does not land back on a concrete action is an AI pattern.

## 7. Endings And Brand Voice

Observed 影视飓风 endings use a punchline after the elevation and a fixed series CTA. Those are their brand voice. Do not copy their phrases, catchphrases, or CTA wording. Use the creator's own recurring ending if one exists; otherwise end on the payoff and one specific action.

## 8. Format Variants

- **Review / comparison:** state the decision the viewer is making, show the test conditions, reveal results one dimension at a time, give a verdict per viewer type, then name what was not tested.
- **Vlog / experience:** a running device (a question, count, quiz, or challenge carried through the whole video) replaces the argument spine. Pay it off at the end.
- **Tutorial / tool:** result first (Gate 1). Use the point unit and self-answered questions inside steps; skip elevation.

## 9. Pre-Screen Before Publishing (点映)

When there is time, show the rough cut to 3-5 target viewers before release. Ask each to mark the moment they first lost interest and the moment they liked most, by timestamp. Fix the earliest common dip first; it usually matches `qc.dropOff`. Record what changed in the revision notes. This is a small-scale version of the internal screening and feedback process 影视飓风 has described publicly.

## Audit Checklist

Use during Gate 5 and Gate 7:

- Does the first sentence carry the hook, and do the next 2-3 sentences raise concrete stakes?
- Does each main point have at least number-or-proof plus one conversion, analogy, or demo?
- Are self-answered questions answered immediately and concretely?
- Is there at least one real turn, and is every turn true?
- Does any ~500-character stretch lack an excitement point?
- In a long video, can each section survive as a short clip?
- Is any phrase, CTA, or catchphrase borrowed from 影视飓风 rather than the creator?
