---
name: bhd-content-skill-pro
description: Vietnam-first content strategy and persuasion skill for creating customer-journey-aware content, sales copy, Facebook Ads, TikTok scripts, landing pages, personal brand posts, social calendars, video scripts, email copy, and repurposed content. Use when Codex is asked to plan, write, improve, audit, or systematize marketing content for the Vietnamese market, with English output supported when requested. Includes guided brief questions, customer journey mapping, experience layer mapping, conversion frameworks, trust/proof handling, Facebook/TikTok platform policy checks, Vietnam advertising-law checks, and compliance QA. Use "bhd auto" mode when the user asks the skill to process a supplied brief without follow-up questions. Use "/bhd-help" when the user wants usage instructions.
---

# BHD Content Skill Pro

## Core Rule

Build content from strategy, not from writing style alone. Before writing, determine the brief, audience, customer journey stage, experience layer, content goal, angle, framework, proof, objections, CTA, and compliance risk.

Default market is Vietnam and default language is modern Vietnamese. Write in English only when the user asks for English output or the brief clearly requires it.

## Operating Modes

### Help Mode

Use help mode when the user includes `/bhd-help`.

Return a concise Vietnamese usage guide instead of starting the brief wizard. Explain:

1. What the skill can create.
2. The difference between guided mode and `bhd auto`.
3. How to provide a brief.
4. Example prompts.
5. Compliance behavior for Facebook, TikTok, and Vietnam advertising law.

Use `assets/bhd-help.md` as the output contract. Do not ask brief questions in help mode unless the user also asks to start a specific task.

### Guided Mode

Use guided mode by default when the user invokes this skill without `bhd auto`.

Ask context-specific brief questions before producing final content. Do not use a fixed form. Ask only what is needed for the requested output.

Each question should include 4-5 suggested options and explicitly allow a custom answer. Keep each round to at most 5 questions. If answers remain insufficient, ask the next smallest useful set of questions.

After each user answer, decide whether the answer creates a new strategic gap. If it does, ask the next deeper question instead of rushing to draft. Good follow-up questions clarify audience specificity, JTBD, journey stage, proof, offer, platform, metric, compliance risk, or copy-ready format.

Use this pattern:

```txt
Câu hỏi 1: [question]
A. [option]
B. [option]
C. [option]
D. [option]
E. [option if useful]
Hoặc nhập câu trả lời tùy chỉnh.
```

If the user does not understand customer journey or experience layers, explain briefly and ask with options instead of expecting them to know the concept.

### bhd auto Mode

Use `bhd auto` mode when the user includes the phrase `bhd auto` in any casing or spacing that clearly means the command.

In `bhd auto` mode:

1. Do not ask follow-up questions.
2. Extract all available brief data.
3. Infer missing data conservatively.
4. Label assumptions clearly.
5. Select journey stage, experience layer, insight, angle, framework, psychology, proof type, objection handling, and CTA.
6. Produce the requested output.
7. Run final compliance and QA checks.

Only stop in `bhd auto` mode if the request is impossible, unsafe, or requires unavailable private proof, private customer data, legal permission, or platform-specific claims the user has not supplied.

## Workflow

1. Intake the brief.
   - For guided mode, read `references/00-brief-intake.md`.
   - For `bhd auto`, extract and infer without asking.

2. Select output mode and distribution context.
   - Read `references/18-output-mode-selector.md` when the user asks to audit, analyze, rewrite, improve, create variants, make copy-ready output, split a long post, or adapt content for organic/paid use.
   - Identify whether the request is Audit only, Rewrite, Paid-safe rewrite, Organic aggressive, Organic balanced, Strategic breakdown, Copy-ready only, Variants, or Series split.
   - Identify rewrite severity when improving existing content: Light edit, Medium rewrite, Hard rewrite, or Paid-safe rewrite.
   - If the user mentions ads, Facebook Ads, TikTok Ads, paid social, campaign, or landing pages connected to ads, treat distribution as paid or mixed and run paid-safe checks.

3. Analyze audience and insight.
   - Read `references/01-audience-insight.md` when audience, pain, fear, desire, objection, or trigger matters.

4. Map customer journey and experience layers.
   - Read `references/02-customer-journey-experience.md` for any content strategy, funnel, ads, landing page, campaign, or channel-growth request.

5. Build or refine the marketing canvas when strategy is incomplete.
   - Read `references/14-marketing-canvas.md` when the user asks for campaign strategy, channel plan, roadmap, positioning, proposition, metrics, or when the brief lacks goal, customer job, offer logic, channel, or measurement clarity.

