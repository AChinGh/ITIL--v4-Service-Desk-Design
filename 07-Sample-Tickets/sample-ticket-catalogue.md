# Ticket Samples Repository

### Richmond Solutions Inc. — IT Service Management

**Document Version:** 1.2  

**Last Updated:** 2026  

**Owner:** Service Desk Team  

**Practice Area:** Incident Management, Service Request Management, Knowledge Management

---

### 1. Purpose

The purpose of this repository is to provide realistic sample IT service 
tickets demonstrating operational workflows used by the Richmond Solutions 
service desk.

These ticket examples demonstrate:
- Incident logging
- Prioritization
- Troubleshooting documentation
- Escalation procedures
- Resolution tracking
- SLA awareness
- Service request fulfilment
- User communication standards

The ticket repository supports operational consistency and knowledge transfer 
across the IT support function.

---

### 2. Scope

This repository includes examples of:
- Incident tickets (P1–P4)
- Service requests
- Access requests
- Hardware requests
- Escalated incidents
- Major incident communications
- Password reset requests
- VPN support cases
- Printer support tickets

All tickets are fictional and created for portfolio and training purposes only.

---

### 3. Ticket Classification Standards

| Ticket Type | Description |
|:------------|:------------|
| Incident | Unplanned interruption or degradation of service |
| Service Request | Standard pre-approved user request |
| Problem | Root cause investigation linked to recurring incidents |
| Change | Authorized modification to infrastructure or services |
| Major Incident | High-impact outage affecting business operations |

---

### 4. Priority Matrix

| Priority | Description | Response Target | Resolution Target |
|:---------|:------------|:----------------|:------------------|
| P1 — Critical | Organization-wide outage | 15 minutes | 4 hours |
| P2 — High | Department-wide impact | 30 minutes | 8 hours |
| P3 — Medium | Multiple users affected | 2 hours | 24 hours |
| P4 — Low | Single user impact | 4 hours | 72 hours |

---

### 5. Ticket Lifecycle

```text
Ticket Logged
↓
Categorization
↓
Prioritization
↓
Assignment
↓
Investigation
↓
Resolution
↓
Validation
↓
Closure
```

---

### 6. Sample Incident Tickets

### INC-2026-0041 — VPN Disconnect During Teams Calls

| Field | Value |
|:------|:------|
| Ticket Type | Incident |
| Priority | P2 — High |
| Status | Resolved |
| Reported By | Finance department user |
| Date Opened | 2026-01-08 09:14 EST |
| Assigned Group | Service Desk |
| Escalated To | Senior IT Analyst |

**User Description**

User reports VPN disconnecting repeatedly during Microsoft Teams meetings 
while working remotely.

**Investigation Notes**

- Confirmed internet connection stable
- Reproduced issue during Teams video call
- Identified VPN tunnel drops during high bandwidth usage
- Reviewed VPN gateway utilization metrics
- Observed gateway bandwidth saturation during peak hours

**Resolution**

Temporary workaround provided:

- Reduced Teams video quality to lower bandwidth demand
- Reconnected VPN session
- Escalated issue to Problem Management for root cause analysis

Problem record raised: **PRB-001 — VPN Gateway Capacity Issue**

**Validation**

- User confirmed stable VPN connection after workaround
- No disconnect observed during 30-minute monitoring period

**SLA Performance**

| Target | Actual |
|:-------|:-------|
| Response: 30 minutes | Responded within 20 minutes ✓ |
| Resolution: 8 hours | Workaround applied within 2 hours ✓ |

**Closure Notes**

Ticket linked to existing problem investigation and closed after user 
confirmation. Root cause investigation continues under PRB-001.

##

### INC-2026-0067 — Microsoft Teams Microphone Failure

| Field | Value |
|:------|:------|
| Ticket Type | Incident |
| Priority | P3 — Medium |
| Status | Resolved |
| Reported By | HR department |
| Date Opened | 2026-01-14 10:22 EST |
| Assigned Group | Service Desk |

**User Description**

