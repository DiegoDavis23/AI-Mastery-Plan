# 09 — SEO Keyword Clustering

**Use case:** Group a list of keywords by search intent and topic
**Recommended temperature:** 0.2
**Best model:** Any Claude model

---

## System Prompt

```
You are an SEO strategist at Atomic Digital specializing in keyword research and content architecture. You group keywords into topic clusters based on search intent and semantic similarity. Your clustering directly informs site structure and content strategy.
```

## User Prompt

```
Cluster the following keywords into topic groups.

Keywords:
{{paste_keyword_list}}

For each cluster, provide:
1. **Cluster name** — A descriptive label
2. **Search intent** — Informational, commercial, transactional, or navigational
3. **Pillar page suggestion** — The main page that should target this cluster
4. **Keywords in cluster** — Listed with estimated intent match
5. **Content recommendation** — What type of content to create (blog post, landing page, comparison page, guide, etc.)

Requirements:
- Group by topic AND intent — same topic but different intent = separate clusters
- Flag any keywords that could be their own standalone pillar page
- Identify keyword cannibalization risks (keywords too similar that would compete)
- Sort clusters by priority (highest commercial value first)

Respond as a structured table or organized list — no paragraphs.

Format:

**Cluster 1: [name]**
- Intent: [intent]
- Pillar page: [suggestion]
- Content type: [type]
- Keywords:
  - keyword 1
  - keyword 2
  - ...
- Cannibalization risk: [none / low / high — explain if high]
```

## Example

**Input:**
Keywords:
- local SEO services
- how to rank on Google Maps
- SEO for small business
- local SEO pricing
- best local SEO company
- Google Business Profile optimization
- how much does local SEO cost
- local SEO checklist
- SEO company near me
- local SEO vs organic SEO

**Output:**

**Cluster 1: Local SEO Services (Commercial)**
- Intent: Commercial
- Pillar page: /local-seo-services — "Local SEO Services for Small Businesses"
- Content type: Service/landing page
- Keywords:
  - local SEO services
  - best local SEO company
  - SEO company near me
- Cannibalization risk: High — "best local SEO company" and "SEO company near me" target similar intent. Consolidate onto one page and use ad copy variations for the other.

**Cluster 2: Local SEO Pricing (Transactional)**
- Intent: Transactional
- Pillar page: /local-seo-pricing — "Local SEO Pricing: What to Expect in 2025"
- Content type: Pricing/comparison page
- Keywords:
  - local SEO pricing
  - how much does local SEO cost
- Cannibalization risk: None

**Cluster 3: Local SEO How-To (Informational)**
- Intent: Informational
- Pillar page: /blog/local-seo-guide — "The Complete Local SEO Checklist"
- Content type: Blog post / long-form guide
- Keywords:
  - local SEO checklist
  - how to rank on Google Maps
  - Google Business Profile optimization
  - SEO for small business
- Cannibalization risk: Low — "Google Business Profile optimization" could warrant its own standalone post if search volume justifies it. Flag for future pillar page.

**Cluster 4: Local SEO vs. Organic SEO (Informational)**
- Intent: Informational
- Pillar page: /blog/local-seo-vs-organic-seo — "Local SEO vs Organic SEO: What's the Difference?"
- Content type: Blog post / comparison article
- Keywords:
  - local SEO vs organic SEO
- Cannibalization risk: None
