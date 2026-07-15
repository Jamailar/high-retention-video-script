# Context Intake And Source Use

Use this reference before writing a production script. Video background rarely arrives as a clean brief. Treat the user's raw materials as the input, then organize them.

## Context Intake Principle

Do not force the user to fill a rigid form. Ask for an unstructured material dump when context is thin:

```text
把你认为可能有用的背景材料一次性发来，不用整理。
可以包括：产品介绍、文件路径、知识库关键词、对标视频链接、已有脚本、评论区、截图、录屏、用户画像、账号定位、禁忌、想表达但还没想清楚的点。
我会先整理这些材料，再决定脚本结构。
```

Ask this as one broad question. Avoid interrogating the user with many narrow questions unless a specific missing item blocks the script.

## Context Sources

Use any available source, in this order:

1. Current conversation and user-provided raw dump.
2. Attached or local files, paths, docs, screenshots, transcripts, CSVs, PDFs, decks.
3. Workspace/repo documentation when the product is in the current workspace.
4. Available knowledge-base clues, memory, database, or search tools if the user points to them or the environment exposes them.
5. Reference videos or competitor materials supplied by the user.
6. The creator's own published work, performance exports, retention graphs, comments, and prior package variants when the user provides or authorizes access.
7. Public research only when the user asks for it, sources are needed, or current facts matter.

When using files or knowledge-base material, record the path, title, query, or URL in the source ledger.

## Intake Modes

### Material Dump Mode

Use when the user has not provided enough background.

Output:

- one broad request for raw materials
- examples of useful material types
- reassurance that the user does not need to organize them
- optional fallback: "If you want me to proceed now, I will mark assumptions explicitly."

### Source Discovery Mode

Use when the user says the background is in files, a knowledge base, a repo, a folder, a transcript, or a prior artifact.

Actions:

- Search obvious local paths or provided directories.
- Read source documents before scripting.
- Extract product facts, claims, proof, constraints, assets, and reference patterns.
- Ask only if access is impossible or the source location is unknown.

### Synthesis Mode

Use after receiving or finding context.

Create:

1. Source ledger.
2. Context report.
3. Evidence inventory.
4. Audience evidence pack.
5. Creator voice pack.
6. Performance evidence pack when history exists.
7. Script-relevant takeaways.
8. Missing context and assumption list.

Only then draft or revise the script.

## Audience Evidence Pack

Do not infer the audience only from age, platform, or creator intent. Extract evidence that reveals the viewer's real viewing moment:

| field | what to extract |
| --- | --- |
| situation | What is happening immediately before they encounter the video? |
| exact_language | Their own words from comments, reviews, search queries, transcripts, tickets, or user notes |
| current_workaround | What they do today and why it is unsatisfying |
| desired_outcome | The observable result they want, not a vague aspiration |
| objection | What makes them doubt the claim, product, creator, effort, price, or fit |
| cost_of_inaction | What continues to waste time, money, confidence, or opportunity |
| identity_cue | The phrase or behavior that makes them recognize themselves |
| proof_threshold | What they need to see before they will believe or act |

If direct audience language is unavailable, mark the inferred language as an assumption. Do not present invented pain phrases as user research.

Convert the evidence pack into one `viewer_moment` sentence:

```text
当[具体处境]发生时，这位观众正在用[现有办法]试图得到[可观察结果]，但担心[主要异议]；本片必须用[证据门槛]让他相信并完成[下一步动作]。
```

## Creator Voice Pack

Video scripts must sound like the creator, not like generic high-conversion copy. When source material exists, analyze 3-5 representative samples from transcripts, captions, previous scripts, long-form writing, voice notes, or published videos.

| field | what to extract |
| --- | --- |
| speaking_position | Peer, practitioner, founder, teacher, reviewer, entertainer, expert, customer |
| sentence_rhythm | Typical length, short/long alternation, pauses, fragments, paragraph cadence |
| perspective | Balance of first-person experience, second-person instruction, and third-person evidence |
| vocabulary | Repeated phrases, technical level, preferred concrete terms |
| emotional_range | Warmth, directness, humor, restraint, vulnerability, intensity |
| transition_habits | How the creator moves between story, proof, explanation, and action |
| evidence_habits | Personal result, demonstration, data, analogy, case, authority, customer language |
| anti_patterns | Words, tones, structures, claims, or creator personas that feel false |

Preserve exact user-owned language when appropriate. Do not copy another creator's distinctive phrasing or manufacture verbal quirks from one sample. When no voice sample exists, mark voice as an assumption and use restrained, direct, conversational language.

Do not stop at surface tone. Extract a `creator_truth_pack` only to the extent required by the selected architecture:

| field | what to extract |
| --- | --- |
| viewer_job_or_trigger | The task/result the viewer needs, or the real event/conflict when a narrative architecture requires one |
| credibility_or_stake | What makes the creator/tool credible; personal stake is optional for a direct utility tutorial |
| belief | A judgment the creator actually holds and could defend |
| failed_attempt | A real failed or unsatisfying attempt only when it improves the selected architecture; never manufacture or force one |
| concrete_detail | An object, screen, line, number, action, or moment only this material provides |
| limit_or_uncertainty | What the creator does not know, cannot promise, or still needs from the audience |

