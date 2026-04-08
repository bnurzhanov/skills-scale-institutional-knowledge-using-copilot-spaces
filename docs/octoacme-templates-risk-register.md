# OctoAcme — Risk Register Template

## Purpose
Provide a copy/paste-ready Risk Register table and guidance so that all projects track risks in a consistent, actionable format that matches the guidance in the Risk Management & Communication doc.

## When to use
- Start the register during project initiation and keep it active through closeout.
- Update at every weekly sync and immediately when a new risk is discovered.
- Archive closed risks (status = Closed/Resolved) but keep them in the table for audit history.

---

## Risk Register Table

Copy the table below into your project's `docs/` folder or project README.

| ID | Date Identified | Description | Category | Impact (H/M/L) | Likelihood (H/M/L) | Risk Score | Owner | Mitigation Plan | Contingency Plan | Status | Last Updated |
|----|-----------------|-------------|----------|----------------|--------------------|------------|-------|-----------------|------------------|--------|--------------|
| RISK-001 | YYYY-MM-DD | Short description of the risk | Technical / Schedule / Resource / External / Compliance | H / M / L | H / M / L | (see scoring) | @owner | Steps to reduce impact or likelihood | What we do if it happens | Open / Mitigated / Closed | YYYY-MM-DD |

---

## Field Definitions

| Field | Description |
|-------|-------------|
| **ID** | Sequential identifier (RISK-001, RISK-002, …). |
| **Date Identified** | When the risk was first logged. |
| **Description** | Clear, concise statement of the risk (what could go wrong). |
| **Category** | `Technical`, `Schedule`, `Resource`, `External`, or `Compliance`. |
| **Impact (H/M/L)** | Effect on project objectives if the risk occurs: `H` = project-critical, `M` = significant but manageable, `L` = minor. |
| **Likelihood (H/M/L)** | Probability the risk will occur: `H` = likely (>50 %), `M` = possible (20–50 %), `L` = unlikely (<20 %). |
| **Risk Score** | Derived from Impact × Likelihood. See scoring table below. |
| **Owner** | GitHub username of the person accountable for monitoring and mitigating this risk. |
| **Mitigation Plan** | Proactive steps to reduce the impact or likelihood before the risk occurs. |
| **Contingency Plan** | Reactive steps taken if the risk does occur (fallback). |
| **Status** | `Open` (active), `Mitigated` (mitigation in place, still monitored), or `Closed` (no longer relevant). |
| **Last Updated** | Date the row was last edited. |

---

## Risk Scoring Matrix

Use this 3×3 matrix to assign a numeric score (1–9). Prioritize risks with score ≥ 6.

|  | **Low Impact (1)** | **Medium Impact (2)** | **High Impact (3)** |
|---|---|---|---|
| **High Likelihood (3)** | 3 | 6 | **9** |
| **Medium Likelihood (2)** | 2 | 4 | **6** |
| **Low Likelihood (1)** | 1 | 2 | 3 |

---

## Example

| ID | Date Identified | Description | Category | Impact | Likelihood | Risk Score | Owner | Mitigation Plan | Contingency Plan | Status | Last Updated |
|----|-----------------|-------------|----------|--------|------------|------------|-------|-----------------|------------------|--------|--------------|
| RISK-001 | 2025-01-10 | Third-party API may deprecate v1 endpoint before our migration completes | External | H | M | 6 | @eng-lead | Monitor API changelog; begin migration work in Sprint 3. | Pin to v1 behind a feature flag; fast-track migration if deprecation announced. | Open | 2025-01-17 |
| RISK-002 | 2025-01-12 | Key developer unavailable for 2 weeks during critical phase | Resource | M | L | 2 | @pm | Cross-train a second developer on the affected module. | Re-prioritize scope; pull in contractor if timeline is threatened. | Mitigated | 2025-02-01 |
| RISK-003 | 2025-02-05 | Security scan flags a critical dependency vulnerability | Technical | H | H | 9 | @security-lead | Add automated dependency scanning to CI; set SLA for critical fixes. | Pause release; apply patch; re-run full test suite before deploying. | Closed | 2025-02-08 |

---

## Maintenance Guidance
- **Who updates it:** The PM owns the register; risk owners update their rows.
- **Cadence:** Review at every weekly sync; update `Last Updated` for any row discussed or changed.
- **Single source of truth:** Keep the register in `docs/risk-register.md` (or linked from the project README). Do not maintain parallel copies in other tools without a sync plan.
- **Escalation:** Any risk with a score ≥ 6 should be surfaced in the weekly stakeholder update (see [Risk Management & Communication](./octoacme-risks-and-communication.md)).

---

## References
- [Risk Management & Communication](./octoacme-risks-and-communication.md) — lifecycle and escalation paths
- [Project Planning](./octoacme-project-planning.md) — initial risk identification
- [Execution & Tracking](./octoacme-execution-and-tracking.md) — weekly risk review
- [Project Closeout](./octoacme-project-closeout.md) — final risk disposition
