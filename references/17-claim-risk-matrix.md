# Claim Risk Matrix

Use this reference whenever the content includes numbers, performance promises, legal/compliance language, market-wide comparisons, platform-policy claims, testimonials, case studies, or strong superiority claims.

The goal is to keep copy persuasive without making unsupported, risky, or brittle claims.

## Claim Categories

```txt
Performance claim:
Examples: giảm CPL 30%, tăng ROAS, tăng match rate 75-90%, tiết kiệm 95%, bot dưới 5%.

Legal/compliance claim:
Examples: đúng luật, hợp Nghị định 13, tránh bị phạt, compliance-ready.

Superiority claim:
Examples: tốt nhất, duy nhất, số một, mọi công cụ khác không có, leading, best.

Certainty claim:
Examples: chắc chắn, đảm bảo, không bao giờ lỗi, dùng mãi, gần như chắc chắn tìm ra winner.

Market/platform claim:
Examples: Meta downrank hook này, TikTok không duyệt dạng này, thuật toán đang ưu tiên X.

Customer proof claim:
Examples: khách đã ra đơn, hook đã ra đơn, case giảm chi phí, testimonial, logo, feedback.

Mechanism claim:
Examples: token không nằm frontend, event_id dedup, smart loading, dual-track, webhook backend.
```

## Risk Levels

```txt
Low:
Claim is modest, conditional, mechanism-based, or supported by process proof.

Medium:
Claim is plausible but needs context, case evidence, sample size, source, or limitation.

High:
Claim sounds guaranteed, absolute, legal, market-wide, comparative, or performance-specific without proof.
```

## Proof Requirements

```txt
Performance claim:
Needs real test data, time period, sample size, campaign context, and condition.

Legal/compliance claim:
Needs legal review, source text, scope, jurisdiction, and limitation. Do not imply legal certification unless provided.

Superiority claim:
Needs lawful substantiation or independent comparison. Usually rewrite safely.

Certainty claim:
Needs strong guarantee terms or must be softened.

Market/platform claim:
Needs official policy, credible report, or clearly labeled internal observation.

Customer proof claim:
Needs permission, real customer data, screenshot, testimonial, or case note.

Mechanism claim:
Needs implementation detail or demo proof. Can often be written as a feature if not tied to guaranteed outcomes.
```

## Safe Rewrite Patterns

```txt
giảm 95% -> trong một số workflow, có thể giảm đáng kể thời gian thao tác thủ công
CPL giảm 30% -> có case/test nội bộ ghi nhận CPL giảm khoảng 30%, nhưng kết quả tùy offer, creative, tệp và setup
match rate lên 75-90% -> match rate có thể đạt khoảng 75-90% nếu tracking, data và server-side setup đúng
bot dưới 5% -> được thiết kế để giảm bot/lead rác bằng honeypot, rate-limit và chống double-submit
đúng luật -> theo checklist tham chiếu quy định liên quan, cần rà soát theo mô hình kinh doanh thực tế
hợp Nghị định 13 -> theo checklist tham chiếu Nghị định 13 về bảo vệ dữ liệu cá nhân
mọi công cụ khác không có -> khác với nhiều cách dùng AI viết ngay sau khi nhập brief
tốt nhất -> nổi bật ở / được thiết kế để / phù hợp với
duy nhất -> một điểm khác biệt là
không bao giờ lỗi -> giảm rủi ro lỗi / hạn chế lỗi thường gặp
gần như chắc chắn tìm ra winner -> tăng xác suất tìm ra hướng hiệu quả nhờ nhiều vòng test hơn
Meta downrank -> trong nhiều test/quan sát gần đây, dạng hook này có dấu hiệu bão hòa hoặc hiệu quả kém hơn
```

## Organic vs Paid Decision

```txt
Organic aggressive:
Can keep sharper language if it is clearly personal opinion, founder POV, or debate framing. Still avoid fabricated proof.

Organic balanced:
Use strong opinion plus limitations. Best default for trust-building posts.

Paid-safe:
Remove or soften unsupported numbers, superiority claims, legal claims, guaranteed outcomes, sensitive personal targeting, and aggressive personal judgment.
```

## Claim Audit Output

Return this when auditing or before finalizing high-risk copy:

```txt
Claim audit:
- Risky claim:
- Risk type:
- Risk level:
- Proof required:
- Safer rewrite:
- Use in organic: Yes/No/With caution
- Use in paid: Yes/No/With proof/Rewrite first
```
