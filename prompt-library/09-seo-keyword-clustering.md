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