User unable to use microphone during Microsoft Teams meetings. Audio output 
functional but microphone not detected.

**Investigation Notes**

- Confirmed headset connected correctly
- Verified microphone not muted in Teams settings
- Reviewed operating system sound configuration
- Tested alternate USB port
- Performed Teams test call

**Resolution**

- Correct microphone device selected in Teams audio settings
- Teams application restarted
- Test call completed successfully

Knowledge article referenced: **KB-002 — Microsoft Teams Microphone 
Troubleshooting**

**Validation**

- User confirmed audio functionality restored
- Teams test call completed successfully

**SLA Performance**

| Target | Actual |
|:-------|:-------|
| Response: 2 hours | Responded within 45 minutes ✓ |
| Resolution: 24 hours | Resolved within 2 hours ✓ |

**Closure Notes**

Isolated incident — no recurrence identified at time of closure. No problem 
record raised. If similar incidents recur across multiple users, a problem 
record will be raised for root cause investigation.

##

### INC-2026-0078 — Printer Offline — Floor 2 (Monday Morning)

| Field | Value |
|:------|:------|
| Ticket Type | Incident |
| Priority | P3 — Medium |
| Status | Resolved |
| Reported By | Operations department user |
| Date Opened | 2026-01-20 08:06 EST |
| Assigned Group | Service Desk |

**User Description**

Both network printers on Floor 2 are offline. Staff unable to print. 
Issue reported at start of business Monday morning.

**Investigation Notes**

- Confirmed printers offline via network monitoring
- Verified network switch connectivity on Floor 2
- Identified DHCP lease renewal failure on printer network interfaces
- Confirmed issue does not affect other floors
- Reviewed previous incidents — eighth consecutive Monday occurrence

**Resolution**

- Manual printer restart performed by service desk analyst
- Printer connectivity validated before business hours
- Both printers confirmed online at 08:22 EST

Problem record referenced: **PRB-003 — Floor 2 Printer Monday Offline Issue**

**Validation**

- Test print confirmed on both Floor 2 printers
- User confirmed printing restored

**SLA Performance**

| Target | Actual |
|:-------|:-------|
| Response: 2 hours | Proactively resolved before user impact ✓ |
| Resolution: 24 hours | Resolved within 20 minutes of business open ✓ |

**Closure Notes**

Workaround applied — proactive Monday restart. Permanent fix pending under 
CHG-015 — Printer Static IP Assignment. Problem investigation continues 
under PRB-003.

##

### INC-2026-0112 — Application Access After Role Change

| Field | Value |
|:------|:------|
| Ticket Type | Incident |
| Priority | P4 — Low |
| Status | Resolved |
| Reported By | Sales department user |
| Date Opened | 2026-02-03 14:35 EST |
| Assigned Group | Service Desk |

**User Description**

User recently transferred from Marketing to Sales department. Unable to 
access CRM reporting module. Receiving "Access Denied" error. Previously 
had access in Marketing role.

**Investigation Notes**

- Confirmed user role updated in HR system to Sales
- Reviewed current CRM permissions — user retains Marketing role group
- Marketing role group does not include CRM reporting module access
- Sales role group includes CRM reporting access
- Confirmed no active change request for role transition access update

**Resolution**

- Removed user from Marketing role group in Microsoft Entra ID
- Added user to Sales role group
- CRM reporting module access confirmed
- Audit log entry recorded for access change

**Validation**

- User confirmed CRM reporting access restored
- Access verified against approved Sales role permissions matrix

**SLA Performance**

| Target | Actual |
|:-------|:-------|
| Response: 4 hours | Responded within 1 hour ✓ |
| Resolution: 72 hours | Resolved within 3 hours ✓ |

**Closure Notes**

Access corrected in line with least privilege principles. Role transition 
access updates to be included in future offboarding/transfer checklist — 
improvement opportunity logged for CIR review.

##

### INC-2026-0091 — Major Email Service Outage

