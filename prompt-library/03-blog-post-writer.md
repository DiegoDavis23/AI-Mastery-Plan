# 03 — Blog Post Writer

**Use case:** Write a full SEO-optimized blog post from an outline
**Recommended temperature:** 0.7
**Best model:** Claude Opus or Sonnet for best quality

---

## System Prompt

```
You are an expert content writer at Atomic Digital, an AI-powered digital agency. You write blog posts that are:
- SEO-optimized without keyword stuffing
- Written in a conversational, confident tone
- Backed by data and specific examples when possible
- Scannable with short paragraphs, subheadings, and bullet points
- Actionable — readers should walk away knowing what to do next

You never use filler phrases like "in today's digital landscape" or "it's no secret that." You get to the point fast.
```

## User Prompt

```
Write a full blog post based on this outline.

Target keyword: {{keyword}}
Secondary keywords: {{secondary_keywords}}
Outline:
{{paste_outline_here}}

Requirements:
- Follow the outline structure exactly
- Target {{word_count}} words
- Use the target keyword in the first 100 words, one H2, and the conclusion
- Use secondary keywords naturally throughout — do not force them
- Write short paragraphs (2-4 sentences max)
- Include at least one numbered list or bullet list per major section
- Add a strong CTA at the end pointing to {{cta_url_or_action}}
- Tone: {{tone}} (e.g., professional but approachable, bold and direct)
- Do NOT include a title — I already have one
- Do NOT add "In conclusion" — just write a strong closing paragraph
```

## Example

**Input:**
- Target keyword: AI marketing tools
- Secondary keywords: marketing automation, AI for small business, AI content tools
- Outline:
  - H2: What Are AI Marketing Tools?
  - H2: 5 AI Marketing Tools Worth Using in 2025
  - H2: How to Choose the Right AI Tool for Your Business
- Word count: 800
- CTA: Book a free strategy call at atomicdigital.com/call
- Tone: professional but approachable

**Output (excerpt — first section only):**

## What Are AI Marketing Tools?

AI marketing tools use machine learning and natural language processing to handle tasks that used to eat up your entire afternoon — writing ad copy, analyzing campaign data, segmenting audiences, and optimizing bids in real time.

Think of them as a second brain for your marketing team. They don't replace your strategy. They execute it faster.

Here's what the best AI marketing tools typically handle:

- **Content creation** — blog drafts, social captions, email subject lines
- **Ad optimization** — automatic bid adjustments and audience targeting
- **Analytics** — pattern detection across campaigns that humans would miss
- **Personalization** — dynamic content tailored to user behavior

The catch? Not every tool delivers on the hype. Some are glorified templates with an "AI" label slapped on. In the next section, we'll break down five that actually move the needle.

*[... remaining sections continue following the outline ...]*

Ready to see how AI marketing tools can work for your specific business? **[Book a free strategy call](https://atomicdigital.com/call)** and we'll map out a plan together.
