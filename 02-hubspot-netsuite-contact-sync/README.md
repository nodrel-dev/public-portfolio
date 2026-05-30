# Integration Specification — HubSpot → NetSuite Contact Sync

A sample **integration specification** for a Celigo flow that syncs HubSpot contacts into NetSuite when they become customers — without creating duplicates.

**[→ Read the specification](./hubspot-netsuite-contact-sync-spec.md)**

---

## What this demonstrates

- A complete field mapping table with direction and source-of-truth marked per field
- Deterministic matching and deduplication logic, explained as design decisions rather than steps
- Explicit source-of-truth reasoning: which system owns what, and why
- The internal-ID write-back pattern that keeps two systems linked over time
- Monitoring framed around the metric that predicts failure (create-vs-update ratio) before it becomes visible damage

## The scenario

Fictional B2B SaaS company (Meridian) running go-to-market in HubSpot and finance in NetSuite. When a contact becomes a customer, Celigo creates or updates the matching NetSuite contact under the correct customer, then writes the NetSuite internal ID back to HubSpot.

The scenario is fictional. The structure, rigor, and format are exactly what a real engagement produces.

## How it was built

Built using a code-first documentation process: direct analysis of the Celigo flow export and field mappings, not interviews. In a real engagement, the Traceability section links to the client's actual configuration.

---

*This specification maps to the [Integration Specification + Runbook Package](https://contra.com/s/32A7W6Bv-integration-specification-runbook-package).*
