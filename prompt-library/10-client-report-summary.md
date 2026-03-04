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