| Field | Value |
|:------|:------|
| Ticket Type | Major Incident |
| Priority | P1 — Critical |
| Status | Resolved |
| Reported By | Automated monitoring alert |
| Date Opened | 2026-01-31 08:02 EST |
| Assigned Group | IT Operations |
| Escalated To | IT Manager |
| Incident Lead | IT Manager |
| Communications Lead | Senior IT Analyst |

**Incident Description**

Organization-wide email outage affecting approximately 150 users. 
Microsoft 365 authentication failure preventing access to all cloud services.

**Major Incident Actions**

- Major incident declared at 08:10 EST
- Emergency bridge call initiated at 08:15 EST
- User communications issued every 30 minutes
- Microsoft 365 admin audit logs reviewed
- Conditional access policy rollback performed

**Major Incident Communications Log**

| Time | Update |
|:-----|:-------|
| 08:10 EST | Major incident declared — investigation underway |
| 08:30 EST | Root cause identified — conditional access policy under review |
| 09:00 EST | Rollback in progress — estimated restoration 09:30 EST |
| 09:28 EST | Services restored — validation underway |
| 09:45 EST | All services confirmed restored — incident resolved |

**Sample User Communication — 08:30 EST**

**To:** All Staff  

**From:** IT Manager  

**Subject:** [ACTIVE — IT INCIDENT] Email Service Disruption  

We are currently investigating an issue affecting email and Microsoft 365 access for all Richmond Solutions staff.

**Current Status:** Root cause identified — fix in progress  

**Impact:** All staff — email and Microsoft 365 authentication  

**Next Update:** 09:00 EST  

We apologize for the disruption and will provide updates every 30 minutes until resolved.

IT Support Team  

itsupport@richmondsolutions.ca | Extension 100

**Root Cause**

Incorrect conditional access policy deployment blocked user authentication 
across all Microsoft 365 services.

**Resolution**

- Reverted failed conditional access policy configuration
- Restored previous authentication ruleset
- Validated mailbox connectivity across all departments

Problem record linked: **PRB-004 — Email Service Outage RCA**  
Change record linked: **CHG-017 — M365 Change Control Improvements**

**Validation**

- Email access restored for all 150 users
- Monitoring alerts cleared
- User confirmation received from department representatives

**SLA Performance**

| Target | Actual |
|:-------|:-------|
| Response: 15 minutes | IT Manager notified within 8 minutes ✓ |
| Resolution: 4 hours | Service restored in 1 hour 26 minutes ✓ |
| Comms every 30 minutes | 5 updates issued on schedule ✓ |

**Post-Incident Review**

PIR scheduled within 48 hours. Problem record PRB-004 raised. 
Change CHG-017 submitted to prevent recurrence.

---

### 7. Sample Service Request Tickets

### SR-2026-0021 — Password Reset Request

| Field | Value |
|:------|:------|
| Ticket Type | Service Request |
| Priority | Standard |
| Status | Completed |
| Requested By | Marketing department user |
| Date Opened | 2026-01-15 08:40 EST |
| Assigned Group | Service Desk |

**Request Description**

User unable to access corporate account after password expiration.

**Fulfilment Actions**

- Verified user identity via security questions
- Reset password in Microsoft Entra ID
- Forced password change at next login
- Confirmed MFA enrollment active

Knowledge article referenced: **KB-001 — Password Reset Procedure**

**Validation**

- User successfully logged into workstation
- User confirmed email access restored

**SLA Performance**

| Target | Actual |
|:-------|:-------|
| Acknowledgement: 1 hour | Acknowledged within 15 minutes ✓ |
| Fulfilment: 1 business hour | Completed within 30 minutes ✓ |

**Closure Notes**

Standard request completed. Self-service password reset (CIR-001) will eliminate this ticket type upon implementation.

##

### SR-2026-0034 — New User Onboarding Request

| Field | Value |
|:------|:------|
| Ticket Type | Service Request |
| Priority | Urgent |
| Status | Completed |
| Requested By | HR department |
| Date Opened | 2026-01-18 14:10 EST |
| Assigned Group | Service Desk |
| Start Date | 2026-01-22 |

