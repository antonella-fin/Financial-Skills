---
name: board-reporting
description: >
  Prepare board reporting materials for Finvisor clients using the latest
  available financial data and client context. Use when the user asks to
  prepare, update, review, or analyze a board deck, board financial section,
  monthly financial presentation, or board financial commentary.
user-invocable: true
---

# Board Reporting

Prepare board-ready financial reporting for Finvisor clients.

The goal is to turn the latest financial data into concise, decision-useful
board reporting.

## Before Starting

1. Identify the client.
2. Read the client's context using `Client-context`.
3. Identify the reporting period.
4. Identify the financial sources configured for that client.
5. Determine whether the user wants:
   - a full board financial report,
   - an update to an existing board deck,
   - a specific financial section, or
   - a review of an existing board deck.

Never assume that reporting rules are the same across clients.

---

# Data Sources

Use the sources defined in the client's context.

These may include:

- Financial model
- Accounting system
- Budget
- Latest forecast
- Revenue / ARR model
- Cash forecast
- Headcount model
- Payroll data
- Existing board deck
- KPI reporting files

Use the client's configured source of truth for each metric.

If a source is unavailable, clearly state what is missing and continue with
the available information.

Never invent financial data.

---

# Financial Analysis

When available, analyze:

## Revenue

- Revenue
- Budget / Forecast
- Variance $
- Variance %
- MoM growth
- YTD performance
- ARR / MRR
- Bookings or pipeline when relevant

## Gross Profit

- Gross Profit
- Gross Margin
- COGS
- Major drivers of variance

## Operating Expenses

Analyze by department when available:

- Sales & Marketing
- R&D
- G&A
- Other relevant departments

Identify:

- Personnel variances
- Headcount variances
- Contractor spend
- Software spend
- Marketing spend
- Professional services
- Other material drivers

## Profitability

When available:

- EBITDA
- Operating Income
- Net Income

Compare against Budget / Forecast.

## Cash

Analyze:

- Ending Cash
- Cash Burn
- Net Cash Flow
- Runway
- AR Collections
- AP / Payables

Highlight unusual cash movements.

## Headcount

Analyze:

- Actual Headcount
- Budgeted Headcount
- New Hires
- Departures
- Open Positions
- Headcount variance

---

# Variance Analysis

Do not only report that a variance exists.

Explain WHY it happened.

Example:

Bad:

`Revenue was $75K below budget.`

Better:

`Revenue was $75K below budget, primarily driven by lower-than-expected T&M sales of $39K and ATE sales of $10K.`

Prioritize the largest and most decision-useful drivers.

Do not list immaterial variances unless specifically requested.

---

# Board Reporting Structure

Default structure:

## 1. Executive Summary

Summarize the 3–5 most important financial developments.

Focus on:

- Revenue performance
- Gross margin
- Operating expenses
- Cash / runway
- Major risks or changes to forecast

Lead with conclusions.

---

## 2. Key Metrics

When available include:

| Metric | Actual | Budget / Forecast | Variance | Prior Period |
|---|---:|---:|---:|---:|
| Revenue | | | | |
| Gross Profit | | | | |
| Gross Margin | | | | |
| Operating Expenses | | | | |
| EBITDA / Net Income | | | | |
| Ending Cash | | | | |
| Cash Burn | | | | |
| Runway | | | | |
| Headcount | | | | |

Only include metrics relevant to the client.

---

## 3. Revenue & Gross Profit

Explain:

- Revenue performance
- Major revenue drivers
- COGS performance
- Gross Profit
- Gross Margin
- Material variances

---

## 4. Operating Expenses

Explain material variances by department.

Focus on WHY spending was above or below plan.

Avoid describing every account.

---

## 5. Cash & Runway

Explain:

- Ending cash
- Cash burn
- Collections
- Payables
- Runway
- Major expected cash movements

Flag liquidity risks clearly.

---

## 6. Headcount

Explain:

- Actual vs plan
- Hiring changes
- Departures
- Hiring delays
- Financial impact

---

## 7. Forecast / Outlook

When forecast data is available, explain:

- Changes to expected revenue
- Changes to expenses
- Expected cash burn
- Runway impact
- Hiring assumptions
- Major risks to the forecast

---

## 8. Key Risks & Watch Items

Identify items management or the board should monitor.

Examples:

- Revenue below plan
- Collections delays
- Higher burn
- Hiring ahead of revenue
- Gross margin pressure
- Material unbudgeted expenses
- Forecast assumptions no longer aligned with actual performance

---

# Existing Board Deck

If the user provides an existing board deck:

1. Review the existing structure.
2. Preserve the client's established format unless instructed otherwise.
3. Identify which slides contain financial information.
4. Update those slides using the latest financial sources.
5. Recalculate all dependent metrics.
6. Update commentary.
7. Check consistency across slides.

Do not rebuild the entire presentation unless requested.

---

# Consistency Checks

Before completing the report, verify:

- Monthly numbers tie to the financial model.
- YTD uses the correct fiscal-year start.
- Budget / Forecast version matches Client-context.
- Variance $ is correct.
- Variance % is correct.
- Cash figures tie across slides.
- Headcount is consistent across slides.
- Gross Margin calculations are correct.
- Dates and reporting periods are consistent.
- Commentary agrees with the numbers shown.

Flag any inconsistency instead of guessing.

---

# Commentary Style

Board commentary should be:

- Concise
- Financial
- Executive-level
- Specific
- Data-driven
- Focused on drivers

Prefer:

`Gross Profit was $75K below plan, primarily driven by lower T&M revenue and higher ATE COGS.`

Avoid:

`Gross Profit experienced an unfavorable variance compared to budget due to several factors affecting the business during the month.`

Use numbers whenever they improve the explanation.

---

# Output

When the user asks for board reporting analysis, return:

1. Executive Summary
2. Key Metrics
3. Revenue & Gross Profit
4. Operating Expenses
5. Cash & Runway
6. Headcount
7. Forecast / Outlook
8. Key Risks / Watch Items

If the user asks only for a specific section, return only that section.

If the user asks to update an existing board deck, preserve its existing
structure and update only the required sections.

---

# Rules

- Always read Client-context first.
- Never mix information between clients.
- Never invent financial data.
- Use the latest approved financial sources.
- Respect each client's fiscal year.
- Respect each client's Budget / Forecast methodology.
- Explain drivers, not just variances.
- Focus on material items.
- Lead with conclusions.
- Flag missing or conflicting data.
- Preserve existing board deck structure unless asked to change it.
- Validate numbers before producing final commentary.

