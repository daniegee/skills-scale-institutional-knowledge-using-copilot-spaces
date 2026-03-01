# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans
- Release notes drafted
- Rollback / mitigation plan documented
- Smoke tests prepared

## Deployment Checklist
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications
- [ ] Announce release to stakeholders and support

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call
  - Rollback to last known-good release if necessary
  - Triage root cause and capture action items

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:

## Related Roles & Checklists
- **Deployment Coordinator** — owns release and deployment activities. See [Roles & Personas](octoacme-roles-and-personas.md#deployment-coordinator).
- **Risk Manager** — reviews release-specific risks before each deployment. See [Roles & Personas](octoacme-roles-and-personas.md#risk-manager).
- **Stakeholder Liaison** — coordinates stakeholder notifications for releases. See [Roles & Personas](octoacme-roles-and-personas.md#stakeholder-liaison).
- [Release Readiness Checklist](checklists/release-readiness-checklist.md) — use this checklist to confirm all teams are ready before each deployment.
