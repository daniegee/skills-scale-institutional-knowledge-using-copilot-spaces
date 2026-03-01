# Release Readiness Checklist

**Owner:** [Deployment Coordinator](../octoacme-roles-and-personas.md#deployment-coordinator)
**Related docs:** [Roles & Personas](../octoacme-roles-and-personas.md) | [Release & Deployment Guide](../octoacme-release-and-deployment.md) | [Risk Register Template](../templates/risk-register.md)

## Purpose
Ensure all teams complete required steps before a release is promoted to production. The Deployment Coordinator is responsible for completing this checklist and confirming sign-off from each role before deployment proceeds.

## Usage Notes
- Complete this checklist for every **Minor** and **Major** release. For **Patch** releases, use the abbreviated checklist below.
- The Deployment Coordinator shares this checklist in the release tracking issue or project board card.
- All items must be checked ✅ or explicitly waived with documented justification before go-live.
- For any blocking item, the Deployment Coordinator escalates to the Project Manager.

---

## Full Release Readiness Checklist (Minor / Major)

### 1. Code & Quality
- [ ] All acceptance criteria for release scope are met
- [ ] All feature PRs are merged to the release branch
- [ ] CI pipeline passes (tests, lint, security scans)
- [ ] Code review completed and approved for all changes
- [ ] No known critical or high-severity bugs outstanding (or documented exceptions)

### 2. Risk & Communication
- [ ] Release-specific risks reviewed with Risk Manager and mitigations in place
  - _Reference: [Risk Register](../templates/risk-register.md)_
- [ ] Rollback / mitigation plan documented and validated
- [ ] Deployment window communicated to all affected teams

### 3. Staging & Testing
- [ ] Deployed to staging environment successfully
- [ ] Smoke tests passed on staging
- [ ] End-to-end acceptance tests passed (or signed off by QA)
- [ ] Performance / load testing completed (if applicable)

### 4. Documentation & Release Notes
- [ ] Release notes drafted and reviewed
  - _Reference: [Release & Deployment Guide](../octoacme-release-and-deployment.md)_
- [ ] User-facing documentation updated (if applicable)
- [ ] API or migration documentation updated (if applicable)

### 5. Stakeholder Sign-off
- [ ] Product Manager / Product Lead approves release scope
- [ ] Stakeholder Liaison has notified relevant external stakeholders
- [ ] Support team briefed on changes and known issues

### 6. Deployment Handoffs
- [ ] Deployment runbook prepared and shared with operations
- [ ] On-call contacts confirmed for deployment window
- [ ] Monitoring dashboards and alerts confirmed active
- [ ] Backup / snapshot taken (if applicable)

### 7. Post-Deploy
- [ ] Post-deploy verification steps documented
- [ ] Announcement drafted (internal and/or external)
- [ ] Retrospective / blameless review scheduled (if applicable)

---

## Abbreviated Checklist (Patch / Hotfix)

- [ ] Root cause identified and fix validated in staging
- [ ] CI pipeline passes
- [ ] Rollback plan confirmed
- [ ] On-call notified of deployment window
- [ ] Post-deploy verification steps ready
- [ ] Stakeholder Liaison notified (if customer-facing)

---

## Sign-off

| Role | Name | Sign-off Date |
|------|------|--------------|
| Deployment Coordinator | | |
| Project Manager | | |
| Product Manager | | |
| Risk Manager | | |
| Stakeholder Liaison (if required) | | |
