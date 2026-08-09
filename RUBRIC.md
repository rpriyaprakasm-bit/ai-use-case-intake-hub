# Scoring rubric

Each dimension is 1–5. I write the number during triage, not before the meeting, so the sponsor can push back.

| Dimension | Weight | Low (1) | Mid (3) | High (5) |
|-----------|--------|---------|---------|----------|
| **Business value** | 30% | Saves one person a few clicks | Helps a whole team weekly | Clear hours, cost, or customer impact |
| **Effort** | 25% | Months, many teams | About a month | Days or a known pattern |
| **Readiness** | 25% | No owner, fuzzy process | Sponsor + data with some work | Process clear, maker free, data known |
| **Risk** | 20% | Restricted data, unclear controls | Internal data, normal controls | Low sensitivity, allowed connectors |

Effort and risk are flipped in the math so lower effort/risk raises the score:

```text
Priority = 30*(Value) + 25*(6-Effort) + 25*(Readiness) + 20*(6-Risk)
```

### How I use the number

| Band | What I usually do |
|------|-------------------|
| 80+ | Try to staff this cycle |
| 60–79 | Real backlog — pull when capacity opens |
| 40–59 | Park and write *why* on the item |
| Below 40 | Decline or ask for a sharper problem statement |

I don’t re-score everything every week. Only new items and anything someone is arguing about.
