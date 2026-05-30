# Integration Runbook — Order Notification Pipeline

A sample **operational runbook** for an n8n workflow that keeps a support team's Zendesk tickets in sync with carrier shipment status.

**[→ Read the runbook](./order-notification-pipeline-runbook.md)**

---

## What this demonstrates

- Translating a technical integration (n8n webhook → status normalization → Zendesk) into operational meaning a support team can act on
- A failure-mode table that maps each break to its detection signal and response
- Monitoring guidance built around the pipeline's defining risk: it fails *silently*
- Clear separation of facts, assumptions, and unknowns — no guesses presented as certainty
- Every claim traceable to a specific source artifact

## The scenario

Fictional DTC homewares brand (Lumen Supply Co.), ~5,000 orders/week shipping via UPS, FedEx, and USPS through EasyPost, support running on Zendesk. The pipeline receives EasyPost tracking webhooks, normalizes three carrier vocabularies into one, and writes status back to the matching ticket.

The scenario is fictional. The structure, rigor, and format are exactly what a real engagement produces.

## How it was built

Built using a code-first documentation process: direct analysis of the workflow source and configuration, not interviews. In a real engagement, the Traceability section links to the client's actual repository.

---

*This runbook maps to the [Integration Runbook service](https://contra.com/s/AmQBsFgg-integration-runbook).*
