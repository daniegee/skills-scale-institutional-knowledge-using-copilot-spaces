# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## Communication Lead

### Role Summary
The Communication Lead ensures that project information reaches the right audiences at the right time. They own the communication plan, manage status reporting, and coordinate messaging across internal and external channels.

### Responsibilities
- Own and maintain the project communication plan
- Draft and distribute regular status updates and announcements
- Coordinate with the Stakeholder Liaison for external communications
- Manage incident communications in partnership with the Project Manager
- Maintain a single source of truth for project status (e.g., project README or release doc)

### Key Artifacts
- Communication Plan
- Weekly status reports
- Announcement drafts and incident communications

### Typical Communication
- Weekly sync with Project Manager
- Milestone-based updates to stakeholders
- Ad-hoc communications for incidents or major decisions

---

## Risk Manager

### Role Summary
The Risk Manager owns the identification, assessment, monitoring, and mitigation of project risks. They ensure risk visibility across teams and support informed decision-making.

### Responsibilities
- Identify and document risks throughout the project lifecycle (initiation through close)
- Assess each risk for impact and likelihood; assign risk scores
- Define and track mitigation actions and contingency plans
- Maintain the [Risk Register](templates/risk-register.md) and keep it current
- Facilitate risk review discussions at weekly syncs and planning sessions
- Escalate high-impact risks to the Project Manager and Product Lead promptly
- Coordinate cross-functional teams on risk-response actions

### Key Artifacts
- [Risk Register](templates/risk-register.md) — owned and maintained by the Risk Manager

### Interactions & Cadence
- **Project Manager**: weekly risk review; escalation for decisions requiring PM authority
- **Developers**: identify technical risks during planning and execution
- **Deployment Coordinator**: align on release-specific risks before each deployment
- **Communication Lead**: share risk status for inclusion in stakeholder updates

### Decision Rights / Escalation
- Owns risk assessment and mitigation recommendations
- Escalates unresolved High/Critical risks to PM → Product Lead → Sponsor as needed

---

## Deployment Coordinator

### Role Summary
The Deployment Coordinator oversees all release and deployment activities. They act as the primary liaison between engineering and operations, ensuring planned releases align with defined processes and quality standards.

### Responsibilities
- Plan, schedule, and coordinate deployment windows with engineering and operations
- Maintain and execute the [Release Readiness Checklist](checklists/release-readiness-checklist.md)
- Ensure all pre-release requirements are met before production deployments
- Manage communication around releases (announcements, post-deploy confirmations)
- Lead rollback decisions and incident response during deployment failures
- Document lessons learned from release incidents

### Key Artifacts
- [Release Readiness Checklist](checklists/release-readiness-checklist.md) — owned by Deployment Coordinator
- Release notes and deployment runbooks

### Interactions & Cadence
- **Project Manager**: align release milestones and flag schedule risks
- **Developers**: confirm feature readiness, PR merge status, and hotfix priorities
- **Risk Manager**: review release-specific risks before each deployment
- **Stakeholder Liaison**: coordinate stakeholder notifications for significant releases

### Decision Rights / Escalation
- Owns go/no-go decision for deployment execution (in coordination with PM)
- Escalates critical deployment failures to PM and on-call operations team

---

## Stakeholder Liaison

### Role Summary
The Stakeholder Liaison serves as the primary point of contact for external stakeholders. They ensure stakeholder requirements and feedback are integrated into the project and facilitate two-way communication between the team and stakeholders.

### Responsibilities
- Identify and map stakeholders; maintain the [Stakeholder Communication Plan](templates/stakeholder-comms-plan.md)
- Gather stakeholder requirements, constraints, and expectations at project initiation
- Facilitate regular stakeholder check-ins and review meetings
- Ensure stakeholder feedback is captured and triaged with the Product Manager
- Represent stakeholder interests in planning and prioritization discussions
- Coordinate approval and sign-off processes for key milestones

### Key Artifacts
- [Stakeholder Communication Plan](templates/stakeholder-comms-plan.md) — owned by Stakeholder Liaison
- Stakeholder feedback summaries and decision logs

### Interactions & Cadence
- **Product Manager**: weekly alignment on stakeholder requirements and priorities
- **Communication Lead**: coordinate messaging and update cadence
- **Project Manager**: escalate unresolved stakeholder issues or blockers
- **Deployment Coordinator**: notify stakeholders of upcoming releases and maintenance windows

### Decision Rights / Escalation
- Owns stakeholder mapping and communication cadence decisions
- Escalates unresolved stakeholder conflicts to PM → Product Lead

---

## Process Improvement Champion

### Role Summary
The Process Improvement Champion drives continuous improvement initiatives across the project team. They collect feedback, identify process gaps, and collaborate with all roles to implement sustainable improvements.

### Responsibilities
- Facilitate retrospectives and gather structured team feedback
- Identify and document process inefficiencies, gaps, and improvement opportunities
- Maintain the [Process Improvement Log](templates/process-improvement-log.md)
- Prioritize and champion improvement initiatives with leadership support
- Track the implementation and impact of process changes
- Share improvement outcomes across teams to build institutional knowledge

### Key Artifacts
- [Process Improvement Log](templates/process-improvement-log.md) — owned by Process Improvement Champion
- Retrospective notes and action item summaries

### Interactions & Cadence
- **Project Manager**: weekly review of outstanding improvement actions
- **All roles**: retrospective sessions after sprints, releases, and incidents
- **Communication Lead**: share improvement results in stakeholder updates where relevant

### Decision Rights / Escalation
- Owns the process improvement backlog and prioritization recommendations
- Escalates systemic or cross-team issues to PM and Product Lead

---

## RACI Summary

The table below maps key project process activities to roles. **R** = Responsible, **A** = Accountable, **C** = Consulted, **I** = Informed.

| Activity | Project Manager | Product Manager | Developers | Communication Lead | Risk Manager | Deployment Coordinator | Stakeholder Liaison | Process Improvement Champion |
|---|---|---|---|---|---|---|---|---|
| Project Initiation | A/R | C | I | I | C | I | C | I |
| Planning & Backlog | A | R | C | I | C | C | C | I |
| Execution & Tracking | A | C | R | I | C | I | I | C |
| Risk Identification & Management | C | I | C | I | A/R | C | I | C |
| Stakeholder Communication | C | C | I | R | I | I | A/R | I |
| Release / Deployment | A | I | C | C | C | R | I | I |
| Retrospective / Continuous Improvement | C | C | C | I | C | C | I | A/R |

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- See also the supporting templates and checklists in [`docs/templates/`](templates/) and [`docs/checklists/`](checklists/) for artifacts owned by specific roles.

