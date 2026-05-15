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

# 2. Scope

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

# 3. Definition of a Change

A **change** is the addition, modification, or removal of anything that could directly or indirectly affect IT services.

Examples include:
- Software deployment
- Network configuration updates
- Policy modifications
- VPN upgrades
- Server maintenance
- Identity and access changes

---

# 4. Change Objectives

The Change Management process aims to:
- Assess implementation risk
- Ensure proper authorization
- Maintain operational visibility
- Reduce change-related incidents
- Support rollback capability
- Improve implementation consistency

---

# 5. Change Types

---

## 5.1 Standard Change

Standard changes are:
- Low risk
- Repeatable
- Pre-approved
- Well documented

No CAB review is required.

### Examples
- Password resets
- Account unlocks
- Approved software installation
- Distribution group updates
- Routine printer configuration

---

## 5.2 Normal Change

Normal changes require:
- Risk assessment
- Implementation planning
- Formal authorization

Higher-risk changes require CAB review.

### Examples
- Organization-wide software deployment
- Firewall rule modifications
- VPN configuration changes
- Conditional access policy updates
- Server configuration changes

---

## 5.3 Emergency Change

Emergency changes are implemented rapidly to:
- Restore service
- Mitigate security threats
- Prevent major business impact

Emergency CAB approval is required before implementation whenever possible.

### Examples
- Critical vulnerability patching
- Outage recovery changes
- Emergency rollback actions
- Active security incident remediation

---

# 6. Change Authority Matrix

| Change Type | Authorization Required |
|---|---|
| Standard Change | Pre-approved |
| Normal Change (Low Risk) | IT Manager |
| Normal Change (High Risk) | CAB Approval |
| Emergency Change | Emergency CAB |

---

# 7. Change Advisory Board (CAB)

The CAB reviews high-risk changes before implementation.

## CAB Members

| Role | Responsibility |
|---|---|
| IT Manager | CAB Chair |
| Senior IT Analyst | Technical Review |
| Department Representative | Business Impact Review |
| Vendor Representative | External System Review (if required) |

---

## CAB Schedule

| Activity | Schedule |
|---|---|
| Standard CAB Meeting | Tuesdays — 10:00 AM EST |
| Emergency CAB | As required |

---

# 8. Change Lifecycle

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

# 9. Change Process Workflow

---

## 9.1 Change Submission

All non-standard changes must include:
- Business justification
- Affected systems
- Implementation plan
- Rollback procedure
- Risk assessment
- Testing details

---

## 9.2 Risk Assessment

Risk is evaluated based on:
- Service criticality
- Number of users affected
- Security impact
- Implementation complexity
- Rollback feasibility

---

## 9.3 Authorization

Changes must receive approval before implementation.

Authorization depends on:
- Risk level
- Operational impact
- Affected business services

---

## 9.4 Scheduling

Approved changes are added to the change calendar.

Scheduling considerations:
- Maintenance windows
- Operational impact
- Staffing availability
- Overlapping changes
- Vendor coordination

---

## 9.5 Implementation

Implementation activities must:
- Follow documented procedures
- Maintain communication with stakeholders
- Document deviations
- Track implementation timestamps

---

## 9.6 Validation & Closure

Following implementation:
- Services must be validated
- Rollback assessed if issues occur
- Documentation updated
- Final outcome recorded

---

# 10. Emergency Change Process

Emergency changes follow an accelerated process.

```text
Critical Issue Identified
↓
Emergency CAB Notification
↓
Rapid Risk Assessment
↓
Authorization
↓
Immediate Implementation
↓
Post-Implementation Review
↓
Documentation Completion
```

---

## Emergency Change Requirements

Even during emergency implementation:
- Approval evidence must be documented
- Rollback planning must exist
- PIR must occur within 48 hours

---

# 11. Standard Change Register

| Change ID | Description | Owner |
|---|---|---|
| SC-001 | Password Reset | Service Desk |
| SC-002 | Account Unlock | Service Desk |
| SC-003 | Standard Software Install | Service Desk |
| SC-004 | Distribution Group Update | Service Desk |
| SC-005 | Printer Configuration | Service Desk |
| SC-006 | Routine Endpoint Patching | Senior IT Analyst |
| SC-007 | Teams Channel Creation | Service Desk |

---

# 12. Sample Change Schedule

| Change ID | Description | Type | Scheduled Date | Status |
|---|---|---|---|---|
| CHG-010 | CRM Application Update | Normal | 2026-01-14 | Completed |
| CHG-011 | Monthly Endpoint Patching | Standard | 2026-01-14 | Completed |
| CHG-012 | VPN Gateway Upgrade | Normal | 2026-01-28 | Scheduled |
| CHG-015 | Printer Static IP Assignment | Normal | 2026-01-22 | Completed |
| CHG-017 | Conditional Access Review Controls | Normal | 2026-02-04 | Pending CAB |

---

# 13. Change Documentation Requirements

All changes must document:
- Implementation timestamps
- Approvers
- Affected services
- Implementation results
- Rollback actions (if applicable)
- Lessons learned

---

# 14. Rollback Planning

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

# 15. Post-Implementation Review (PIR)

PIRs evaluate:
- Implementation success
- Unexpected issues
- SLA impact
- Lessons learned
- Improvement opportunities

---

## PIR Required For

| Scenario | PIR Required |
|---|---|
| Emergency Changes | Yes |
| Failed Changes | Yes |
| High-Risk Changes | Yes |
| Major Service Impact | Yes |

---

# 16. Failed Change Handling

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

# 17. Security & Compliance Considerations

Changes affecting:
- Identity systems
- Authentication controls
- VPN infrastructure
- Security policies
- Privileged access

must:
- Maintain audit traceability
- Include documented approval
- Follow least privilege principles
- Preserve logging integrity

---

# 18. Relationship to Other Processes

| Process | Relationship |
|---|---|
| Incident Management | Failed changes may generate incidents |
| Problem Management | Permanent fixes often require changes |
| Continual Improvement | PIR findings drive process improvements |
| Knowledge Management | Procedures documented for reuse |

---

# 19. Continual Improvement Integration

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

# 20. ITIL v4 Guiding Principles Applied

| Principle | Application |
|---|---|
| Focus on Value | Changes implemented to improve operational capability |
| Keep It Simple and Practical | Standard changes reduce unnecessary overhead |
| Collaborate and Promote Visibility | CAB provides operational transparency |
| Progress Iteratively with Feedback | PIR findings improve future changes |
| Optimize and Automate | Repeatable changes standardized wherever possible |

---

# 21. Related Documents

- Incident Management Process  
- Service Request Catalogue  
- SLA & OLA Document  
- Problem Management Register  
- Continual Improvement Register  

---
