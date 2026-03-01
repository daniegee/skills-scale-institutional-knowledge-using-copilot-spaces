# Process Improvement Log Template

**Owner:** [Process Improvement Champion](../octoacme-roles-and-personas.md#process-improvement-champion)
**Related docs:** [Roles & Personas](../octoacme-roles-and-personas.md) | [Retrospective & Continuous Improvement](../octoacme-retrospective-and-continuous-improvement.md)

## Purpose
Capture improvement opportunities, decisions, and outcomes in a structured, searchable log. The Process Improvement Champion owns this log, surfaces items at retrospectives, and tracks implementation through to completion.

## Usage Notes
- Add entries whenever a process gap or improvement opportunity is identified — during retrospectives, standups, incidents, or ad-hoc discussions.
- Review the log at each retrospective and at the weekly PM sync.
- Mark items as **Done** when the improvement is implemented and validated; archive periodically.
- Share outcomes with the broader team to build institutional knowledge and celebrate progress.

---

## Improvement Log

| ID | Title | Description | Source (e.g., retro, incident) | Category | Priority (High/Med/Low) | Status | Owner | Target Date | Outcome / Notes |
|----|-------|-------------|-------------------------------|----------|------------------------|--------|-------|-------------|-----------------|
| PI-001 | _Example: Automate release notes generation_ | _Currently release notes are written manually, causing delays_ | Sprint 3 retrospective | Tooling | Medium | In Progress | Process Improvement Champion | YYYY-MM-DD | _Draft automation script created_ |
| PI-002 | | | | | | | | | |

### Status Values
- **Proposed** — Identified but not yet reviewed/prioritized
- **Approved** — Accepted for implementation; owner and timeline assigned
- **In Progress** — Implementation underway
- **Done** — Implemented and validated
- **Deferred** — Acknowledged but deprioritized; revisit date noted
- **Won't Do** — Reviewed and explicitly declined (document reason)

### Category Examples
- Process — Changes to how the team works (meetings, workflows, ceremonies)
- Tooling — New tools, automation, or improvements to existing tools
- Documentation — Updates to process docs, templates, or checklists
- Communication — Improvements to internal or external communication
- Quality — Testing, review, or quality gate improvements
- Other — Anything that doesn't fit the above

---

## Retrospective Action Items (Linked)

Improvement items that originate from retrospectives should also be tracked as issues in the project board with a clear owner and due date. Reference the issue link in the **Outcome / Notes** column above (e.g., `#123` for GitHub issues or a full URL for external trackers).

See [Retrospective & Continuous Improvement](../octoacme-retrospective-and-continuous-improvement.md) for the retrospective structure and action item template.

---

## Quarterly Review Checklist

- [ ] Review all **In Progress** items — are they on track?
- [ ] Close or defer any stale items with documented rationale
- [ ] Identify top 3 improvement themes for next quarter
- [ ] Share improvement outcomes with team and leadership
- [ ] Update the Process Improvement Log and commit to project repo
