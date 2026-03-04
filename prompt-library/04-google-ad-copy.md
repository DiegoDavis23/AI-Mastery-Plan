# 04 — Google Ad Copy

**Use case:** Generate Google Search ad variations (headlines + descriptions)
**Recommended temperature:** 0.6
**Best model:** Any Claude model

---

## System Prompt

```
You are a Google Ads specialist at Atomic Digital. You write high-converting search ad copy that maximizes Quality Score and click-through rate. You understand character limits, keyword insertion, and emotional triggers that drive clicks.
```

## User Prompt

```
Create Google Search ad copy for the following campaign.

Business: {{business_name}}
Service/Product: {{service_or_product}}
Target keyword: {{keyword}}
Unique selling points: {{usps}}
Landing page URL: {{url}}
Competitor weakness to exploit (optional): {{competitor_weakness}}
Offer/Promotion (optional): {{offer}}

Requirements:
- Headlines: Max 30 characters each
- Descriptions: Max 90 characters each
- Include the target keyword in at least 2 headlines
- Use numbers, power words, or urgency when appropriate
- Each variation should test a different angle (benefit, fear, social proof, urgency)

Provide 3 complete ad variations in this format:

**Ad Variation 1 — Angle: [angle name]**
- Headline 1: ... [xx chars]
- Headline 2: ... [xx chars]
- Headline 3: ... [xx chars]
- Description 1: ... [xx chars]
- Description 2: ... [xx chars]

**Ad Variation 2 — Angle: [angle name]**
...

**Ad Variation 3 — Angle: [angle name]**
...
```
