# Nodrel — Documentation Portfolio

Integration and systems documentation for SaaS operations teams, written by an integration engineer who documents from the codebase, not from interviews.

These are representative samples. Each is built on a fictional scenario, but the structure, rigor, and format are exactly what a real engagement produces. In a real engagement, every traceability reference resolves to the client's own repository.

---

## Samples

| # | Document | Type | Stack | Service |
|---|----------|------|-------|---------|
| 1 | [Order Notification Pipeline](./01-order-notification-runbook) | Runbook | n8n → Zendesk, EasyPost | [Integration Runbook](https://contra.com/s/AmQBsFgg-integration-runbook) |
| 2 | [HubSpot → NetSuite Contact Sync](./02-hubspot-netsuite-contact-sync) | Specification | Celigo, HubSpot, NetSuite | [Spec + Runbook Package](https://contra.com/s/32A7W6Bv-integration-specification-runbook-package) |
| 3 | [Salesforce ↔ Zendesk Case Escalation](./03-salesforce-zendesk-case-escalation) | Spec + Runbook | n8n, Salesforce, Zendesk | [Spec + Runbook Package](https://contra.com/s/32A7W6Bv-integration-specification-runbook-package) |
| 4 | [Celigo vs. n8n for Ops Automation](./04-adr-n8n-vs-celigo) | ADR | Platform decision | [Systems Documentation Sprint](https://contra.com/s/ergPoELN-systems-documentation-sprint) |

---

## What runs through all four

- **Code-first.** Documentation built from workflow exports, configs, and source — not secondhand accounts. The output reflects how a system actually behaves, not how someone remembers it.
- **Decision-useful diagrams.** Every diagram is Mermaid, readable, and exists to help someone understand or decide — never decoration.
- **Honest confidence.** Facts, assumptions, and unknowns are kept separate. Nothing inferred is presented as certain.
- **Traceable.** Every substantial claim ties back to a specific source artifact.

## The range

The four samples deliberately span document types and tools: an operational runbook, a design specification, a two-document package for a bidirectional integration, and a platform-level decision record — across n8n, Celigo, Salesforce, Zendesk, HubSpot, and NetSuite. The point is to show fluency across both the *kinds* of documentation a team needs and the *platforms* it runs on.

---

*Services: [Contra profile](https://contra.com/kyle_tully_01gz48a4)*
