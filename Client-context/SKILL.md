---
name: finvisor-context
description: >
  Reads and updates context for Finvisor clients and generates a concise
  client financial report using the latest connected sources.
user-invocable: true
---

# Finvisor Context

Use this skill to view or update the current financial and reporting context
for a Finvisor client.

Each client has its own context file containing:

- Financial sources
- Accounting system
- Budget and forecast sources
- Reporting rules
- Key metrics
- Important accounting rules
- Current issues
- Recurring deliverables

## View Context

When the user runs:

`/finvisor-context <client>`

1. Identify the client.
2. Read the client's context.
3. Read the latest available connected financial sources.
4. Generate a concise report.

The report should include, when available:

- Reporting period
- Revenue
- ARR / MRR
- Gross Margin
- Operating Expenses
- Cash
- Burn
- Runway
- Headcount
- Budget / Forecast version
- Latest BvA
- Latest Board Deck
- Current financial issues
- Important client-specific rules

Do not show raw configuration files.

## Update Context

When the user runs:

`/finvisor-context update <client>`

1. Read the client's configured financial sources.
2. Pull the latest available data.
3. Identify the latest Actual month.
4. Extract summary financial metrics.
5. Compare them with the existing context.
6. Update only fields that changed.
7. Generate the updated client report.

Do not overwrite unrelated client information.

## Client Sources

Each client may have sources such as:

- Google Sheets financial model
- QBO / Xero / Netsuite
- Payroll system
- Revenue model
- Budget
- Forecast
- Board deck

Use the configured source of truth for each metric.

## Rules

- Never hallucinate missing client context.
- Never mix information between clients.
- Prefer current connected sources over old context.
- Clearly flag missing or stale data.
- Never silently change reporting methodology.
- Keep reports concise and decision-useful.

