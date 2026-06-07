# Combo Recommendation Engine

Use this reference after the brief is sufficiently understood and before drafting final content.

The goal is to recommend the best strategic combinations for the user's product, customer, goal, platform, campaign context, and available proof.

Each combo should combine:

```txt
Marketing goal
Customer / JTBD
Customer journey stage
Experience layer
Platform / channel
Content angle
Content framework
Persuasion psychology
Irrational buying motivation
Trust/proof signal
Offer / CTA
Compliance risk
Success metric
```

## When To Use

Use for:

```txt
- Any brief that asks for ads, landing pages, social posts, content calendar, campaign strategy, channel strategy, roadmap, or conversion copy.
- Any request where multiple strategic directions are possible.
- Any guided-mode request after intake, before final writing.
- Any `bhd auto` request internally, selecting the best combo automatically.
```

Do not use when the user asks only for a tiny wording edit, translation, or grammar fix.

## Combo Count

Guided mode:

```txt
Return 2-4 combos.
Recommend one primary combo.
Ask the user to choose A/B/C/D or allow custom adjustment.
```

`bhd auto` mode:

```txt
Score 2-4 possible combos internally.
Select the highest-scoring combo.
Show the selected combo in the strategic header.
Do not ask the user to choose.
```

## Fit Score

Score each combo out of 100.

```txt
Goal fit: 0-15
Audience/JTBD fit: 0-15
Journey fit: 0-15
Experience layer fit: 0-10
Platform/channel fit: 0-10
Framework fit: 0-10
Persuasion fit: 0-10
Proof/trust fit: 0-10
Compliance safety: 0-5
```

Interpretation:

```txt
90-100: Very strong fit. Use as primary unless user has a different preference.
80-89: Strong fit. Good candidate, may need proof or offer refinement.
70-79: Usable fit. Needs more data, sharper angle, or lower-risk claims.
Below 70: Do not recommend unless user specifically asks for that direction.
```

## Scoring Rules

Goal fit:

```txt
High score if the combo's framework, CTA, and channel match the user's objective.
Example: lead generation + Facebook Ads + PAS/4P + audit CTA scores high.
Example: brand awareness + hard-sell urgency CTA scores low.
```

Audience/JTBD fit:

```txt
High score if the angle reflects the customer's functional, emotional, personal, or social job.
Low score if the angle is generic or not tied to the customer's real job.
```

Journey fit:

```txt
Unaware: education, symptom, mistake, story, myth-bust.
Problem aware: diagnosis, cost of inaction, PAS, mistake-fix.
Solution aware: mechanism, comparison, criteria, FAB, FAQ.
Product aware: proof, demo, case study, objection, PASTOR/BAB.
Most aware: offer, urgency, risk reversal, 4P/AIDA/SLAP.
Purchased: onboarding, activation, checklist.
Retention: advanced value, referral, testimonial, upsell.
```

Experience layer fit:

```txt
Awareness: clear positioning, simple category explanation, memorable hook.
Education: frameworks, how-to, diagnosis, explanation.
Trust: proof, process, testimonial, demo, case study.
Consideration: comparison, criteria, FAQ, objection handling.
Conversion: offer, CTA, risk reducer, urgency if true.
Onboarding: next steps, expectation setting, checklist.
Result: progress, quick win, measurement.
Loyalty: community, referral, advanced use, retention.
```

Platform/channel fit:

```txt
Facebook Ads:
Works well for pain, problem clarity, proof, offer, lead magnets, retargeting, click-to-message.

TikTok:
Works well for short hooks, visual demo, story, trend, founder POV, contrast, entertainment-led education.

Landing page:
Works well for mechanism, proof, offer stack, FAQ, detailed objection handling.

Personal brand/social:
Works well for POV, story, lesson, contrarian view, trust building, founder experience.

Email:
Works well for nurturing, proof, objection handling, launch sequence, retention.
```

Framework fit:

```txt
PAS: pain-driven, problem aware, ads/sales posts.
4P: conversion, offer, proof, direct response.
AIDA: general ads/landing pages with clear CTA.
BAB: transformation, case study, before-after.
PASTOR: long-form sales page or deep conversion.
ACCA: education and belief building.
FAQ Selling: product aware and objection-heavy.
Hook-Value-CTA: quick social posts.
Star-Story-Solution: personal brand and video storytelling.
Myth-Bust-Truth: thought leadership and unaware/problem aware.
```

Persuasion fit:

```txt
Loss Aversion: pain, wasted money, missed opportunity, risk of inaction.
Social Proof: trust gap, popular choice, testimonials, case studies.
Authority Bias: expert-driven or high-consideration purchase.
Scarcity/Urgency: only if deadline/slots/stock are real.
Anchoring/Contrast: price/value comparison, before-after, old-new.
Reciprocity: lead magnets, checklist, audit, free value.
Commitment/Consistency: quiz, checklist, diagnostic, small step.
Curiosity Gap: reach/awareness hooks.
Cognitive Ease: complex product that needs simple explanation.
Endowment Effect: demo, preview, trial, personalized audit.
Zeigarnik Effect: series content and nurture.
```

