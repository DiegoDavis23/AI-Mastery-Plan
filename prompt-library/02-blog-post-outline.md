# 02 — Blog Post Outline

**Use case:** Generate an SEO-optimized blog structure before writing
**Recommended temperature:** 0.5
**Best model:** Any Claude model

---

## System Prompt

```
You are an SEO content strategist at Atomic Digital. You create blog post outlines that rank on Google by matching search intent, using proper heading hierarchy, and including semantic keywords naturally. Every outline you create is designed to be comprehensive, scannable, and actionable.
```

## User Prompt

```
Create a detailed blog post outline for the following topic.

Target keyword: {{keyword}}
Secondary keywords: {{secondary_keywords}}
Search intent: {{intent}} (informational / commercial / transactional / navigational)
Target audience: {{audience}}
Desired word count: {{word_count}} (e.g., 1500, 2500)
Competitor URLs to beat (optional): {{competitor_urls}}

Requirements:
- Start with a compelling H1 title that includes the target keyword
- Use H2 and H3 subheadings in logical hierarchy
- Include a "Key Takeaways" or "TL;DR" section at the top
- Each section should have 1-2 bullet points describing what to cover
- Suggest where to place internal links and CTAs
- Include a FAQ section at the bottom with 3-5 questions
- Suggest the meta description and URL slug

Respond in this format:

**Title (H1):** ...
**URL slug:** ...
**Meta description:** ...

**Key Takeaways:**
- ...

**Outline:**
## H2: ...
### H3: ...
- Points to cover
- [CTA opportunity] or [internal link opportunity]

**FAQ Section:**
- Q: ...
  A: (brief answer direction)
```

## Example

**Input:**
- Target keyword: AI for small business marketing
- Secondary keywords: AI marketing tools, small business AI, automated marketing
- Search intent: informational
- Target audience: Small business owners with limited marketing budgets
- Desired word count: 2000
