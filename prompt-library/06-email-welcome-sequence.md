# 06 — Email Welcome Sequence

**Use case:** Create a 3-email onboarding sequence for new subscribers or leads
**Recommended temperature:** 0.6
**Best model:** Claude Sonnet or Opus

---

## System Prompt

```
You are an email marketing strategist at Atomic Digital. You write email sequences that build trust, deliver value, and convert subscribers into customers. Your emails are concise, personal, and always include a clear next step. You write like a smart friend giving advice, not a corporation sending a newsletter.
```

## User Prompt

```
Write a 3-email welcome sequence for the following business.

Business: {{business_name}}
Industry: {{industry}}
What the subscriber signed up for: {{lead_magnet_or_offer}}
Main product/service to eventually sell: {{product_or_service}}
Brand voice: {{voice}} (e.g., friendly and bold, professional but warm)
CTA for the sequence: {{desired_action}} (e.g., book a call, start free trial, buy)

Requirements for each email:
- Subject line (under 50 chars) + preview text (under 80 chars)
- Body: 150-250 words max
- Write in first person (from the founder)
- Each email has ONE clear CTA — do not add multiple links
- Use short paragraphs (1-3 sentences)

Sequence structure:
- **Email 1 (Day 0):** Welcome + deliver what they signed up for + set expectations
- **Email 2 (Day 2):** Provide quick value/tip related to their problem + build credibility
- **Email 3 (Day 4):** Soft pitch — share a result/case study + CTA to take action

Format each email as:

**Email [#] — Day [#]**
**Subject:** ...
**Preview text:** ...

[email body]

[CTA button text]
```

## Example

**Input:**
- Business: Atomic Digital
- Industry: Digital marketing
- What the subscriber signed up for: Free guide — "5 SEO Fixes That Double Your Traffic"
- Main product/service to eventually sell: Monthly SEO management packages
- Brand voice: Friendly and bold
- CTA for the sequence: Book a free strategy call

**Output:**

**Email 1 — Day 0**
**Subject:** Your SEO guide is here
**Preview text:** Plus what to fix on your site first (takes 10 min)

Hey {{first_name}},

Welcome — and thanks for grabbing the guide.

Here's your copy of **5 SEO Fixes That Double Your Traffic**: [Download Link]

Fair warning: Fix #3 alone has helped our clients see traffic jumps of 30-50% in a single month. Start there if you're short on time.

Over the next few days, I'll send you a couple of quick tips that go beyond what's in the guide. No fluff, no pitch-a-thon — just stuff that works.

Talk soon,
Davis — Atomic Digital

**[Download My Free Guide]**

---

**Email 2 — Day 2**
**Subject:** The SEO mistake I see every week
**Preview text:** Takes 5 minutes to fix and it's probably on your site

Hey {{first_name}},

Here's something I see on almost every small business site we audit: **title tags that don't include the city you serve.**

Google uses your title tag as a primary ranking signal for local searches. If yours just says "Home — Your Business Name," you're invisible for local keywords.

Quick fix:
1. Go to your homepage
2. Change your title tag to: **[Primary Service] in [City] | [Business Name]**
3. Do the same for your top 3 service pages

That's it. Five minutes, real results.

Want to know what else is holding your site back? I might have an idea for you in my next email.

Davis

**[Re-read the SEO Guide]**

---

**Email 3 — Day 4**
**Subject:** How we took a site from 800 to 4,200 visits/mo
**Preview text:** Same industry, similar starting point — here's how

Hey {{first_name}},

Quick story: A local service business came to us getting about 800 organic visits per month. Good service, good reviews — but their website was working against them.

We ran the same fixes from your guide, then layered on a content strategy and technical cleanup. Within 4 months: **4,200 monthly visits and 35+ inbound leads per month.**

No ads. No tricks. Just SEO that compounds.

If you've gone through the guide and want to see what a full strategy would look like for your business, let's talk. No pressure, no commitment — just a 20-minute call to see where the biggest opportunities are.

Davis

**[Book a Free Strategy Call]**
