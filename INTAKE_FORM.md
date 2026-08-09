# Intake form fields

Use as a **Microsoft Form**, **SharePoint list**, or **Power Apps** canvas form. Keep required fields minimal; optional fields help triage.

## Required

| Field | Type | Notes |
|-------|------|--------|
| Title | Text | Short name of the use case |
| Business problem | Multi-line | What hurts today? |
| Desired outcome | Multi-line | Measurable success (hours saved, error rate, cycle time) |
| Sponsor (name + email) | Text | Accountable business owner |
| Process owner | Text | Day-to-day contact |
| Primary tool interest | Choice | Copilot / Power Automate / Power Apps / Copilot Studio / Other AI / Unknown |
| Data sensitivity | Choice | Public / Internal / Confidential / Restricted |

## Strongly recommended

| Field | Type | Notes |
|-------|------|--------|
| Systems involved | Text | SharePoint, Excel, SAP, Jira, etc. |
| Frequency | Choice | Ad hoc / Daily / Weekly / Monthly |
| Users impacted | Number | Approx. headcount |
| Existing workaround | Multi-line | Manual steps today |
| Deadline / regulatory driver | Date/text | Optional pressure |
| Links | URL | SOP, sample file, ticket |

## Triage-only (filled by program team)

| Field | Type |
|-------|------|
| Stage | Submitted / Triaged / Prioritized / In Build / Deployed / Parked / Declined |
| Value score (1–5) | Number |
| Effort score (1–5) | Number |
| Readiness score (1–5) | Number |
| Risk score (1–5) | Number |
| Priority score | Calculated |
| Assigned maker / squad | Person |
| Governance notes | Multi-line |
| Last updated | Date |

## SharePoint list tip

Create columns to match the CSV headers in `data/backlog.csv`. Power Automate can trigger on **item created** (see `POWER_AUTOMATE.md`).
