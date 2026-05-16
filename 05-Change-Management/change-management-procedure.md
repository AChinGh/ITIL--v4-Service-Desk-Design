# Change Management Procedure  
### Richmond Solutions Inc. — IT Service Management

**Document Version:** 1.1  

**Last Updated:** 2026  

**Owner:** IT Manager  

**ITIL Practice Area:** Change Enablement, Release Management  

---

### 1. Purpose

The purpose of Change Management is to ensure IT changes at Richmond Solutions Inc. are implemented in a controlled and standardized manner while minimizing risk to business operations.

This process supports:
- Service stability
- Controlled deployment of changes
- Risk reduction
- Operational visibility
- Rollback preparedness
- Continual improvement

The objective is to maximize successful changes while minimizing:
- Service disruption
- Failed implementations
- Operational downtime
- Security risk

---

### 2. Scope

This process applies to all IT changes that may affect:
- Microsoft 365 services
- User endpoints
- Identity systems
- VPN infrastructure
- Networking equipment
- Shared drives
- Business applications
- Authentication policies
- Security controls

---

### 3. Definition of a Change

A **change** is the addition, modification, or removal of anything that could directly or indirectly affect IT services.

Examples include:
- Software deployment
- Network configuration updates
- Policy modifications
- VPN upgrades
- Server maintenance
- Identity and access changes

---

### 4. Change Objectives

The Change Management process aims to:
- Assess implementation risk
- Ensure proper authorization
- Maintain operational visibility
- Reduce change-related incidents
- Support rollback capability
- Improve implementation consistency

---

### 5. Change Types

### 5.1 Standard Change


### Standard Change
- **Definition:** Pre-approved, low risk, well-understood, follows a documented procedure, repeatable
- **Authorization:** Pre-approved — no individual assessment needed
- **CAB Required:** No
- **Examples at Richmond Solutions:**
  - Password reset / account unlock
  - Standard software installation from approved list
  - Adding user to existing distribution list
  - Routine weekly patch application (Patch Tuesday)
  - Printer configuration using standard procedure

##

### 5.2 Normal Change

- **Definition:** Requires individual risk assessment, formal authorization before implementation, implementation planning
- **Authorization:** IT Manager (low-medium risk) or CAB (high risk)
- **CAB Required:** Yes for high-risk changes
- **Examples at Richmond Solutions:**
  - New software deployment organization-wide
  - Network infrastructure changes (Firewall rule modifications)
  - Server configuration changes (VPN configuration changes)
  - New user access permissions (non-standard)
  - Changes to conditional access policies (M365)

##

### 5.3 Emergency Change

- **Definition:** Must be implemented urgently to restore service, prevent significant business impact or mititgate security threats
- **Authorization:** Emergency CAB (IT Manager + available senior staff)
- **CAB Required:** Emergency CAB only
- **Examples at Richmond Solutions:**
  - Critical security patch for active vulnerability
  - Emergency fix for a P1 major incident
  - Immediate rollback of a failed change causing outage

---

### 6. Change Authority Matrix

| Change Type | Authorization Required |
|:--------|:---------------------------|
| Standard Change | Pre-approved - no individual authority required |
| Normal Change (Low - medium Risk) | IT Manager |
| Normal Change (High Risk) | CAB Approval: IT Manager + Department Head + Senior Analyst |
| Emergency Change | Emergency CAB: IT Manager + available staff (minimum 2 approvers) |

---

### 7. Change Advisory Board (CAB)

The CAB reviews high-risk changes before implementation.

## CAB Members

| Role | Responsibility |
|:-----|:---------------|
| IT Manager | CAB Chair |
| Senior IT Analyst | Technical Review |
| Department Representative | Business Impact Review |
| Vendor Representative | External System Review (if required) |

##

## CAB Schedule

| Activity | Schedule |
|:---------|:---------|
| Standard CAB Meeting | Tuesdays — 10:00 AM EST |
| Emergency CAB | As required |

| # | Agenda Item |
|:--|:------------|
| 1 | Review changes submitted since last meeting |
| 2 | Risk assessment for normal changes |
| 3 | Change schedule review |
| 4 | Post-implementation review of recent changes |
| 5 | Failed and rejected change debrief |

---

### 8. Change Lifecycle

```text
Request Submitted
↓
Initial Review
↓
Risk Assessment
↓
Authorization
↓
Scheduling
↓
Implementation
↓
Validation
↓
Post-Implementation Review
↓
Closure
```

