# AI Use-Case Intake Hub

**Intake → triage → prioritize → track** for AI and citizen-led automation initiatives.

Built as a portfolio pattern for **AI Value Hub / CoE-style** programs: structured backlog, transparent scoring, Power Automate-ready workflow, and a live pipeline dashboard.

[![Dashboard](https://img.shields.io/badge/Live-Dashboard-38bdf8)](https://raw.githack.com/rpriyaprakasm-bit/ai-use-case-intake-hub/main/docs/dashboard.html)

---

## Why this exists

Value Hub teams need more than ideas in email. They need:

1. A **standard intake form** (business problem, data sensitivity, tools, sponsor)
2. A **scoring rubric** (value, effort, readiness, risk)
3. A **pipeline view** (Submitted → Triaged → Prioritized → In Build → Deployed / Parked)
4. Clear **handoffs** to makers, delivery leads, and governance

This repo is a ready-to-adapt blueprint with sample data and docs.

---

## What’s included

| Artifact | Purpose |
|----------|--------|
| [docs/dashboard.html](./docs/dashboard.html) | Pipeline dashboard (counts, RAG, top scored cases) |
| [data/backlog.csv](./data/backlog.csv) | Sample use-case backlog |
| [data/backlog.json](./data/backlog.json) | Same data for the dashboard |
| [RUBRIC.md](./RUBRIC.md) | Value / effort / readiness / risk scoring |
| [INTAKE_FORM.md](./INTAKE_FORM.md) | Fields for SharePoint list or Microsoft Form |
| [POWER_AUTOMATE.md](./POWER_AUTOMATE.md) | Flow pattern: new item → notify → triage queue |
| [GOVERNANCE_CHECKLIST.md](./GOVERNANCE_CHECKLIST.md) | Data classification, licensing, DLP gates |
| [PLAYBOOK_TRIAGE.md](./PLAYBOOK_TRIAGE.md) | 30-min weekly triage meeting agenda |

---

## Pipeline stages

```text
Submitted → Triaged → Prioritized → In Build → Deployed
                ↘ Parked / Declined
```

---

## Skills demonstrated (role map)

- Intake, triage, prioritization, backlog tracking  
- AI / automation use-case lifecycle  
- Stakeholder coordination and risk flags  
- Power Automate + SharePoint/Excel pattern  
- Governance and deployment readiness gates  
- Reusable program documentation  

---

## Live demo

**→ [Open pipeline dashboard](https://raw.githack.com/rpriyaprakasm-bit/ai-use-case-intake-hub/main/docs/dashboard.html)**

---

## License

MIT
