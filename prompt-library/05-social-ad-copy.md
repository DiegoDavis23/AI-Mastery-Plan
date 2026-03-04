# 05 — Facebook/Instagram Ad Copy

**Use case:** Write social media ad copy for paid campaigns
**Recommended temperature:** 0.7
**Best model:** Any Claude model

---

## System Prompt

```
You are a social media advertising expert at Atomic Digital. You write scroll-stopping ad copy for Facebook and Instagram that drives clicks and conversions. You understand the difference between cold, warm, and hot audiences and tailor your messaging accordingly.
```

## User Prompt

```
Write Facebook/Instagram ad copy for the following campaign.

Business: {{business_name}}
Product/Service: {{product_or_service}}
Target audience: {{audience}} (demographics, interests, pain points)
Audience temperature: {{temperature}} (cold / warm / retargeting)
Campaign goal: {{goal}} (awareness, traffic, leads, sales)
Offer: {{offer}}
Landing page: {{url}}

Requirements:
- Write 3 variations, each testing a different hook
- Each ad should include:
  - Hook (first line — this is what stops the scroll)
  - Body (2-4 short sentences — problem, agitation, solution)
  - CTA (clear call to action)
- Use line breaks for readability
- Keep it conversational — no corporate speak
- Use emojis sparingly (1-2 max per ad)

Format:

**Variation 1 — Hook type: [type]**
```
[ad copy here]
```

**Variation 2 — Hook type: [type]**
```
[ad copy here]
```

**Variation 3 — Hook type: [type]**
```
[ad copy here]
```
```

## Example

**Input:**
- Business: Atomic Digital
- Product/Service: Website redesign packages
- Target audience: Small business owners (25-55) frustrated with an outdated website that doesn't generate leads
- Audience temperature: Cold
- Campaign goal: Leads
- Offer: Free website performance audit
- Landing page: atomicdigital.com/website-audit

**Output:**

**Variation 1 — Hook type: Pain point**
```
Your website is costing you customers.

If your site takes more than 3 seconds to load, 53% of visitors leave before they ever see what you offer.

We help small businesses turn their website into a 24/7 sales machine — fast load times, clear messaging, and built-in lead capture.

Grab a free website performance audit and see exactly what's costing you leads.

👉 Tap "Learn More" to claim yours.
```

**Variation 2 — Hook type: Stat/curiosity**
```
87% of consumers judge a business by its website.

What does yours say about you?

Most small business sites were "good enough" three years ago. But your customers' expectations have changed — and your competitors have caught up.

We'll audit your website for free and show you the 3 biggest fixes that will turn more visitors into paying customers.

Click below to get your free audit 🔍
```

**Variation 3 — Hook type: Transformation**
```
What if your website actually brought in leads while you slept?

That's not a fantasy. It's what happens when your site is built for conversions — not just "looking nice."

We redesign small business websites that load fast, rank on Google, and guide visitors straight to your contact form.

Start with a free website audit — we'll tell you exactly what's holding you back.

👇 Tap below to get yours.
```
