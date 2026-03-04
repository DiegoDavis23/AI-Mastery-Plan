# 08 — Social Media Repurposer

**Use case:** Turn one blog post into multiple social media posts
**Recommended temperature:** 0.7
**Best model:** Any Claude model

---

## System Prompt

```
You are a social media content strategist at Atomic Digital. You take long-form content and extract the most engaging, shareable moments to create platform-specific social media posts. You understand that each platform has different norms — Twitter/X is punchy and opinionated, LinkedIn is professional with storytelling, and Instagram is visual and inspirational.
```

## User Prompt

```
Repurpose the following blog post into social media content.

Blog post title: {{title}}
Blog post content:
{{paste_full_post_or_summary}}

Create the following:

**Twitter/X Posts (5):**
- Each under 280 characters
- Mix of: hot takes, stats, tips, and thread starters
- Use line breaks for readability
- No hashtags unless highly relevant (1 max)

**LinkedIn Posts (3):**
- 100-200 words each
- Start with a strong hook line
- Tell a micro-story or share a contrarian insight
- End with a question to drive comments
- No hashtags

**Instagram Captions (2):**
- 50-150 words
- Conversational and value-packed
- Include a CTA (save this, share this, link in bio)
- Suggest 3-5 relevant hashtags at the end

Format each clearly with the platform name and post number.
```

## Example

**Input:**
- Blog post title: "Why Most Small Businesses Waste Money on Google Ads"
- Blog post content (summary): The post argues that most small businesses launch Google Ads without proper conversion tracking, negative keywords, or landing pages — burning budget on clicks that never convert. It covers 3 common mistakes (broad match keywords, sending traffic to the homepage, and ignoring Quality Score) and offers a simple checklist to fix each one.

**Output:**

**Twitter/X Post 1:**
Most small businesses don't have a Google Ads problem.

They have a Google Ads *setup* problem.

3 fixes that can cut your wasted ad spend in half:

**Twitter/X Post 2:**
Sending Google Ads traffic to your homepage is like paying for a billboard that says "figure it out yourself."

Build a landing page. Seriously.

**Twitter/X Post 3:**
The #1 Google Ads mistake I see with small businesses: no negative keywords.

You're paying for clicks from people searching "free" and "DIY." Add those to your negative list today.

**Twitter/X Post 4:**
Google rewards relevance. If your ad says "Tampa plumber" but your landing page says "Welcome to our website," your Quality Score tanks and you pay more per click.

Match the message.

**Twitter/X Post 5:**
Hot take: Most small businesses should pause Google Ads for one week, fix their tracking, then turn them back on.

You'll spend less and convert more. #GoogleAds

**LinkedIn Post 1:**
I audited a small business Google Ads account last month. They'd spent $4,200 over 90 days.

Conversions tracked? Zero. Not because nobody converted — because tracking was never set up.

They had no idea which keywords drove leads and which ones burned cash. So they kept spending on everything equally.

We installed conversion tracking, added 85 negative keywords, and built one dedicated landing page. Same budget. Next 90 days: 47 tracked leads.

The ads weren't broken. The foundation was.

How many businesses do you think are running ads right now with no conversion tracking?

**LinkedIn Post 2:**
"We tried Google Ads. It didn't work."

I hear this constantly. But when I look under the hood, it's almost always the same three problems:

1. Broad match keywords eating the budget
2. Traffic going to the homepage instead of a landing page
3. No negative keywords filtering out junk clicks

None of these are hard to fix. But most business owners don't know they exist until the budget is gone.

What's the most common ad mistake you've seen?

**LinkedIn Post 3:**
Your Google Ads Quality Score directly affects how much you pay per click.

Low score = higher costs, worse placement. Google is literally charging you more for being irrelevant.

The fix is straightforward: make sure your keyword, ad copy, and landing page all say the same thing. Alignment is the game.

Most businesses skip this and wonder why their cost-per-lead keeps climbing. Are you checking your Quality Scores regularly?

**Instagram Caption 1:**
Stop sending ad traffic to your homepage. Seriously.

Your homepage is built for everyone. Your ad is targeting someone specific with a specific problem. Those two things need different pages.

One landing page with a clear headline, a matching offer, and a single call to action will outperform your homepage every single time.

Save this for the next time you launch a campaign.

#GoogleAds #PPC #SmallBusinessTips #DigitalMarketing #MarketingStrategy

**Instagram Caption 2:**
3 Google Ads mistakes burning your budget right now:

1. Using broad match keywords without negative keywords
2. No conversion tracking (so you're flying blind)
3. Sending clicks to a generic homepage

Fix all three this week and watch your cost per lead drop.

Tag a business owner who needs to hear this.

#GoogleAds #MarketingTips #SmallBizTips #PaidMedia
