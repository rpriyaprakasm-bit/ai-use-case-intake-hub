# Governance & deployment readiness checklist

Complete before **In Build → Deployed** for production use.

## Data & compliance

- [ ] Data sensitivity classified (Public / Internal / Confidential / Restricted)
- [ ] No Restricted data in personal productivity tools without approved pattern
- [ ] Retention / records policy considered if storing business records
- [ ] External sharing off unless explicitly required

## Platform & security

- [ ] Flows/apps built in correct **environment** (not default, if policy requires)
- [ ] Connectors allowed under **DLP** policy
- [ ] Least-privilege connections (service account vs personal where required)
- [ ] Secrets in secure store — not hard-coded in flows

## Licensing

- [ ] Premium connectors identified and capacity confirmed
- [ ] Copilot / Copilot Studio licensing path confirmed for intended users
- [ ] Guest/external users considered

## Solution quality

- [ ] Owner and backup owner named
- [ ] Basic error handling and run history monitored
- [ ] Documentation link (SOP or readme) attached to backlog item
- [ ] Success metric defined and baseline noted

## Deployment

- [ ] UAT with sponsor complete
- [ ] Support path agreed (maker vs L1 vs Value Hub)
- [ ] Rollback / disable plan known

**Escalation:** blocked items → Value Hub lead + risk/technology partner within 5 business days.
