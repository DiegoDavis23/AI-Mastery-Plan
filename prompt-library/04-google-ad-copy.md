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

## Example

**Input:**
- Business: Atomic Digital
- Service/Product: SEO services for local businesses
- Target keyword: local SEO services
- Unique selling points: Results in 90 days or less, AI-powered strategy, transparent monthly reporting
- Landing page URL: atomicdigital.com/local-seo
- Competitor weakness: Most agencies lock clients into 12-month contracts
- Offer: Free SEO audit

**Output:**

**Ad Variation 1 — Angle: Benefit**
- Headline 1: Local SEO Services That Work [28 chars]
- Headline 2: Rankings in 90 Days or Less [27 chars]
- Headline 3: Free SEO Audit — Start Now [27 chars]
- Description 1: AI-powered local SEO services built to get your business on page 1. Transparent reporting. [90 chars]
- Description 2: Stop guessing. Get a free audit and see exactly what's holding your rankings back today. [89 chars]

**Ad Variation 2 — Angle: Fear/Competitor**
- Headline 1: Stuck in a 12-Month Contract? [29 chars]
- Headline 2: Local SEO Services, No Lock-In [30 chars]
- Headline 3: Switch and Save — Free Audit [28 chars]
- Description 1: Most SEO agencies trap you in long contracts with no results. We earn your business monthly. [90 chars]
- Description 2: Flexible local SEO services powered by AI. Real rankings, real reporting, zero lock-in. [87 chars]

**Ad Variation 3 — Angle: Social Proof/Urgency**
- Headline 1: 150+ Local Businesses Ranked [28 chars]
- Headline 2: Local SEO Services by Experts [29 chars]
- Headline 3: Claim Your Free SEO Audit [26 chars]
- Description 1: Join 150+ businesses that boosted local traffic with our AI-powered SEO. Get your audit now. [90 chars]
- Description 2: Limited spots this month. See where you rank and what it takes to hit page 1. Free audit. [88 chars]
