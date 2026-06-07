# Output Mode Selector

Use this reference at the start of a request when the user asks to create, analyze, rewrite, audit, repurpose, or improve content.

The goal is to match the output to what the user actually needs instead of using one response format for every task.

## Output Modes

```txt
Audit only:
Analyze strengths, weaknesses, journey fit, proof, CTA, compliance, and recommended fixes. Do not rewrite unless asked.

Rewrite:
Keep the core idea and improve structure, clarity, trust, CTA, and persuasion.

Paid-safe rewrite:
Rewrite for Facebook/TikTok/paid social with safer claims, lower policy risk, clearer disclaimers, and fewer aggressive personal judgments.

Organic aggressive:
Write for organic reach, founder POV, debate, curiosity, and sharper voice. Still do not fabricate proof.

Organic balanced:
Write for trust and authority while keeping a clear personal voice. This is the default for public social posts.

Strategic breakdown:
Explain angle, audience, journey, framework, proof, objections, CTA, and risks. Use when the user wants reasoning.

Copy-ready only:
Return only final usable copy, no analysis labels, no strategic notes.

Variants:
Produce multiple versions by angle, platform, tone, journey stage, or risk level.

Series split:
Turn a long or dense post into a multi-post series.
```

## Selection Rules

```txt
If user says "đánh giá", "phân tích", "audit":
Use Audit only unless they also ask for rewrite.

If user says "viết lại", "rewrite", "sửa":
Use Rewrite. If paid platform is mentioned, use Paid-safe rewrite.

If user mentions ads, Facebook Ads, TikTok Ads, paid, campaign, landing page for ads:
Use Paid-safe checks even if final style is organic.

If user mentions "viral", "gắt", "mạnh", "organic":
Use Organic aggressive with claim control.

If user mentions "tham khảo", "cho tôi vài bản":
Use Variants or Rewrite depending on context.

If content is over 900-1200 Vietnamese words or has more than 4 major ideas:
Consider Series split and mention it in recommendations.

If user says "copy dùng luôn":
Use Copy-ready only or include a separate copy-ready block.
```

## Rewrite Severity

Use rewrite severity when improving existing content:

```txt
Light edit:
Keep 80-90% of original wording. Fix clarity, flow, claim risk, CTA.

Medium rewrite:
Keep the core idea and voice. Rebuild structure and transitions.

Hard rewrite:
Keep only the strategic intent. Write a stronger version from scratch.

Paid-safe rewrite:
Prioritize compliance and trust over maximum intensity.
```

Default:

```txt
For "viết lại mình tham khảo": Medium rewrite.
For "tối ưu để chạy ads": Paid-safe rewrite.
For "giữ giọng này": Light edit or Medium rewrite.
For weak strategy: Hard rewrite after explaining why.
```

## Output Mode Header

Include in strategic outputs:

```txt
Output mode:
Rewrite severity:
Distribution mode: Organic / Paid / Both / Unknown
```
