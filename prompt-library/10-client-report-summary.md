# 10 — Client Report Summary

**Use case:** Turn raw analytics data into a clear, actionable client report
**Recommended temperature:** 0.3
**Best model:** Any Claude model

---

## System Prompt

```
You are a digital marketing analyst at Atomic Digital. You translate raw analytics data into clear, jargon-free insights that business owners can understand and act on. You always lead with what matters most — revenue impact, traffic changes, and what to do next. You never dump numbers without context.
```

## User Prompt

```
Generate a client performance report summary from the following data.

Client: {{client_name}}
Reporting period: {{date_range}}
Previous period for comparison: {{comparison_period}}

Data:
{{paste_data}}
(This could be Google Analytics, Search Console, ad platform data, or a CSV)

Include these sections:

**1. Executive Summary (3-4 sentences)**
- Biggest win this period
- Biggest concern or area to watch
- Overall trend direction (growing, flat, declining)

**2. Key Metrics**
- Present each metric with: current value, previous value, % change, and a one-line interpretation
- Use arrows or +/- to show direction
- Format as a clean table

**3. Top Insights (3-5 bullets)**
- What's working and why
- What's not working and why
- Any anomalies or surprises in the data

**4. Recommendations (3-5 bullets)**
- Specific, actionable next steps based on the data
- Prioritize by expected impact
- Each recommendation should start with a verb (Increase, Test, Fix, Create, etc.)

**5. Next Period Goals**
- 2-3 measurable targets for the next reporting period

Requirements:
- Write for a business owner, not a marketer — no jargon
- Every number needs context ("12,000 sessions" means nothing without comparison)
- Be honest about what's not working — don't sugarcoat
- Keep the entire report under 500 words
```

## Example

**Input:**
- Client: Brightside Dental
- Reporting period: February 2025
- Previous period: January 2025
- Data:
  - Sessions: 4,820 (was 3,910)
  - Organic sessions: 3,105 (was 2,340)
  - Google Ads clicks: 1,290 (was 1,410)
  - Google Ads spend: $2,100 (was $2,100)
  - Form submissions: 87 (was 62)
  - Phone calls from website: 34 (was 28)
  - Top landing page: /teeth-whitening-tampa (1,240 sessions)
  - Bounce rate: 52% (was 58%)
  - Avg. session duration: 2m 18s (was 1m 52s)

**Output:**

**1. Executive Summary**

February was Brightside Dental's strongest month since we started. Organic traffic jumped 33% thanks to the teeth whitening content we published in January, and total leads (forms + calls) hit 121 — up 40% from last month. One area to watch: Google Ads click volume dipped 8.5% at the same budget, suggesting rising competition in paid search. Overall trend is solidly upward.

**2. Key Metrics**

| Metric | Feb 2025 | Jan 2025 | Change |
|---|---|---|---|
| Total Sessions | 4,820 | 3,910 | +23.3% |
| Organic Sessions | 3,105 | 2,340 | +32.7% |
| Google Ads Clicks | 1,290 | 1,410 | -8.5% |
| Ad Spend | $2,100 | $2,100 | — |
| Cost Per Ad Click | $1.63 | $1.49 | +9.4% |
| Form Submissions | 87 | 62 | +40.3% |
| Phone Calls | 34 | 28 | +21.4% |
| Total Leads | 121 | 90 | +34.4% |
| Bounce Rate | 52% | 58% | -6 pts |
| Avg. Session Duration | 2m 18s | 1m 52s | +23.3% |

**3. Top Insights**

- The /teeth-whitening-tampa page is the #1 traffic driver this month, pulling 1,240 sessions almost entirely from organic search. The blog-to-service-page strategy is paying off.
- Bounce rate dropped 6 points and time on site increased — visitors are finding your content more relevant and exploring more pages.
- Google Ads cost per click rose 9.4% without a budget change, which means you got fewer clicks for the same spend. Competitor bidding in the Tampa dental space is heating up.
- Form submissions grew faster than phone calls, suggesting the new contact form placement on service pages is working.

**4. Recommendations**

- **Create** 2 more localized service pages (dental implants, emergency dentist) to replicate the teeth whitening traffic success.
- **Audit** Google Ads keywords and pause any with cost-per-click above $3.50 and low conversion rates to fight rising CPCs.
- **Test** a click-to-call button above the fold on mobile — phone leads are growing but still lag behind form fills.
- **Add** patient testimonials to the top 3 landing pages to improve trust signals and conversion rate.

**5. Next Period Goals**

- Reach 5,500 total sessions (+14%)
- Hit 135 total leads (forms + calls)
- Reduce Google Ads cost per click below $1.50 through keyword refinement
