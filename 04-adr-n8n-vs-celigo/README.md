# Architecture Decision Record — Celigo vs. n8n for Ops Automation

A sample **ADR** recording a platform decision: which automation tool a growing systems team should standardize on, and how to route future work between them.

**[→ Read the ADR](./adr-ops-automation-platform.md)**

---

## What this demonstrates

- Platform-level architectural judgment, not just integration documentation
- A genuine decision with a clear statement, not a vendor comparison that dodges the call
- A full alternatives table — including the rejected single-tool options and why each fails the context
- A nuanced but committed outcome: workload allocation by fit, with an explicit routing rule for future work
- Honest trade-offs (vendor lock-in, two-platform operating surface) stated plainly rather than hidden
- The closing insight that the strategy fails on governance, not technology — if no one owns routing, the estate drifts

## The scenario

Fictional mid-market SaaS company (Brightline) whose integration needs have outgrown an informal all-n8n approach. The systems team needs a deliberate platform strategy across NetSuite, Salesforce, HubSpot, and Zendesk.

The scenario is fictional. The reasoning, structure, and decision discipline are exactly what a real engagement produces.

## Why an ADR

A runbook documents how something runs. A specification documents how something is built. An ADR documents *why a decision was made* — the reasoning that the other documents assume. It is the highest-leverage document type for a team that wants to understand not just its systems, but the choices behind them.

## How it was built

Built using a code-first documentation process: analysis of the existing automation estate and a proof-of-concept, not interviews alone. In a real engagement, the Traceability section links to the client's actual artifacts.

---

*This document maps to the [Systems Documentation Sprint](https://contra.com/s/ergPoELN-systems-documentation-sprint), where ADRs are a typical deliverable.*
