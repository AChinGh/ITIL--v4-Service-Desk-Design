# Knowledge Management Practice  
### Richmond Solutions Inc. — IT Service Management

**Document Version:** 1.1

**Last Updated:** 2026  

**Owner:** Service Desk Team  

**ITIL Practice Area:** Knowledge Management, Service Desk, Incident Management  

---

### 1. Purpose

The purpose of the Knowledge Management practice is to ensure operational knowledge is:
- Captured  
- Organized  
- Shared  
- Maintained  
- Reused Across IT Operations  

This practice supports:
- Faster Incident Resolution  
- Reduced Escalations  
- Improved First Contact Resolution  
- Operational Consistency  
- User Self-Service Support  

The objective is to ensure that valuable operational knowledge is retained within Northgate Solutions and can be reused efficiently by IT staff and end users.

---

### 2. Knowledge Management Model

Knowledge Management at Northgate Solutions follows the DIKW hierarchy:
- Data  
- Information  
- Knowledge  
- Wisdom  

Operational incident data is transformed into structured knowledge articles that improve decision-making, reduce resolution times, and preserve organizational learning.

Knowledge is stored within the Northgate Solutions Knowledge Management System (KMS), built on Microsoft SharePoint and integrated with the broader Service Knowledge Management System (SKMS), including:
- Incident Records  
- Problem Records  
- Change Records  
- Configuration Data (CMDB)  
- Knowledge Articles  
- Major Incident Reviews  

The KMS is accessible internally through the IT service portal and SharePoint knowledge site.

---

### 3. Scope

Knowledge articles may include:
- Troubleshooting Guides  
- Known Errors  
- Standard Operating Procedures  
- User Instructions  
- Service Request Guidance  
- Configuration Procedures  
- Escalation Instructions  
- Onboarding Documentation  
- Major Incident Review Findings  

This practice applies to all IT-supported systems and services at Northgate Solutions.

---

### 4. Knowledge Sources

Knowledge may originate from:
- Incident Resolution Activities  
- Problem Management Reviews  
- Major Incident Reviews  
- Vendor Documentation  
- Change Implementations  
- User Feedback  
- Trend Analysis  
- Continual Improvement Initiatives  
- Onboarding And Offboarding Activities  

Knowledge creation is considered part of normal operational work and is not treated as a separate documentation exercise.

---

### 5. Knowledge Lifecycle

| Stage | Owner | Activity |
|:------|:------|:---------|
| Create | Service Desk Analyst | Draft article from incident resolution, problem review, or major incident review |
| Review | Senior IT Analyst | Validate technical accuracy and troubleshooting steps |
| Approve | IT Manager | Confirm article meets operational and security standards |
| Publish | Service Desk Analyst | Publish article to SharePoint Knowledge Base and apply category tags |
| Maintain | Service Desk Team | Update article after process changes or quarterly review |
| Retire | IT Manager | Archive outdated articles no longer relevant to supported systems |

---

### 6. Knowledge Article Standards

All knowledge articles must include:
- Title  
- Symptoms  
- Affected Systems  
- Root Cause (If Known)  
- Resolution Steps  
- Validation Steps  
- Escalation Criteria  
- Related Services  
- Related Incidents Or Problems  
- Last Review Date  

Articles must:
- Use Clear Operational Language  
- Avoid Unnecessary Technical Jargon  
- Include Repeatable Troubleshooting Steps  
- Follow The Standard KB Template  
- Be Reviewed Quarterly For Accuracy  

---

### 7. Knowledge Base Categories

| Category | Examples |
|:---------|:---------|
| Authentication | Password Reset, MFA Enrollment |
| Collaboration | Teams Audio Issues, Shared Mailbox Access |
| Connectivity | VPN Troubleshooting, Network Access |
| Hardware | Printer Troubleshooting, Laptop Setup |
| Software | Application Errors, Software Installation |
| Security | Phishing Reporting, Endpoint Protection |
| Onboarding | New User Setup, Account Provisioning |

---

### 8. Roles & Responsibilities

| Role | Responsibility |
|:-----|:---------------|
| Service Desk Analyst | Create, update, and maintain knowledge articles |
| Senior IT Analyst | Review technical accuracy and approve troubleshooting procedures |
| IT Manager (Knowledge Manager) | Owns the Knowledge Management practice, standards, governance, and review process |
| All Staff | Submit knowledge gaps, documentation requests, and feedback through the service portal |

---

### 9. Knowledge Review Schedule

| Activity | Frequency |
|---|---|
| Knowledge Article Review | Quarterly |
| Outdated Article Audit | Semi-Annual |
| Major Incident Knowledge Update | After Each PIR |
| Knowledge Category Review | Quarterly |
| KB Template Review | Annually |

---

### 10. Success Metrics

