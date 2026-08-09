# Use-case scoring rubric

Score each dimension **1–5**. Priority score = weighted total (max 100).

| Dimension | Weight | 1 | 3 | 5 |
|-----------|--------|---|---|---|
| **Business value** | 30% | Local convenience | Team efficiency / quality | Enterprise or customer impact, measurable $ or hours |
| **Effort** (invert) | 25% | Multi-team, 3+ months | 4–8 weeks, one maker + sponsor | Days–2 weeks, clear pattern exists |
| **Readiness** | 25% | No data, no owner, unclear process | Sponsor named, data accessible with work | Process mapped, data classified, maker available |
| **Risk / compliance** (invert) | 20% | Restricted data, no DLP path | Internal data, standard controls | Public/low sensitivity, approved connectors |

### Formula

```text
Priority = 30*(Value) + 25*(6-Effort) + 25*(Readiness) + 20*(6-Risk)
```

Effort and Risk are inverted so *lower* effort/risk increases priority.

### Decision bands

| Score | Guidance |
|-------|----------|
| **80–100** | Prioritize this cycle |
| **60–79** | Backlog — schedule when capacity opens |
| **40–59** | Park — needs sponsor, data, or pattern work |
| **&lt;40** | Decline or rewrite problem statement |

### Facilitator notes

- Do not score “AI for AI’s sake.” Value must name a process outcome.  
- Premium connectors / Copilot Studio / external APIs raise **Risk** and sometimes **Effort**.  
- Duplicate of an existing pattern → boost Readiness, cut Effort.  