---

### 9. Change Process Workflow

### 9.1 Change Submission

All non-standard changes must include:
- Business justification
- Affected systems
- Implementation plan
- Rollback procedure
- Risk assessment
- Testing details

##

### 9.1.1. Change Request Form Template

| Field | Detail |
|:------|:-------|
| Change ID | [Auto-generated] |
| Date Submitted | |
| Submitted By | |
| Change Title | |
| Change Type | Standard / Normal / Emergency |
| Priority | Low / Medium / High / Critical |
| Business Justification | |
| Affected Systems | |
| Users Affected | |
| Risk Level | Low / Medium / High |
| Implementation Plan | |
| Rollback Plan | |
| Testing Details | |
| Scheduled Date | |
| Maintenance Window Required | Yes / No |
| CAB Approval Required | Yes / No |

**Approvals**

| Role | Name | Date |
|:-----|:-----|:-----|
| IT Manager | | |
| CAB Chair (if applicable) | | |
| Department Head (if required) | | |

**Post-Implementation**

| Field | Detail |
|:------|:-------|
| Implementation Successful | Yes / No / Partial |
| Issues Encountered | |
| Rollback Required | Yes / No |
| PIR Required | Yes / No |
| PIR Scheduled | |

##

### 9.2 Risk Assessment

Risk is evaluated based on:
- Service criticality
- Number of users affected
- Security impact
- Implementation complexity
- Rollback feasibility

##

### 9.3 Authorization

Changes must receive approval before implementation.

Authorization depends on:
- Risk level
- Operational impact
- Affected business services

##

### 9.4 Scheduling

Approved changes are added to the change calendar.

Scheduling considerations:
- Maintenance windows
- Operational impact
- Staffing availability
- Overlapping changes
- Vendor coordination

##

### 9.5 Implementation

Implementation activities must:
- Follow documented procedures
- Maintain communication with stakeholders
- Document deviations
- Track implementation timestamps

##

### 9.6 Validation & Closure

Following implementation:
- Services must be validated
- Rollback assessed if issues occur
- Documentation updated
- Final outcome recorded

---

### 10. Normal Change Process

```text
Identify need
↓
Submit Change Request Form (below)
↓
IT Manager Initial Review (24 hours)
↓
CAB Review (if required) — Tuesday meeting
↓
Authorized?
├── Yes → Schedule on Change Schedule → Implement → Update CMDB → PIR → Close
└── No  → Return to Requester with Feedback
```

---

### 11. Standard Change Process

```text
Identify need
↓
Verify it is on the Standard Change Register
↓
Follow Documented Procedure
↓
Update CMDB
↓
Close Ticket
```

##

### Standard Change Register

| Change ID | Description | Procedure Reference | Owner |
|:----------|:------------|:--------------------|:------|
| SC-001 | Password Reset | Service Request Catalogue — Cat 1 | Service Desk |
| SC-002 | Account Unlock | Service Request Catalogue — Cat 1 | Service Desk |
| SC-003 | Standard Software Install | Software Install SOP | Service Desk |
| SC-004 | Distribution Group Update | Email Admin SOP | Service Desk |
| SC-005 | Printer Configuration | Printer Setup SOP | Service Desk |
| SC-006 | Routine Endpoint Patching | Patch Management SOP | Senior IT Analyst |
| SC-007 | Teams Channel Creation | M365 Admin SOP | Service Desk |

---

### 12. Emergency Change Process

Emergency changes follow an accelerated process.

```text
Critical Issue Identified
↓
Immediate IT Manager Notification
↓
Emergency CAB Notification
↓
Rapid Risk Assessment
↓
Authorized?
├── Yes → Immediate Implemention → Document Retrospectively → PIR within 48 hours
└── No  → Escalate / Alternative Approach
↓
Documentation Completion
```

**Note:** Retrospective documentation must include: approval evidence, implementation timestamps, rollback assessment, affected systems, and post-implementation validation results. Documentation must be completed within 24 hours of implementation.

---

### 13. Sample Change Schedule

