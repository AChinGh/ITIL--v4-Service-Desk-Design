# Ticket Samples Repository  
### Richmond Solutions Inc. — IT Service Management

**Document Version:** 1.1  

**Last Updated:** 2026  

**Owner:** Service Desk Team  

**Practice Area:** Incident Management, Service Request Management, Knowledge Management  

---

### 1. Purpose

The purpose of this repository is to provide realistic sample IT service tickets demonstrating operational workflows used by the Richmond Solutions service desk.

These ticket examples demonstrate:

- Incident Logging  
- Prioritization  
- Troubleshooting Documentation  
- Escalation Procedures  
- Resolution Tracking  
- SLA Awareness  
- Service Request Fulfillment  
- User Communication Standards  

The ticket repository supports operational consistency and knowledge transfer across the IT support function.

---

### 2. Scope

This repository includes examples of:

- Incident Tickets  
- Service Requests  
- Access Requests  
- Hardware Requests  
- Escalated Incidents  
- Major Incident Communications  
- Password Reset Requests  
- VPN Support Cases  
- Printer Support Tickets  

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
| P1 — Critical | Organization-wide outage | 15 Minutes | 4 Hours |
| P2 — High | Department-wide impact | 30 Minutes | 8 Hours |
| P3 — Medium | Multiple users affected | 2 Hours | 24 Hours |
| P4 — Low | Single user impact | 4 Hours | 72 Hours |

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
| Reported By | Finance Department User |
| Date Opened | 2026-01-08 09:14 EST |
| Assigned Group | Service Desk |
| Escalated To | Senior IT Analyst |

##

### User Description

User reports VPN disconnecting repeatedly during Microsoft Teams meetings while working remotely.

##

### Investigation Notes

- Confirmed internet connection stable  
- Reproduced issue during Teams video call  
- Identified VPN tunnel drops during high bandwidth usage  
- Reviewed VPN gateway utilization metrics  
- Observed gateway bandwidth saturation during peak hours  

##

### Resolution

Temporary workaround provided:

- Reduced Teams video quality  
- Reconnected VPN session  
- Escalated issue to Problem Management for root cause analysis  

Problem record raised:

- PRB-001 — VPN Gateway Capacity Issue  

##

### Validation

- User confirmed stable VPN connection after workaround  
- No disconnect observed during 30-minute monitoring period  

##

### Closure Notes

Ticket linked to existing problem investigation and closed after user confirmation.

##

### INC-2026-0067 — Microsoft Teams Microphone Failure

| Field | Value |
|:------|:------|
| Ticket Type | Incident |
| Priority | P3 — Medium |
| Status | Resolved |
| Reported By | HR Department |
| Date Opened | 2026-01-14 10:22 EST |
| Assigned Group | Service Desk |

##

### User Description

User unable to use microphone during Microsoft Teams meetings. Audio output functional but microphone not detected.

##

### Investigation Notes

- Confirmed headset connected correctly  
- Verified microphone muted in Teams settings  
- Reviewed operating system sound configuration  
- Tested alternate USB port  
- Performed Teams test call  

##

### Resolution

- Correct microphone device selected in Teams  
- Teams application restarted  
- Test call successful  

Knowledge article referenced:

- KB-002 — Microsoft Teams Microphone Troubleshooting  

##

### Validation

- User confirmed audio functionality restored  
- Teams test call completed successfully  

##

### SR-2026-0021 — Password Reset Request

| Field | Value |
|:------|:------|
| Ticket Type | Service Request |
| Priority | Standard |
| Status | Completed |
| Requested By | Marketing Department User |
| Date Opened | 2026-01-15 08:40 EST |
| Assigned Group | Service Desk |

##

### Request Description

User unable to access corporate account after password expiration.

##

### Fulfillment Actions

- Verified user identity  
- Reset password in identity platform  
- Forced password change at next login  
- Confirmed MFA enrollment active  

Knowledge article referenced:

- KB-001 — Password Reset Procedure  

##

### Validation

- User successfully logged into workstation  
- User confirmed email access restored  

##

### SR-2026-0034 — New User Onboarding Request

| Field | Value |
|:------|:------|
| Ticket Type | Service Request |
| Priority | High |
| Status | Completed |
| Requested By | HR Department |
| Date Opened | 2026-01-18 14:10 EST |
| Assigned Group | Service Desk |

##

### Request Description

New employee onboarding request for Finance Department staff member starting 2026-01-22.

##

### Provisioning Tasks Completed

- Created Microsoft Entra ID account  
- Assigned Microsoft 365 license  
- Configured MFA enrollment  
- Assigned corporate laptop  
- Applied security baseline image  
- Joined device to domain  
- Configured Teams access  
- Assigned Finance shared drive permissions  
- Installed department applications  

##

### Validation

- Successful workstation login confirmed  
- Mailbox verified operational  
- User received onboarding instructions  

Related process:

- User Onboarding Workflow & Procedure  

##

### INC-2026-0091 — Major Email Service Outage

| Field | Value |
|:------|:------|
| Ticket Type | Major Incident |
| Priority | P1 — Critical |
| Status | Resolved |
| Reported By | Automated Monitoring Alert |
| Date Opened | 2026-01-31 08:02 EST |
| Assigned Group | IT Operations |
| Escalated To | IT Manager |

##

### Incident Description

Organization-wide email outage affecting approximately 150 users.

##

### Major Incident Actions

- Major Incident declared at 08:10 EST  
- Emergency bridge call initiated  
- User communication updates issued every 30 minutes  
- Microsoft 365 admin audit logs reviewed  
- Conditional access policy rollback performed  

##

### Root Cause

Incorrect conditional access policy deployment blocked user authentication.

##

### Resolution

- Reverted failed policy configuration  
- Restored authentication services  
- Validated mailbox connectivity across departments  

Problem record linked:

- PRB-004 — Email Service Outage RCA  

Change record linked:

- CHG-017 — M365 Change Control Improvements  

##

### Validation

- Email access restored for all users  
- Monitoring alerts cleared  
- User confirmation received from department representatives  

---

### 7. Ticket Documentation Standards

All service tickets must include:

- Accurate Categorization  
- Clear User Description  
- Troubleshooting Steps  
- Escalation Actions  
- Resolution Details  
- Validation Confirmation  
- Linked Problems Or Changes (If Applicable)  

Tickets must avoid:

- Vague Technical Notes  
- Missing Resolution Details  
- Unverified Closures  
- Incomplete Escalation Documentation  

---

### 8. SLA Alignment

Ticket handling activities align with the Richmond Solutions SLA targets for:

- Response Times  
- Resolution Targets  
- Escalation Procedures  
- Major Incident Communication Standards  

---

### 9. Related Documents

- Incident Management Process  
- Service Request Catalogue  
- SLA & OLA Document  
- Problem Management Register  
- Change Management Procedure  
- Continual Improvement Register  
- Knowledge Management Practice  
- User Onboarding Workflow & Procedure  

---

### 10. ITIL v4 Guiding Principles Applied

| Guiding Principle | Application |
|:------------------|:------------|
| Focus on Value | Ticket workflows prioritize rapid restoration of user productivity |
| Keep It Simple And Practical | Standardized ticket templates ensure consistent documentation |
| Collaborate And Promote Visibility | Escalations and linked records improve operational transparency |
| Progress Iteratively With Feedback | Ticket trends contribute to continual improvement initiatives |
| Start Where You Are | Ticket processes built from common operational support scenarios |

---