**Request Description**

New employee onboarding request for Finance department staff member 
starting 2026-01-22.

**Provisioning Tasks Completed**

- ✓ Created Microsoft Entra ID account
- ✓ Assigned Microsoft 365 licence
- ✓ Configured MFA enrollment
- ✓ Assigned corporate laptop from asset pool
- ✓ Applied security baseline image
- ✓ Joined device to domain
- ✓ Configured Teams access
- ✓ Assigned Finance shared drive permissions
- ✓ Installed department applications
- ✓ Sent welcome instructions to user

**Validation**

- Successful workstation login confirmed
- Mailbox verified operational
- User received onboarding instructions before start date

Related process: **User Onboarding Workflow & Procedure**

**SLA Performance**

| Target | Actual |
|:-------|:-------|
| Acknowledgement: 2 hours | Acknowledged within 1 hour ✓ |
| Fulfilment: Before start date | All tasks completed 2026-01-21 ✓ |

##

### SR-2026-0055 — Application Access Request

| Field | Value |
|:------|:------|
| Ticket Type | Service Request |
| Priority | Standard |
| Status | Completed |
| Requested By | Sales Manager (on behalf of staff member) |
| Date Opened | 2026-01-25 11:20 EST |
| Assigned Group | Service Desk |
| Approval Status | Manager approved — 2026-01-25 11:45 EST |

**Request Description**

Sales Manager requesting CRM application access for a new Sales department 
team member. User currently has standard Microsoft 365 access only.

**Approval Verification**

- Manager approval confirmed via service portal
- User role verified as Sales Representative
- CRM access appropriate for role — confirmed against role access matrix
- Request does not exceed standard Sales role permissions
- Least privilege principles applied — read/write access granted, 
  no admin permissions

**Fulfilment Actions**

- Added user to CRM Sales role group in Microsoft Entra ID
- Confirmed CRM licence available in tenant
- Assigned CRM licence to user account
- Tested user login to CRM application
- Audit log entry recorded

**Validation**

- User confirmed CRM access functional
- Manager notified of completion
- Access verified against approved Sales role permissions matrix

**SLA Performance**

| Target | Actual |
|:-------|:-------|
| Acknowledgement: 1 hour | Acknowledged within 30 minutes ✓ |
| Fulfilment: 1 business day | Completed within 4 hours of approval ✓ |

**Closure Notes**

Access granted in line with least privilege principles. Manager approval 
documented and retained for audit purposes.

##

### SR-2026-0071 — Laptop Replacement Request

| Field | Value |
|:------|:------|
| Ticket Type | Service Request |
| Priority | Standard |
| Status | Completed |
| Requested By | Operations Manager (on behalf of staff member) |
| Date Opened | 2026-02-01 09:15 EST |
| Assigned Group | Service Desk |
| Approval Status | Manager approved — 2026-02-01 09:30 EST |

**Request Description**

Operations department staff member's laptop is failing — screen flickering 
intermittently and battery no longer holding charge. Laptop is 4 years old 
and beyond warranty. Manager requesting replacement.

**Assessment**

- Device age confirmed: 4 years — meets replacement eligibility criteria
- Hardware fault confirmed: screen and battery failure
- Asset register updated — device status changed to "End of Life"
- Replacement laptop available in asset pool

**Fulfilment Actions**

- Assigned replacement laptop from asset pool
- Applied standard corporate security baseline image
- Joined device to domain
- Transferred user profile and data from old device
- Installed department-standard applications
- Encrypted hard drive on failed device before disposal
- Asset register updated — new device assigned to user
- Failed device logged for secure disposal

**Validation**

- User confirmed all data accessible on new device
- Applications confirmed functional
- Workstation login successful

**SLA Performance**

| Target | Actual |
|:-------|:-------|
| Acknowledgement: 1 hour | Acknowledged within 30 minutes ✓ |
| Fulfilment: 3 business days | Completed same business day ✓ |

**Closure Notes**

