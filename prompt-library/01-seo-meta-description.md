# 01 — SEO Meta Description

**Use case:** Write click-worthy meta descriptions for any page
**Recommended temperature:** 0.4
**Best model:** Any Claude model

---

## System Prompt

```
You are a senior SEO copywriter at Atomic Digital, an AI-powered digital agency. You specialize in writing meta descriptions that maximize click-through rates from Google search results.
```

## User Prompt

```
Write a meta description for the following page.

Page type: {{page_type}} (e.g., homepage, service page, blog post, product page)
Business: {{business_name}}
Industry: {{industry}}
Target keyword: {{keyword}}
Page content summary: {{brief_summary}}

Requirements:
- Under 155 characters (hard limit)
- Include the target keyword naturally — do not force it
- Use active voice
- Include a clear call to action or value proposition
- Create urgency or curiosity without being clickbait
- Do not use quotes or special characters

Respond with exactly 3 variations, formatted as:

1. [meta description] — [character count]
2. [meta description] — [character count]
3. [meta description] — [character count]
```

## Example

**Input:**
- Page type: Service page
- Business: Atomic Digital
- Industry: Digital marketing
- Target keyword: AI marketing agency
- Page content summary: We use AI to optimize marketing campaigns, SEO, and web design for growing businesses.

**Output:**
1. Grow faster with an AI marketing agency that optimizes your SEO, ads, and content automatically. See results in 48hrs. — 131 chars
2. AI marketing agency built for growth. We use data-driven AI to scale your traffic, leads, and revenue. Start free. — 117 chars
3. Your AI marketing agency partner. Smarter campaigns, faster results, compounding growth. Book a free strategy call. — 119 chars
