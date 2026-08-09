# Power Automate pattern — intake to triage

## Flow A — New use case submitted

```text
Trigger: When an item is created (SharePoint list: AI Use Case Intake)
  → Scope: Initialize variables (Title, Sponsor, Sensitivity)
  → Condition: Data sensitivity = Restricted?
       │ Yes → Post adaptive card to Governance channel + set Stage = "Needs review"
       │ No  → Continue
  → Post message in Triage Teams channel (title, sponsor, link to item)
  → Send email / Teams chat to sponsor: "We received your use case"
  → Update item: Stage = Submitted, Received date = utcNow()
```

## Flow B — Weekly triage reminder (Friday or Monday)

```text
Trigger: Recurrence (weekly)
  → Get items where Stage in (Submitted, Triaged)
  → Create HTML table
  → Post to Value Hub channel: "Triage queue this week" + link to list/dashboard
```

## Flow C — Stage moved to Prioritized

```text
Trigger: When an item is modified + Stage = Prioritized
  → Notify assigned maker
  → Add row to delivery tracker (or create Planner task / DevOps work item)
```

## Connectors (typical)

| Connector | License note |
|-----------|----------------|
| SharePoint, Outlook, Teams | Standard in many M365 plans |
| Approvals | Standard |
| HTTP (e.g. external backlog) | May be premium |
| AI Builder / GPT actions | Capacity / premium — flag in governance |

## Error handling

- Configure **run after** on failed actions → post to ops channel.  
- Do not put secrets in plain compose actions; use environment variables.  
