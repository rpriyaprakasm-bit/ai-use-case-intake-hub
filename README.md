# AI Use-Case Intake Hub

I kept getting the same problem: good automation ideas stuck in email, no shared way to say yes, later, or no.

This repo is a simple intake and prioritization setup I would actually run — SharePoint/Excel backlog, a scoring sheet, a weekly triage agenda, and a small dashboard so the queue is visible.

**Dashboard:** [open it here](https://raw.githack.com/rpriyaprakasm-bit/ai-use-case-intake-hub/main/docs/dashboard.html)

---

## What’s in the folder

| File | What it’s for |
|------|----------------|
| `docs/dashboard.html` | Counts by stage + sorted backlog |
| `data/backlog.csv` | Sample cases (mix of deployed, stuck, and declined) |
| `RUBRIC.md` | How I score value, effort, readiness, risk |
| `INTAKE_FORM.md` | Fields I’d put on a Form or SharePoint list |
| `POWER_AUTOMATE.md` | Flow sketch when a new item lands |
| `GOVERNANCE_CHECKLIST.md` | Things to check before something goes live |
| `PLAYBOOK_TRIAGE.md` | 30-minute weekly meeting — tight on purpose |

---

## Stages I use

```text
Submitted → Triaged → Prioritized → In Build → Deployed
                ↘ Parked / Declined
```

Parked is not the same as declined. Parked means “not now — missing owner, data, or a pattern.” Declined means we won’t do it in this shape.

---

## Choices I made on purpose

- **Four scores, not twelve.** People stop using rubrics that feel like homework.
- **Risk and effort are inverted in the formula** so “hard and risky” doesn’t float to the top just because someone wrote a long pitch.
- **Sample data includes a declined HR bot and a parked contract tool.** Real queues have both.
- **No Dataverse in the default design.** A lot of teams only have SharePoint lists; the pattern should still work.

What I didn’t build: a full Power App UI or CoE Starter Kit install. That’s intentional — this is the operating layer, not a platform rebuild.

---

## If you copy this

1. Put the columns from `data/backlog.csv` into a SharePoint list.  
2. Wire the flow in `POWER_AUTOMATE.md` (or skip automation until volume justifies it).  
3. Run triage for two weeks before changing the rubric.  

---

MIT
