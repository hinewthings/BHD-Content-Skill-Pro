# Feature To Outcome Translator

Use this reference when content lists product features, technical details, modules, templates, algorithms, tracking, automation, AI workflows, integrations, or platform capabilities.

The goal is to prevent feature dumping and turn features into customer-relevant outcomes.

## Translation Formula

```txt
Feature:
What the product/tool does.

User meaning:
Why the user should care in plain language.

Business outcome:
What this can improve in time, cost, trust, data quality, conversion, risk, speed, or control.

Proof/condition:
What must be true for the outcome to happen.

Copy line:
One natural sentence for the final content.
```

## Examples

```txt
Feature: Pixel + CAPI dedup
User meaning: Giảm lỗi đếm trùng và lệch dữ liệu.
Business outcome: Thuật toán có dữ liệu sạch hơn để tối ưu.
Proof/condition: Cần setup event_id và server-side đúng.
Copy line: Tracking được thiết kế để giảm lỗi đếm trùng bằng event_id dedup giữa Pixel và CAPI.
```

```txt
Feature: Honeypot + rate-limit
User meaning: Giảm bot và submit rác.
Business outcome: Lead sạch hơn, đội sales đỡ mất thời gian.
Proof/condition: Cần cấu hình form và rule phù hợp.
Copy line: Form có honeypot và rate-limit để giảm lead rác trước khi dữ liệu đi vào campaign.
```

```txt
Feature: Smart loading
User meaning: Chỉ load phần cần dùng.
Business outcome: Tiết kiệm token và trả lời gọn hơn.
Proof/condition: Cần cấu trúc module rõ.
Copy line: Skill chỉ gọi đúng module cần thiết, nên nhẹ hơn khi bạn chỉ hỏi một phần nhỏ.
```

```txt
Feature: Industry presets
User meaning: Bài viết bớt generic.
Business outcome: Giọng, pain, hook và từ vựng sát ngành hơn.
Proof/condition: Cần preset dựa trên insight thật hoặc dữ liệu test.
Copy line: Preset theo ngành giúp bài ra sát bối cảnh khách hàng hơn thay vì nghe như một mẫu AI chung chung.
```

## Feature Density Rule

```txt
If a paragraph contains more than 3 features, add an outcome sentence.
If a post contains more than 7 features, group them into 2-3 benefit clusters.
If the audience is non-technical, translate technical terms before listing them.
If the audience is senior/technical, keep mechanism detail but still connect it to business impact.
```

## Benefit Clusters

Use these clusters:

```txt
Speed:
test nhanh hơn, ra bản nháp nhanh hơn, giảm thời gian chờ.

Control:
không phụ thuộc vendor, tự chỉnh được, workflow rõ hơn.

Data quality:
tracking sạch hơn, ít lệch hơn, ít bot hơn, dễ đọc số liệu hơn.

Conversion:
offer rõ hơn, CTA gọn hơn, objection được xử lý tốt hơn.

Trust:
proof rõ hơn, claim mềm hơn, policy/chính sách được rà trước.

Cost:
giảm thao tác thuê ngoài, giảm vòng sửa, giảm lãng phí thử sai.
```

## Output

Return when auditing:

```txt
Feature-outcome check:
- Feature-heavy area:
- Missing user meaning:
- Better outcome framing:
- Suggested rewrite:
```