A polished creator-led opinion, story, or presenter script should use sourced fingerprints from the voice and truth packs. A direct screen-led tutorial may rely on clear product language and real operation without inserting autobiography. When voice evidence is necessary but missing, invite a natural answer rather than a formal brief:

```text
像跟朋友讲一样说说：你会怎么直接向朋友介绍这个结果或方法？哪些词你平时绝对不会用？如果这条片子确实需要个人经历，再补充为什么想拍、哪一刻最关键，以及手里哪段画面能证明。
```

If the user chooses not to provide more, continue only with a clearly labeled provisional voice draft. Never invent the creator's history to satisfy the structure.

## Performance Evidence Pack

When the creator has published comparable work, use their own baseline before generic advice.

Capture only metrics actually available:

| field | use |
| --- | --- |
| package | Title, thumbnail/cover, first frame, hook |
| audience_context | Platform, follower state, traffic source, publication timing |
| appeal | Impressions, view choice, click-through, swipe-away when available |
| retention | First 3/6/30 seconds, average duration, completion, graph shape |
| moment_signals | Spikes, dips, replays, shares, saves, comments, exits |
| conversion | Follows, clicks, sign-ups, purchases, comments, downloads, or task completion |
| content_features | Angle, story type, proof type, HKRR pattern, runtime, delivery style |

Compare like with like: similar platform, placement, runtime, audience, and video job. A result from one video is a clue, not a law. Record sample size, recency, and confidence.

Create a compact creator learning profile:

```yaml
creator_baseline:
  comparable_videos:
  date_range:
observed_strengths:
  - evidence-backed pattern
observed_weaknesses:
  - evidence-backed pattern
untested_hypotheses:
  - testable idea
confidence: high | medium | low
```

## Source Ledger Format

| source_id | type | source | status | usable_for | risk |
| --- | --- | --- | --- | --- | --- |
| S1 | file/url/chat/knowledge/video | path, URL, note, or query | used/partial/missing | hook/proof/audience/CTA/visuals | privacy/copyright/stale/unknown |

## Context Report Format

```yaml
context_status: sufficient | partial | weak
used_context:
  - source-backed fact or material
missing_context:
  - item that would improve customization
assumptions:
  - assumption used only because source is missing
do_not_claim:
  - claims unsupported by current context
script_implications:
  - how context changes hook, proof, structure, visuals, or CTA
creator_voice:
  - evidence-backed language or delivery rule
performance_implications:
  - creator-specific pattern or hypothesis
```

## Evidence Inventory Format

| claim_or_script_need | available_evidence | proof_level | gap | action |
| --- | --- | --- | --- | --- |
| Product can produce final artifact | screen recording / artifact / demo | strong/medium/weak | missing final output screenshot | capture before production |

Proof levels:

- Strong: real artifact, screen recording, before/after, user result, data with context.
- Medium: process screenshot, product doc, credible example, structured transcript.
- Weak: founder claim, generic category claim, unsourced memory, vague user assertion.

If evidence is weak, reduce the claim or add a capture/source requirement.

## Reference Video Teardown

When the user provides reference videos, do not copy surface style blindly. Extract:

| field | question |
| --- | --- |
| package | What did title/cover/first frame promise? |
| first_6_seconds | What conflict, proof, reversal, or curiosity appears? |
| viewer_contract | How did the hook confirm and extend the package without repeating it? |
| story_architecture | What question, story engine, or proof progression carried the video? |
| question_payoff | Which questions were opened, partially paid, and fully closed? |
| stimulus_clock | What happens at 12/1/2/3/4/5/6/7/8/9/10/11/finish? Which marks are big vs small? |
| stimulus_pattern | How do the big and small stimulus points alternate across the clock? |
| micro_pacing | Speech rate, sentence rhythm, pauses, result holds, information density, cut and sound timing |
| energy_curve | Where does intensity rise, release, or become deliberately still? |
| proof_strategy | What evidence makes claims believable? |
| visual_language | Screen recording, face cam, B-roll, captions, motion, sound |
| voice | What is structural and adaptable versus distinctive phrasing that must not be copied? |
| borrow | What can be adapted ethically? |
| avoid | What is irrelevant, misleading, off-brand, or too expensive? |

## Missing Context Policy

Do not block on every missing detail. Classify gaps:

- Blocking: product facts, target audience, core offer, legal/privacy limits, unavailable files required for claims.
- Important: reference videos, exact UI wording, final artifact screenshots, real user comments.
- Nice-to-have: music style, font preference, secondary CTA, optional B-roll.

If blocking gaps exist, ask for them before scripting. If only important or nice-to-have gaps exist, proceed with explicit assumptions and a capture list.

## Anti-Generic Rules

- Do not write a script from only the product category if product-specific sources are available.
- Do not invent testimonials, metrics, UI labels, customer results, or competitor claims.
- Do not turn every source into a script beat. Select sources that support the single promise.
- Do not let reference videos override the user's product truth.
- Do not treat another creator's surface wording, personality, edit style, or audience relationship as a transferable formula.
- Do not generalize a winning pattern from one published video without labeling it a hypothesis.
- Do not ignore the creator's own language and performance history when those sources are available.
- Do not hide uncertainty. Mark assumptions and source gaps clearly.