Failed device quarantined for secure data destruction before disposal in 
line with IT Asset Management policy. Asset register updated.

---

### 8. SLA Alignment

All tickets in this repository demonstrate compliance with Richmond Solutions 
SLA targets.

| Ticket | Type | Priority | Response Target | Response Achieved | Resolution Target | Resolution Achieved |
|:-------|:-----|:---------|:----------------|:------------------|:------------------|:--------------------|
| INC-2026-0041 | Incident | P2 | 30 minutes | 20 minutes ✓ | 8 hours | 2 hours (workaround) ✓ |
| INC-2026-0067 | Incident | P3 | 2 hours | 45 minutes ✓ | 24 hours | 2 hours ✓ |
| INC-2026-0078 | Incident | P3 | 2 hours | Proactive ✓ | 24 hours | 20 minutes ✓ |
| INC-2026-0112 | Incident | P4 | 4 hours | 1 hour ✓ | 72 hours | 3 hours ✓ |
| INC-2026-0091 | Major Incident | P1 | 15 minutes | 8 minutes ✓ | 4 hours | 1h 26min ✓ |
| SR-2026-0021 | Service Request | Standard | 1 hour | 15 minutes ✓ | 1 business hour | 30 minutes ✓ |
| SR-2026-0034 | Service Request | Urgent | 2 hours | 1 hour ✓ | Before start date | Completed day before ✓ |
| SR-2026-0055 | Service Request | Standard | 1 hour | 30 minutes ✓ | 1 business day | 4 hours ✓ |
| SR-2026-0071 | Service Request | Standard | 1 hour | 30 minutes ✓ | 3 business days | Same day ✓ |

---

### 9. Ticket Documentation Standards

All service tickets must include:
- Accurate categorization
- Clear user description
- Troubleshooting steps
- Escalation actions
- Resolution details
- Validation confirmation
- Linked problems or changes where applicable

Tickets must avoid:
- Vague technical notes
- Missing resolution details
- Unverified closures
- Incomplete escalation documentation

---

### 10. Success Metrics

| Metric | Standard | Purpose |
|:-------|:---------|:--------|
| Ticket categorization accuracy | 100% correct category assigned | Supports trend analysis |
| Resolution documented on closure | 100% of tickets | Enables knowledge reuse |
| Linked problem or change records | 100% where applicable | Maintains traceability |
| User validation before closure | 100% of P1/P2 incidents | Confirms service restoration |
| SLA response compliance | >98% of tickets | Reflects SLA performance |
| Audit log entry for access changes | 100% of access tickets | Supports compliance and IAM |

---

### 11. ITIL v4 Guiding Principles Applied

| Guiding Principle | Application |
|:------------------|:------------|
| Focus on Value | Ticket workflows prioritize rapid restoration of user productivity |
| Keep It Simple and Practical | Standardized ticket templates ensure consistent documentation |
| Collaborate and Promote Visibility | Escalations and linked records improve operational transparency |
| Progress Iteratively with Feedback | Ticket trends contribute to continual improvement initiatives |
| Start Where You Are | Ticket processes built from common operational support scenarios |

---

### 12. Related Documents

- Incident Management Process
- Service Request Catalogue
- SLA & OLA Document
- Problem Management Register
- Change Management Procedure
- Continual Improvement Register
- Knowledge Management Practice
- User Onboarding Workflow & Procedure

---

### Change Log

| Version | Date | Author | Changes |
|:--------|:-----|:-------|:--------|
| 1.0 | January 2026 | Service Desk Team | Initial repository — INC-2026-0041, SR-2026-0021, INC-2026-0091 |
| 1.1 | February 2026 | Service Desk Team | Added INC-2026-0067, SR-2026-0034, documentation standards, SLA alignment section |
| 1.2 | February 2026 | Service Desk Team | Added INC-2026-0078 (printer), INC-2026-0112 (P4 role change), SR-2026-0055 (access request), SR-2026-0071 (hardware request), major incident comms log, SLA compliance table, success metrics section |