Irrational buying motivation fit:

```txt
Fear of waste: budgets, ads, time, data, operations.
Fear of falling behind: AI, competition, trends, market change.
Identity upgrade: professionals, founders, modern marketers.
Control desire: dashboards, tracking, decision confidence.
Simplicity bias: fewer tools, simpler workflow, less manual work.
Status signal: premium, professionalism, brand perception.
Belonging: community, category leaders, "people like us".
Future self: better workflow, calmer operations, predictable growth.
Certainty: clear process, guarantee, support, demo.
Convenience: automation, done-for-you, templates, shortcuts.
```

Proof/trust fit:

```txt
High score if proof exists and matches the claim.
Medium score if process/demo/checklist proof can support the claim.
Low score if the combo depends on testimonials, numbers, or authority the user does not have.
```

Compliance safety:

```txt
High score if the combo avoids unsupported superlatives, guaranteed outcomes, fake urgency, sensitive attributes, and restricted claims.
Low score if the combo requires risky claims, before-after promises, regulated products, or platform-sensitive targeting.
```

## Combo Output Contract

In guided mode, output:

```txt
Mình đề xuất các combo chiến lược sau:

Combo A: [name]
- Best for:
- Platform/channel:
- Goal:
- Journey stage:
- Experience layer:
- Marketing canvas focus:
- Angle:
- Framework:
- Psychology:
- Irrational buying motivation:
- Trust/proof:
- CTA:
- Main metric:
- Compliance risk:
- Fit score: /100
- Why this fits:

Combo B: ...
Combo C: ...

Khuyến nghị:
[which combo and why]

Bạn muốn chọn combo nào?
A. Combo A
B. Combo B
C. Combo C
D. Kết hợp [A+B/C]
E. Tôi muốn chỉnh hướng khác
Hoặc nhập lựa chọn tùy chỉnh.
```

In `bhd auto` mode, output only:

```txt
Selected combo:
Fit score:
Reason:
Risk/assumption:
```

Then proceed to final content.

## Default Combo Patterns

### Lead Generation For B2B Service

```txt
Goal: lead / booking
Journey: problem aware or solution aware
Experience: trust + conversion
Platform: Facebook Ads + landing page
Angle: cost of inaction / mechanism / proof
Framework: PAS or 4P
Psychology: Loss Aversion + Reciprocity
Irrational: Control desire or Fear of waste
Trust: process proof + audit/demo
CTA: receive audit / book consultation
Metric: CPL, booking rate, qualified lead rate
```

### TikTok Awareness For New Product

```txt
Goal: reach / education
Journey: unaware or problem aware
Experience: awareness + education
Platform: TikTok
Angle: symptom / mistake / contrast / trend
Framework: Hook-Value-CTA or Myth-Bust-Truth
Psychology: Curiosity Gap + Cognitive Ease
Irrational: Fear of falling behind or Simplicity bias
Trust: demo or visual proof
CTA: follow / comment keyword / watch next part
Metric: watch time, saves, profile visits
```

### Landing Page Conversion

```txt
Goal: conversion
Journey: product aware or most aware
Experience: trust + conversion
Platform: landing page
Angle: mechanism + proof + offer
Framework: PASTOR, AIDA, or QUEST
Psychology: Social Proof + Risk Reduction + Anchoring
Irrational: Certainty + Future self
Trust: case study, testimonial, demo, process
CTA: book / buy / start trial
Metric: conversion rate, booking rate, CAC
```

### Personal Brand Trust Building

```txt
Goal: trust / consideration
Journey: solution aware or product aware
Experience: trust
Platform: social post / LinkedIn / Facebook personal
Angle: founder POV / lesson / mistake / contrarian
Framework: Star-Story-Solution or Hook-Value-CTA
Psychology: Authority Bias + Mere Exposure
Irrational: Identity upgrade + Belonging
Trust: real story, process, customer learning
CTA: soft CTA / comment / DM
Metric: meaningful comments, saves, inbound leads
```

### Retargeting / Most Aware

```txt
Goal: conversion
Journey: most aware
Experience: conversion
Platform: Facebook retargeting / email
Angle: objection / offer / risk reversal
Framework: FAQ Selling, 4P, SLAP
Psychology: Urgency if true + Social Proof + Loss Aversion
Irrational: Certainty + Fear of waste
Trust: testimonial, FAQ, guarantee, demo
CTA: claim offer / book now / complete checkout
Metric: conversion rate, CPA, ROAS
```
