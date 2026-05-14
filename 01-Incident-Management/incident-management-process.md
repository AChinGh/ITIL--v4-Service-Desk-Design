# Incident Management Process
### Richmond Solutions Inc. — IT Service Management

Document Version: 1.1

Last Updated: 2026

Owner: Service Desk Team

Practice Area: Incident Management, Service Desk Operations, Event Monitoring

---
### 1. Purpose

The purpose of this process is to restore normal IT service operation as quickly as possible following an unplanned disruption, while minimizing impact to business operations at Richmond Solutions Inc.

This process defines how incidents are:

- Reported
- Logged
- Categorized
- Prioritized
- Investigated
- Resolved
- Closed

---

### 2. Scope

This process applies to all IT-supported services, including:

- Microsoft 365 services
- User endpoints (Windows 11 laptops/desktops)
- Network connectivity and VPN access
- File shares and shared drives
- Business applications (e.g., CRM systems)
- Printing and peripheral services

---

### 3. Definition of an Incident

An incident is any unplanned interruption to an IT service or a reduction in the quality of an IT service.

Examples:
- User cannot access email
- VPN disconnecting repeatedly
- Printer not responding
- Application crashing or freezing
- Network connectivity loss

Not an incident:
- Service Request - Requesting new software
- Service Request - Asking for access to a folder
- Change - Planned system upgrade
- Problem - Root cause investigation

---

### 4. Incident Priority Model
Priority is assigned based on Impact + Urgency

| Priority | Description | Impact | Urgency | Typical Example | Response Target | Resolution Target |
|:--------:|:-----------:|:------:|:-------:|:---------------:|:---------------:|:-----------------:|
| **P1 - Critical** | Major business disruption | Organization-wide | Immediate | Email outage, core system down | 15 minutes | 4 hours |
| **P2 - High** | Significant operational impact | Department-wide | High | VPN failure affecting remote staff | 30 minutes | 8 hours |
| **P3 - Medium** | Limited impact, workaround available | Multiple users | Medium | Application issues, intermittent errors | 2 hours | 24 hours |
| **P4 - Low** | Minor issue workaround available | Low | Single user | Printer issue, display settings | 4 hours | 72 hours |

---

### 5. Incident Lifecycle
The incident lifecycle follows a structured flow:

Detect &#8594; Log &#8594; Categorize &#8594; Prioritize &#8594; Investigate &#8594; Resolve &#8594; Close



### Process Steps
### 5.1 Detect / Identify / Report
Incidents may be detected via:
- Service Desk phone/email
- Self-service portal submission
- Monitoring and alerting tools
- Internal IT identification

Standard channels:
- Email: itsupport@richmondsolutions.ca
- Phone: Extension 100
- Portal: service.richmondsolutions.ca

##

### 5.2 Log
Create an incident ticket immediately in ITSM system.

Minimum required information:
- Reporter name and contact details
- Date and time reported
- Description of issue (user wording)
- Affected system or service
- Number of users affected
- Initial category

##

### 5.3 Categorize

Incidents are categorized to support routing and trend analysis:
- Network / Connectivity
- Hardware
- Software / Application
- Email / Communication Tools
- Identify & Access (Entra ID / AD)
- Printing / Peripherals
- Security-realted issues
- Other

##

### 5.4 Prioritize

Priority is assigned using the Priority Model.

Considerations include:
- Number of users affected
- Business criticality of service
- Workaround availability
- Time sensitivity

##

### 5.5 Investigate & Diagnose

Service Desk performs initial troubleshooting:

Typical activities:

Tier 1
- User verification and clarification
- Remote session analysis
- Log review (where applicable)
- Basic connectivity checks
- Knowledge base article usage

Tier 2 - Escalation occurs when:
- Issue cannot be resolved at Tier 1
- Multiple users are impacted
- Incident exceeds SLA thresholds
- Technical expertise is required

##

### 5.6 Escalation Model

Functional Escalation

Escalation to higher technical expertise:
- Service Desk &#8594; Senior Analyst &#8594; IT Manager / Vendor

##

### 5.7 Resolve & Recover

Resolution involves restoring service using:
- Configuration correction
- Service restart
- User guidance
- Workaround implementation
- Confirm with user that service is restored
- Document the resolution in the ticket
- Change request (if required), if a workaround is applied, a Problem Record is created for root cause investigation

##

### 5.8 Close

An incident is closed only when:
- Service is confirmed restored
- User validation is completed (where applicable)
- Update ticket status to CLosed
- Category and resolution codes are recorded for trending analysis

For P1 / P2 incidents:
- User satisfaction may be requested after closure

---

### 7. Escalation Paths

User Reports Incident

&#8595;

Tier 1 - Service Desk Analyst

├──Resolved &#8594; Close ticket

└──Not resolved within 30 min or P1 / P2 

&#8595;

Tier 2 - Senior IT Analyst

├──Resolved &#8594; Close ticket

└──Not resolved or requires vendor / external support &#8594; IT Manager + Vendor Escalation


### Escalation Types

| Type | When to Use |
|:-----|:------------|
| **Functional** | Issue beyond current analyst's technical expertise |
| **Hierarchical** | SLA at risk, major incident, executive affected, security breach |

##

### Major Incident Handling

A Major Incident is declared when:
- P1 incident affecting critical business systems occurs
- More than 50 users are impacted
- Core services (email, identity, network, payroll) are unavailable

Major Incident Process:
1. Escalation - IT Manager is notified immediately
2. Incident bridge established (Teams/phone)
3. Roles assigned (Incident Lead, Communications Lead)
4. Status updates every 30 minutes
5. Post-Incident Review (PIR) within 48 hours
6. Problem record created if required

---

### 8. SLA Integration

Incident handling is directly tied to SLA commitments:

- Response time = first acknowledgement by technician
- Resolution time = service restored (not root cause fix)

SLA compliance is tracked per incident and reported monthly.

---

### 9. Continual Improvement

Incident trends feed into:

- Problem Management Register
- Continual Improvement Register
- Knowledge Base updates
- Service improvements and automation initiatives

Example triggers:

- Recurring incidents (3+ occurrences)
- High-volume ticket categories
- SLA breaches
- User dissatisfaction trends

---

### 10. Related Documents

- Service Request Catalogue
- SLA & OLA Document
- Problem Management Register
- Change Management Procedure
- Continual Improvement Register