| Change ID | Description | Type | Scheduled Date | Owner | Status |
|:----------|:------------|:-----|:---------------|:------|:-------|
| CHG-010 | CRM Application Update | Normal | 2026-01-14 | Senior Analyst | Completed |
| CHG-011 | Monthly Endpoint Patching | Standard | 2026-01-14 | Senior Analyst | Completed |
| CHG-012 | VPN Gateway Upgrade | Normal | 2026-01-28 | IT Manager | Scheduled |
| CHG-015 | Printer Static IP Assignment | Normal | 2026-01-22 | Senior Analyst | Completed |
| CHG-017 | Conditional Access Review Controls | Normal | 2026-02-04 | IT Manager | Pending CAB |

---

### 14. Change Documentation Requirements

All changes must document:
- Implementation timestamps
- Approvers
- Affected services
- Implementation results
- Rollback actions (if applicable)
- Lessons learned

---

### 15. Rollback Planning

Every non-standard change must include a rollback plan.

Rollback plans should define:
- Restoration steps
- Responsible personnel
- Estimated recovery time
- Validation requirements

Changes without rollback capability may require:
- Additional CAB review
- Maintenance window restrictions
- Executive approval

---

### 16. Post-Implementation Review (PIR)

PIRs evaluate:
- Implementation success
- Unexpected issues
- SLA impact
- Lessons learned
- Improvement opportunities

##

### PIR Required For

| Scenario | PIR Required |
|:---------|:-------------|
| Emergency Changes | Yes |
| Failed Changes | Yes |
| High-Risk Changes | Yes |
| Major Service Impact | Yes |

---

### 17. Failed Change Handling

A change is classified as failed when:
- Rollback required
- Unexpected outage occurs
- Service degradation persists
- Implementation objectives not achieved

Failed changes may trigger:
- Incident records
- Problem investigations
- Process review

---

### 18. Security & Compliance Considerations

Changes affecting:
- Identity systems
- Authentication controls
- VPN infrastructure
- Security policies
- Privileged access

Must:
- Maintain audit traceability
- Include documented approval
- Follow least privilege principles
- Preserve logging integrity

---

### 19. Relationship to Other Processes

| Process | Relationship |
|:--------|:-------------|
| Incident Management | Failed changes may generate incidents |
| Problem Management | Permanent fixes often require changes |
| Continual Improvement | PIR findings drive process improvements |
| Knowledge Management | Procedures documented for reuse |

---

### 20. Continual Improvement Integration

Change metrics reviewed monthly include:
- Change success rate
- Failed change percentage
- Emergency change frequency
- Rollback occurrences
- CAB effectiveness

Improvement opportunities may include:
- Automation
- Improved testing
- Better rollback procedures
- Enhanced scheduling coordination

---

### 21. Success Metrics

| Metric | Baseline | Target | Measurement Frequency |
|:-------|:---------|:-------|:----------------------|
| Change success rate | 88% | >95% | Monthly |
| Failed change rate | 12% | <5% | Monthly |
| Emergency change frequency | 3 per month | <1 per month | Monthly |
| Rollback rate | 8% of changes | <3% | Monthly |
| PIR completion rate | Not tracked | 100% of required PIRs | Per change |
| Standard change as % of total | Not tracked | >60% | Monthly |

---

### 22. ITIL v4 Guiding Principles Applied

| Principle | Application |
|:----------|:------------|
| Focus on Value | Changes implemented to improve operational capability |
| Keep It Simple and Practical | Standard changes (pre-approved) reduce unnecessary overhead |
| Collaborate and Promote Visibility | CAB provides operational transparency - prevent conflict |
| Progress Iteratively with Feedback | PIR findings after every normal / emergency change improves future changes |
| Optimize and Automate | Repeatable changes standardized wherever possible - repeatable and efficient |

---

### 23. Related Documents

- Incident Management Process  — failed changes that cause incidents trigger incident procedures
- Service Request Catalogue  — standard changes originate from catalogue requests
- SLA & OLA Document  — change targets must align with SLA commitments
- Problem Management Register  — resolved problems generate change requests for permanent fixes
- Continual Improvement Register  — PIR findings drive CIR entries
- Service Configuration Management — CMDB updated after every implemented change


---

### 24. Change Log

| Version | Date | Author | Changes |
|:--------|:-----|:-------|:--------|
| 1.0 | January 2026 | IT Manager | Initial procedure — change types, CAB structure, standard change register |
| 1.1 | February 2026 | IT Manager | Added rollback planning section, failed change handling, security and compliance controls, PIR requirements table, emergency change process flow |

---
