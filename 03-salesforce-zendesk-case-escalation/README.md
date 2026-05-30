# Integration Spec + Runbook — Salesforce ↔ Zendesk Case Escalation

A sample **two-document package** for a bidirectional integration that links Zendesk tickets to Salesforce Cases: a specification covering the design, and a runbook covering operations.

**[→ Read the specification](./case-escalation-spec.md)** — how it's designed
**[→ Read the runbook](./case-escalation-runbook.md)** — how it's operated

---

## What this demonstrates

- A complete two-document package — the same integration documented for two different readers and purposes
- Bidirectional sync design, including the loop-prevention contract (actor exclusion + skip-unchanged guard) that one-way syncs never need
- Per-field source-of-truth decisions where neither system fully owns the record
- Explicit, lossy status mapping between two systems with incompatible status models
- A runbook organized around the integration's defining risk — the sync loop — with containment-before-diagnosis triage

## The scenario

Fictional B2B technology company (Halytech Systems) running front-line support in Zendesk and engineering escalation in Salesforce. A Zendesk escalation creates a linked Salesforce Case; engineering's progress syncs back to the ticket. Data moves both ways, which is what makes loop prevention and source-of-truth the central design problems.

The scenario is fictional. The structure, rigor, and format are exactly what a real engagement produces.

## How it was built

Built using a code-first documentation process: direct analysis of both workflow exports and the loop-prevention configuration, not interviews. In a real engagement, the Traceability sections link to the client's actual repository.

---

*This package maps to the [Integration Specification + Runbook Package](https://contra.com/s/32A7W6Bv-integration-specification-runbook-package).*
