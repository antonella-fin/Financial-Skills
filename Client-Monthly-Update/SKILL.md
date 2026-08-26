---
name: client-monthly-update
description: >
  Generate a concise monthly financial and business update for a Finvisor
  client using the latest available financial data, client context, BvA
  analysis, cash information, KPIs, and other relevant reporting sources.
  Use when the user asks for a monthly client update, financial summary,
  management update, executive update, or monthly reporting summary.
user-invocable: true
---

# Client Monthly Update

Generate a concise, decision-useful monthly update for a Finvisor client.

The purpose of this skill is to summarize the most important financial
developments of the month without reproducing the full financial model
or BvA.

The update should answer:

1. What happened this month?
2. Why did it happen?
3. How does performance compare with plan?
4. What changed from the prior month?
5. What should management pay attention to next?

---

# Before Starting

1. Identify the client.
2. Identify the reporting month.
3. Read `Client-context` for that client.
4. Identify the latest available financial sources.
5. Use the client's reporting rules and source-of-truth definitions.
6. Determine which metrics are relevant for that client.

Never mix information between clients.

Never assume reporting methodology.

---

# Sources

Use the latest available sources defined in `Client-context`.

These may include:

- Financial model
- Accounting system
- Budget
- Forecast
- BvA analysis
- Cash forecast
- Revenue / ARR model
- Headcount model
- Payroll data
- AR / collections data
- Board reporting
- KPI dashboards
- Previous monthly update

Use the designated source of truth for each metric.

If a required source is unavailable, state that clearly.

Never invent missing numbers.

---

# Monthly Financial Analysis

Analyze the following when relevant.

## Revenue

Review:

- Revenue
- Budget / Forecast
- Variance $
- Variance %
- Month-over-month movement
- YTD performance
- ARR / MRR
- Bookings
- Pipeline

Identify the primary drivers of material changes.

---

## Gross Profit

Review:

- Gross Profit
- Gross Margin
- COGS
- Budget / Forecast variance
- Major COGS drivers

Explain whether changes are driven by:

- Revenue
- Volume
- Pricing
- Labor
- Vendors
- Usage
- Other material factors

---

## Operating Expenses

Review material changes in:

- Sales & Marketing
- R&D
- G&A
- Other relevant departments

Focus on:

- Personnel
- Headcount
- Contractors
- Software
- Marketing
- Professional services
- Other material expenses

Do not describe every account.

Focus on the largest and most decision-useful drivers.

---

## Cash

Review:

- Ending Cash
- Cash Burn
- Net Cash Flow
- Runway
- AR Collections
- Payables
- Financing activity

Explain material changes in cash.

Distinguish between:

- Operating performance
- Working capital timing
- Financing activity
- One-time cash movements

---

## Headcount

When relevant, review:

- Ending Headcount
- Budgeted Headcount
- New Hires
- Departures
- Open Positions
- Hiring delays
- Headcount-related savings or overspend

---

# Variance Analysis

Do not simply state that a variance exists.

Explain the drivers.

Bad:

`Operating expenses were $50K above budget.`

Better:

`Operating expenses were $50K above budget, primarily driven by higher contractor and software spend in G&A.`

Prioritize material drivers.

If several small items explain the variance, group them rather than listing
every account.

---

# Month-over-Month Analysis

Compare the current month with the prior month when useful.

Highlight meaningful changes such as:

- Revenue growth or decline
- Gross Margin movement
- Increase or decrease in burn
- Large AR collections
- Significant vendor spend
- Headcount changes
- One-time expenses

Do not highlight normal monthly fluctuations unless they are decision-useful.

---

# Output Structure

Default monthly update:

## [Client] — [Month] Monthly Update

### Executive Summary

Provide 3–5 concise points covering the most important developments.

Prioritize:

- Revenue
- Profitability
- Spending
- Cash
- Major risks or positive developments

---

### Financial Performance

Summarize:

- Revenue
- Gross Profit / Gross Margin
- Operating Expenses
- EBITDA / Net Income when relevant

Include Budget / Forecast comparison when available.

---

### Key Variance Drivers

Explain the largest favorable and unfavorable variances.

Focus on WHY they occurred.

---

### Cash & Runway

Summarize:

- Ending Cash
- Burn
- Collections
- Payables
- Runway

Explain any unusual movements.

---

### Headcount

Include only when relevant.

Summarize:

- Actual vs plan
- New hires
- Departures
- Hiring delays
- Financial impact

---

### Outlook

Explain meaningful forward-looking items such as:

- Expected revenue changes
- Upcoming collections
- Hiring plans
- Expected expenses
- Forecast changes
- Runway implications

Do not invent forecasts that are not supported by source data.

---

### Key Watch Items

Include only material items requiring attention.

Examples:

- Revenue below plan
- Delayed collections
- Gross Margin pressure
- Burn increasing
- Hiring ahead of revenue
- Material unbudgeted spend
- Budget becoming outdated
- Forecast assumptions requiring revision

---

# Writing Style

Write for executives and client management.

The update should be:

- Concise
- Clear
- Financial
- Data-driven
- Decision-useful
- Focused on drivers

Lead with the conclusion.

Prefer:

`Revenue finished $120K below plan, primarily due to lower enterprise sales.`

Avoid:

`There was an unfavorable variance in revenue during the month.`

Use numbers whenever they improve the explanation.

Do not over-explain accounting mechanics unless they materially affect
the conclusion.

---

# Previous Month

When a previous monthly update is available:

1. Read it.
2. Preserve useful formatting and terminology.
3. Identify what changed.
4. Do not copy old commentary without validating it against current data.
5. Remove issues that are no longer relevant.
6. Update recurring watch items.

The new update must reflect current source data.

---

# Data Quality Checks

Before producing the final update, verify:

- Reporting month is correct.
- Actuals correspond to the correct period.
- Budget / Forecast version is correct.
- YTD starts in the correct fiscal month.
- Variance calculations are correct.
- Cash figures are consistent.
- Gross Margin calculations are correct.
- Headcount figures are consistent.
- Commentary agrees with the underlying numbers.

If something does not tie, flag it.

Do not guess.

---

# Cross-Skill Workflow

Use other Finvisor skills when available.

`Client-context`
→ client rules, sources, fiscal year and reporting methodology

`Board-reporting`
→ board-level financial conclusions and existing board analysis

`BvA-analysis`
→ detailed Budget vs Actual variance drivers

`Cash-forecast`
→ cash, burn and runway

`Vendor-analysis`
→ vendor-level expense drivers

`Scenario-analysis`
→ forecast and scenario implications

Do not duplicate detailed analysis already available from another skill.

Use its conclusions to build the monthly executive update.

---

# Rules

- Always identify the client and reporting period.
- Always read Client-context first.
- Use the latest approved financial sources.
- Never mix clients.
- Never invent financial data.
- Respect the client's fiscal year.
- Respect the client's Budget / Forecast methodology.
- Explain drivers, not just variances.
- Focus on material items.
- Lead with conclusions.
- Flag missing or conflicting data.
- Distinguish actual results from forecasts and assumptions.
- Keep the final update concise.
---