| Metric | Baseline | Target |
|:-------|:---------|:-------|
| First Contact Resolution | 72% | >80% |
| Knowledge Usage Rate | Not currently tracked | Measured and increasing quarterly |
| Ticket Escalation Rate | 28% of tickets escalated | Reduce by 20% within 6 months |
| Repeat Incident Volume | Top 15 incidents recurring monthly | Reduce repeat incidents by 20% |

---

### 11. Related Documents
- Incident Management Process  
- Service Request Catalogue  
- SLA & OLA Document  
- Problem Management Register  
- Change Management Procedure  
- Continual Improvement Register  
- User Onboarding Workflow & Procedure  

---

### 12. ITIL v4 Guiding Principles Applied

| Guiding Principle | Application |
|:------------------|:------------|
| Focus on Value | Knowledge reuse reduces resolution time and restores user productivity faster |
| Start Where You Are | Articles are created from existing incident trends, problem records, and operational experience |
| Progress Iteratively with Feedback | Quarterly reviews and post-incident updates improve article quality continuously |
| Keep It Simple and Practical | Standardized templates ensure consistent and usable documentation |
| Collaborate and Promote Visibility | Knowledge base is accessible to all staff through the service portal |

---

### 13. Core Knowledge Articles

The following knowledge articles are maintained within the Northgate Solutions Knowledge Base:
- KB-001 — Password Reset Procedure  
- KB-002 — Microsoft Teams Microphone Troubleshooting  
- KB-003 — VPN Reconnect Checklist  
- KB-004 — Printer Offline Resolution SOP  

### KB-001 — Password Reset Procedure

### Symptoms

Users report:
- Incorrect Password  
- Account Locked  
- Sign-In Failure  
- MFA Prompt Loop  

### Resolution Steps

1. Verify user identity using internal verification procedure  
2. Open identity management console  
3. Locate user account  
4. Reset password to secure temporary value  
5. Force password change at next login  
6. Unlock account if required  
7. Confirm successful login with user  

### Validation Steps

- User Successfully Logs Into Workstation  
- User Successfully Accesses Email  
- MFA Authentication Completes Successfully  

### Escalation Criteria

Escalate if:
- Suspicious Login Activity Detected  
- MFA Device Unavailable Or Lost  
- Identity Verification Cannot Be Completed  

##

### KB-002 — Microsoft Teams Microphone Troubleshooting

### Symptoms

Users report:
- No Audio During Meetings  
- Microphone Not Detected  
- Audio Works In Other Applications But Not In Teams  
- Participants Cannot Hear User  

### Resolution Steps

1. Confirm microphone is not physically muted  
2. Check operating system sound settings  
3. Verify correct input device is selected  
4. Open Microsoft Teams settings  
5. Navigate to Devices section  
6. Select correct microphone input  
7. Run Teams test call feature  
8. Restart Teams if issue persists  

### Validation Steps

- Microphone Input Detected Successfully  
- Test Call Produces Audio  
- Other Participants Confirm Audio Quality  

### Escalation Criteria

Escalate if:
- Hardware Failure Suspected  
- Device Drivers Fail To Load  
- Microphone Not Detected By Operating System  

##

### KB-003 — VPN Reconnect Checklist

### Symptoms

Users report:
- VPN Disconnects During Sessions  
- Unable To Reconnect VPN  
- MFA Timeout Errors  
- Unstable Remote Access Connection  

### Resolution Steps

1. Confirm internet connectivity is available  
2. Disconnect VPN session fully  
3. Restart VPN client application  
4. Re-authenticate with corporate credentials  
5. Approve MFA request  
6. Verify IP assignment  
7. Attempt reconnect  
8. Restart workstation if issue persists  

### Validation Steps

- VPN Status Shows Connected  
- Internal Systems Accessible  
- Connection Remains Stable For 10 Minutes  

## Escalation Criteria

Escalate if:
- Multiple Users Affected Simultaneously  
- VPN Gateway Unreachable  
- Authentication Failures Continue After Reset  

## Related Systems

- Remote Access Gateway  
- Identity Authentication Services

##

### KB-004 — Printer Offline Resolution SOP

## Symptoms

Users report:
- Printer Offline Status  
- Print Jobs Stuck In Queue  
- Printer Unavailable On Network  
- Intermittent Print Failures  

### Resolution Steps

1. Confirm printer is powered on  
2. Verify network cable connectivity  
3. Check printer IP address assignment  
4. Ping printer from workstation  
5. Restart print spooler service  
6. Clear stuck print jobs  
7. Remove and re-add network printer  
8. Print test page  

### Validation Steps

- Printer Responds To Ping  
- Test Page Prints Successfully  
- Print Queue Processes Normally  

### Escalation Criteria

Escalate if:
- Printer Hardware Failure Suspected  
- Multiple Users Affected  
- Switch Or VLAN Issue Identified  

### Related Systems

- Print Server Infrastructure  
- Network Switch Infrastructure  