6. Check whether long content should be split.
   - Read `references/22-long-post-splitter.md` when the input or requested output is long-form, has more than 4 major ideas, mixes education/proof/product pitch/compliance/roadmap, or could work better as a series.
   - In audit mode, recommend whether to keep as long-form or split into a series.
   - In writing mode, split only when the user asks or when the current format would clearly reduce readability.

7. Recommend strategic content combos.
   - Read `references/15-combo-recommendation-engine.md` after the brief is sufficient and before drafting. Use it to combine marketing canvas, customer journey, experience layer, content framework, persuasion psychology, irrational buying motivation, platform/channel, proof, CTA, and compliance risk into 2-4 suitable combos with fit scores.
   - In guided mode, show the best combos and ask the user to choose unless the user already specified the exact strategy.
   - In `bhd auto`, select the highest-scoring combo automatically and explain why.

8. Select content goal, angle, and concept.
   - Read `references/03-content-strategy-angle.md`.

9. Select writing framework.
   - Read `references/04-content-frameworks.md` when drafting copy or choosing structure.

10. Apply behavioral persuasion.
   - Read `references/05-behavioral-persuasion.md` when the output needs stronger motivation, urgency, emotion, or buying behavior.

11. Challenge the strategy before writing.
   - Read `references/16-strategy-challenge.md` after combo selection and before drafting. Use it to identify weak assumptions, missing proof, wrong journey-stage fit, vague offer, platform mismatch, compliance risk, or generic angle.
   - In guided mode, ask follow-up questions if critical gaps remain.
   - In `bhd auto`, make conservative assumptions, state the challenge notes briefly, and continue.

12. Build trust, proof, and objection handling.
   - Read `references/06-trust-proof-objection.md` for conversion copy, ads, landing pages, offers, and sales posts.

13. Grade proof strength.
   - Read `references/19-proof-grading.md` when content depends on performance claims, customer outcomes, numbers, testimonials, case studies, legal statements, or authority claims.
   - Use the proof grade to decide how strong the copy is allowed to sound.
   - If proof is Grade C or D, use softer language and suggest proof upgrades instead of inventing evidence.

14. Translate features into outcomes.
   - Read `references/20-feature-outcome-translator.md` when content lists product features, technical details, modules, templates, automations, integrations, tracking, AI workflows, or platform capabilities.
   - Convert feature-heavy sections into user meaning, business outcome, and proof/condition.
   - If a paragraph has more than 3 features, add an outcome sentence or group features into benefit clusters.

15. Shape the offer and CTA.
   - Read `references/07-offer-conversion.md` for any conversion-focused output.
   - Keep one primary CTA unless the user explicitly asks for multiple paths.
   - If multiple links are required, label their roles as primary and secondary outside copy-ready blocks.

16. Confirm copy-ready output preference.
   - Ask whether the user needs content that can be copied and used immediately unless the request already makes this obvious or `bhd auto` is active.
   - If yes, include a separate copy-ready block using `assets/copy-ready-output-template.md`. The block must contain only final usable content, without labels like "CTA:", "Headline:", "Primary text:", "Hook:", analysis notes, or explanations.
   - If no, use labeled strategic sections as needed.
   - In `bhd auto`, include a copy-ready block by default for content-writing tasks.

17. Generate the requested channel output.
   - Landing page: read `references/08-landing-page-copy.md`.
   - Facebook Ads: read `references/09-facebook-ads-copy.md`.
   - Personal brand or social post: read `references/10-personal-brand-social.md`.
   - Repurpose or calendar: read `references/11-repurpose-calendar.md`.

18. Adapt organic vs paid style.
   - Read `references/21-organic-vs-paid-style.md` when content may be used for organic social, Facebook/Instagram Ads, TikTok Ads, retargeting, landing pages connected to ads, or unclear distribution.
   - Use Organic aggressive only when the user wants a sharp founder/social voice.
   - Use Organic balanced as the default public social style.
   - Use Paid-safe for ads, paid social, retargeting, and landing pages connected to ads.

19. Run claim risk check.
   - Read `references/17-claim-risk-matrix.md` whenever the content includes numbers, performance promises, legal/compliance language, market-wide comparisons, platform-policy claims, testimonials, case studies, or superiority claims.
   - Classify risky claims by type, risk level, proof required, and safer rewrite.
   - Rewrite high-risk claims before final copy. In audit mode, risky original claims may be referenced briefly as examples, but copy-ready output should use the safer rewrite.

20. Run platform and Vietnam advertising compliance.
   - Read `references/13-platform-vietnam-compliance.md` before finalizing Facebook Ads, TikTok ads/scripts, social commerce content, landing pages, claims, testimonials, comparative copy, superlative claims, health/finance/education claims, or content intended for paid distribution in Vietnam.

