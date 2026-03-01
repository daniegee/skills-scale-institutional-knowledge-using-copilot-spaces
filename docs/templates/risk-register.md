# Risk Register Template

**Owner:** [Risk Manager](../octoacme-roles-and-personas.md#risk-manager)
**Related docs:** [Roles & Personas](../octoacme-roles-and-personas.md) | [Risk Management & Communication](../octoacme-risks-and-communication.md)

## Purpose
Provide a lightweight, consistent structure for tracking project risks. The Risk Manager owns this register, updates it at least weekly, and reviews it with the Project Manager at each sync.

## Usage Notes
- Create one Risk Register per project and store it in the project's `docs/` folder.
- Use the **Risk Score** (Impact × Likelihood) to prioritize mitigation efforts.
- Review all open risks at the weekly PM sync; close or archive risks that are resolved.
- Escalate **High** or **Critical** risks to the Project Manager immediately.

## Risk Scoring Guide

| Score | Impact | Likelihood |
|-------|--------|------------|
| 1 | Low — minimal effect on scope, timeline, or quality | Unlikely — rare occurrence |
| 2 | Medium — noticeable but manageable impact | Possible — could occur |
| 3 | High — significant impact on timeline, budget, or quality | Likely — expected to occur |

**Risk Score = Impact × Likelihood** (range: 1–9)
- 1–2: Low
- 3–4: Medium
- 6–9: High/Critical — escalate to PM

## Risk Register

| ID | Description | Category | Impact (1–3) | Likelihood (1–3) | Risk Score | Owner | Mitigation Plan | Contingency Plan | Status | Date Identified | Last Updated |
|----|-------------|----------|-------------|-----------------|------------|-------|-----------------|-----------------|--------|----------------|--------------|
| R-001 | _Example: Third-party API deprecation before release_ | Technical | 3 | 2 | 6 | Risk Manager | Evaluate alternative APIs; track vendor roadmap | Switch to fallback integration | Open | YYYY-MM-DD | YYYY-MM-DD |
| R-002 | | | | | | | | | | | |

## Risk Lifecycle

1. **Identify** — Raise risks during planning, standups, or at any point in execution
2. **Assess** — Risk Manager assigns impact, likelihood, and score
3. **Assign** — Risk Manager assigns an owner for each mitigation action
4. **Mitigate** — Owner executes mitigation plan; Risk Manager tracks progress
5. **Monitor** — Review status at weekly PM sync; update score if conditions change
6. **Close** — Mark risk as resolved when mitigation is complete or risk is no longer applicable

## Escalation Path

- **Medium risk** (score 3–4): Monitor weekly; include in status updates
- **High/Critical risk** (score 6–9): Escalate to Project Manager → Product Lead → Sponsor as needed