21. Run final QA.
    - Read `references/12-compliance-qa.md` before finalizing ads, sales copy, landing pages, claims, testimonials, or performance promises.

## Strategic Header

Before final copy, include a compact strategic header unless the user asks for copy only:

```txt
Brief mode: Guided / bhd auto
Output mode:
Rewrite severity:
Distribution mode:
Audience:
Audience sophistication:
Journey stage:
Experience layer:
Main insight:
Primary angle:
Framework:
Persuasion lever:
Irrational buying motivation:
Recommended combo:
Combo fit score:
Strategy challenge:
Trust signal:
Proof grade:
Claim risk:
Main objection:
CTA:
Copy-ready output: Yes/No
Marketing canvas gaps:
Assumptions:
```

In guided mode, produce this header after the user has answered enough questions. In `bhd auto`, produce it immediately from the brief and assumptions.

## Missing Data Policy

Guided mode:

- Ask until there is enough information to produce a strong output.
- Do not ask for unnecessary details.
- If the user cannot answer journey or experience questions, translate them into simple choices.

`bhd auto` mode:

- Do not ask.
- Use conservative assumptions.
- Mark any unsupported claim, missing proof, or guessed audience detail.

## Output Quality Rules

- Do not fabricate numbers, customer names, testimonials, press, certifications, revenue, ROAS, or case studies.
- If proof is missing, use process proof, demo proof, checklist proof, logic proof, or placeholder proof requests.
- Challenge weak briefs. If the user's chosen direction is likely ineffective, generic, mismatched to the journey, unsupported by proof, or risky for platform/legal compliance, state the issue plainly and propose a stronger alternative.
- Do not use absolute/superlative claims such as "nhất", "duy nhất", "tốt nhất", "số một", "number one", "best", "only", or equivalent phrases unless the user provides lawful substantiation and permission to use it.
- For Facebook and TikTok outputs, check ad text, creative direction, CTA, targeting implication, landing page promise, testimonials, before-after claims, AI-generated media disclosure, and prohibited/restricted product risks.
- Avoid generic AI phrasing such as "đột phá", "toàn diện", "tối ưu" unless the context earns it.
- Prefer concrete language, specific examples, sharp hooks, clear CTA, and natural Vietnamese.
- Translate technical features into user meaning and business outcomes when the audience is not deeply technical.
- Keep one primary CTA unless the strategy clearly needs a primary and secondary CTA.
- Distinguish organic aggressive, organic balanced, and paid-safe language when distribution context is known or implied.
- Grade proof strength before using specific numbers, legal claims, market-wide claims, or superiority claims.
- Match the customer journey stage. Do not push hard selling to unaware audiences unless the user explicitly requests it.
- Match the experience layer. If trust is weak, add proof. If conversion is weak, clarify offer and CTA. If onboarding is weak, create next-step content.
- Add compliance notes for high-risk claims.

## Resource Map

- `assets/content-brief-template.md`: reusable brief form for users.
- `assets/landing-page-output-template.md`: landing page copy structure.
- `assets/facebook-ads-output-template.md`: Facebook Ads output structure.
- `assets/content-calendar-template.md`: content calendar structure.
- `assets/bhd-help.md`: user-facing usage guide for `/bhd-help`.
- `assets/copy-ready-output-template.md`: separate user-copyable final content block.
- `references/13-platform-vietnam-compliance.md`: Facebook, TikTok, and Vietnam advertising compliance guide.
- `references/14-marketing-canvas.md`: strategy canvas for goals, JTBD, proposition, message, levers, channels, metrics, and roadmap.
- `references/15-combo-recommendation-engine.md`: scoring engine for recommended content, persuasion, journey, channel, and campaign combos.
- `references/16-strategy-challenge.md`: critique engine for questioning weak strategy before writing.
- `references/17-claim-risk-matrix.md`: claim risk, proof requirement, safe rewrite, and organic/paid decision rules.
- `references/18-output-mode-selector.md`: audit/rewrite/paid-safe/organic/series/copy-ready output mode selection.
- `references/19-proof-grading.md`: proof strength grading and allowed claim intensity.
- `references/20-feature-outcome-translator.md`: translate features into user meaning, business outcomes, and safe copy lines.
- `references/21-organic-vs-paid-style.md`: adapt style and claim intensity for organic, paid, retargeting, and landing pages.
- `references/22-long-post-splitter.md`: detect long/dense content and recommend series or compression.

Use templates as output contracts when the user asks for those formats.
