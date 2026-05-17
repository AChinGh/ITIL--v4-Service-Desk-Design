# Knowledge Management Practice

### Richmond Solutions Inc. — IT Service Management

**Document Version:** 1.3

**Last Updated:** 2026

**Owner:** Service Desk Team

**Practice Area:** Knowledge Management, Service Desk, Incident Management

---

## 1. Purpose

The purpose of the Knowledge Management practice is to ensure operational
knowledge is:

- captured
- organized
- shared
- maintained
- reused across IT operations

This practice supports:

- faster incident resolution
- reduced escalations
- improved first contact resolution
- operational consistency
- user self-service support

The objective is to ensure that valuable operational knowledge is retained
within Richmond Solutions and can be reused efficiently by IT staff and
end users.

---

## 2. Knowledge Management Model

Knowledge Management at Richmond Solutions follows the DIKW hierarchy:

- data
- information
- knowledge
- wisdom

Operational incident data is transformed into structured knowledge articles
that improve decision-making, reduce resolution times, and preserve
organizational learning.

Knowledge is stored within the Richmond Solutions Knowledge Management
System (KMS), built on Microsoft SharePoint and integrated with the broader
Service Knowledge Management System (SKMS), including:

- incident records
- problem records
- change records
- configuration data (CMDB)
- knowledge articles
- major incident reviews

The KMS is accessible internally through the IT service portal at
`portal.richmondsolutions.ca` and the SharePoint knowledge site at
`knowledge.richmondsolutions.ca`

---

## 3. Scope

Knowledge articles may include:

- troubleshooting guides
- known errors
- standard operating procedures
- user instructions
- service request guidance
- configuration procedures
- escalation instructions
- onboarding documentation
- major incident review findings

This practice applies to all IT-supported systems and services at
Richmond Solutions.

---

## 4. Knowledge Sources

Knowledge may originate from:

- incident resolution activities
- problem management reviews
- major incident reviews
- vendor documentation
- change implementations
- user feedback
- trend analysis
- continual improvement initiatives
- onboarding and offboarding activities

Knowledge creation is considered part of normal operational work and is
not treated as a separate documentation exercise.

---

## 5. Knowledge Lifecycle

| Stage | Owner | Activity |
|-------|-------|----------|
| Create | Service Desk Analyst | Draft article from incident resolution, problem review, or major incident review |
| Review | Senior IT Analyst | Validate technical accuracy and troubleshooting steps |
| Approve | IT Manager | Confirm article meets operational and security standards |
| Publish | Service Desk Analyst | Publish article to SharePoint knowledge base and apply category tags |
| Maintain | Service Desk Team | Update article after process changes or quarterly review |
| Retire | IT Manager | Archive outdated articles no longer relevant to supported systems |

---

## 6. Knowledge Article Standards

All knowledge articles must include:

- title
- symptoms
- affected systems
- root cause (if known)
- resolution steps
- validation steps
- escalation criteria
- related services
- related incidents or problems
- last review date

Articles must:

- use clear operational language
- avoid unnecessary technical jargon
- include repeatable troubleshooting steps
- follow the standard KB template
- be reviewed quarterly for accuracy

---

## 7. Knowledge Base Categories

| Category | Examples |
|----------|----------|
| Authentication | Password reset, MFA enrollment |
| Collaboration | Teams audio issues, shared mailbox access |
| Connectivity | VPN troubleshooting, network access |
| Hardware | Printer troubleshooting, laptop setup |
| Software | Application errors, software installation |
| Security | Phishing reporting, endpoint protection |
| Onboarding | New user setup, account provisioning |

---

## 8. Roles & Responsibilities

| Role | Responsibility |
|------|----------------|
| Service Desk Analyst | Create, update, and maintain knowledge articles |
| Senior IT Analyst | Review technical accuracy and approve troubleshooting procedures |
| IT Manager (Knowledge Manager) | Owns the Knowledge Management practice, standards, governance, and review process |
| All Staff | Submit knowledge gaps, documentation requests, and feedback through the service portal |

---

## 9. Knowledge Review Schedule

| Activity | Frequency |
|----------|-----------|
| Knowledge article review | Quarterly |
| Outdated article audit | Semi-annual |
| Major incident knowledge update | After each PIR |
| Knowledge category review | Quarterly |
| KB template review | Annually |

---

## 10. Success Metrics

| Metric | Baseline | Target | Measurement Frequency |
|--------|----------|--------|-----------------------|
| First contact resolution | 72% | >80% | Monthly |
| Knowledge usage rate | Not currently tracked | Measured and increasing quarterly | Monthly |
| Ticket escalation rate | 28% of tickets escalated | Reduce by 20% within 6 months | Monthly |
| Repeat incident volume | Top 15 incidents recurring monthly | Reduce by 20% | Monthly |

---

## 11. Related Documents

- Incident Management Process
- Service Request Catalogue
- SLA & OLA Document
- Problem Management Register
- Change Management Procedure
- Continual Improvement Register
- User Onboarding Workflow & Procedure
- Ticket Samples Repository

---

## 12. ITIL v4 Guiding Principles Applied

| Guiding Principle | Application |
|-------------------|-------------|
| Focus on Value | Knowledge reuse reduces resolution time and restores user productivity faster |
| Start Where You Are | Articles are created from existing incident trends, problem records, and operational experience |
| Progress Iteratively with Feedback | Quarterly reviews and post-incident updates improve article quality continuously |
| Keep It Simple and Practical | Standardized templates ensure consistent and usable documentation |
| Collaborate and Promote Visibility | Knowledge base is accessible to all staff through the service portal |

---

## 13. Knowledge Base — Published Articles

---

### KB-001 — Password Reset Procedure

| Field | Detail |
|-------|--------|
| Article ID | KB-001 |
| Category | Authentication |
| Author | Service Desk Team |
| Last Reviewed | January 2026 |
| Related Tickets | SR-2026-0021, SR-2026-0034 |
| Related Problems | — |
| Status | Published |

#### Symptoms

Users report:

- incorrect password
- account locked
- sign-in failure
- MFA prompt loop

#### Resolution Steps

1. Verify user identity using internal verification procedure
2. Open identity management console (Microsoft Entra ID)
3. Locate user account
4. Reset password to secure temporary value
5. Force password change at next login
6. Unlock account if required
7. Confirm successful login with user

#### Validation Steps

- user successfully logs into workstation
- user successfully accesses email
- MFA authentication completes successfully

#### Escalation Criteria

Escalate if:

- suspicious login activity detected
- MFA device unavailable or lost
- identity verification cannot be completed

#### Related Systems

- Microsoft Entra ID (identity platform)
- Active Directory
- Microsoft 365 (mailbox and authentication)
- MFA authentication service

---

### KB-002 — Microsoft Teams Microphone Troubleshooting

| Field | Detail |
|-------|--------|
| Article ID | KB-002 |
| Category | Collaboration |
| Author | Service Desk Team |
| Last Reviewed | January 2026 |
| Related Tickets | INC-2026-0067 |
| Related Problems | — |
| Status | Published |

#### Symptoms

Users report:

- no audio during meetings
- microphone not detected
- audio works in other applications but not in Teams
- participants cannot hear user

#### Resolution Steps

1. Confirm microphone is not physically muted
2. Check operating system sound settings
3. Verify correct input device is selected
4. Open Microsoft Teams settings
5. Navigate to Devices section
6. Select correct microphone input
7. Run Teams test call feature
8. Restart Teams if issue persists

#### Validation Steps

- microphone input detected successfully
- test call produces audio
- other participants confirm audio quality

#### Escalation Criteria

Escalate if:

- hardware failure suspected
- device drivers fail to load
- microphone not detected by operating system

#### Related Systems

- Microsoft Teams
- Windows audio subsystem

---

### KB-003 — VPN Reconnect Checklist

| Field | Detail |
|-------|--------|
| Article ID | KB-003 |
| Category | Connectivity |
| Author | Service Desk Team |
| Last Reviewed | January 2026 |
| Related Tickets | INC-2026-0041 |
| Related Problems | PRB-001 — VPN Gateway Capacity Issue |
| Status | Published |

#### Symptoms

Users report:

- VPN disconnects during sessions
- unable to reconnect VPN
- MFA timeout errors
- unstable remote access connection

#### Resolution Steps

1. Confirm internet connectivity is available
2. Disconnect VPN session fully
3. Restart VPN client application
4. Re-authenticate with corporate credentials
5. Approve MFA request
6. Verify IP assignment
7. Attempt reconnect
8. Restart workstation if issue persists

#### Validation Steps

- VPN status shows connected
- internal systems accessible
- connection remains stable for 10 minutes

#### Escalation Criteria

Escalate if:

- multiple users affected simultaneously
- VPN gateway unreachable
- authentication failures continue after reset

#### Related Records

- PRB-001 — VPN Gateway Capacity Issue (known error — permanent fix in
  progress under CHG-012)
- Note: recurring VPN drops during Teams calls are a known capacity issue.
  Refer to PRB-001 for root cause detail and workaround guidance.

#### Related Systems

- remote access gateway
- identity authentication services

---

### KB-004 — Printer Offline Resolution SOP

| Field | Detail |
|-------|--------|
| Article ID | KB-004 |
| Category | Hardware |
| Author | Service Desk Team |
| Last Reviewed | January 2026 |
| Related Tickets | INC-2026-0078 |
| Related Problems | PRB-003 — Floor 2 Printer Monday Offline Issue |
| Status | Published |

#### Symptoms

Users report:

- printer offline status
- print jobs stuck in queue
- printer unavailable on network
- intermittent print failures

#### Resolution Steps

1. Confirm printer is powered on
2. Verify network cable connectivity
3. Check printer IP address assignment
4. Ping printer from workstation
5. Restart print spooler service
6. Clear stuck print jobs
7. Remove and re-add network printer
8. Print test page

#### Validation Steps

- printer responds to ping
- test page prints successfully
- print queue processes normally

#### Escalation Criteria

Escalate if:

- printer hardware failure suspected
- multiple users affected
- switch or VLAN issue identified

#### Related Records

- PRB-003 — Floor 2 Printer Monday Offline Issue (known error — permanent
  fix in progress under CHG-015)
- Note: if printer offline occurs on a Monday morning on Floor 2, this is
  a known recurring issue. Apply the standard restart workaround and refer
  to PRB-003. Permanent fix via static IP assignment is pending under
  CHG-015.

#### Related Systems

- print server infrastructure
- network switch infrastructure

---

## Document Change Log

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.0 | January 2026 | Service Desk Team | Initial document — purpose, scope, roles, review schedule |
| 1.1 | February 2026 | Service Desk Team | Added DIKW model, SKMS reference, knowledge lifecycle table, four complete knowledge articles, expanded article standards, success metrics with baselines |
| 1.2 | February 2026 | Service Desk Team | Fixed capitalisation throughout, separated article list from article content, corrected escalation criteria formatting |
| 1.3 | February 2026 | Service Desk Team | Fixed company name to Richmond Solutions throughout, repaired broken reference tags in KB-001 and KB-002, added KMS URLs, added article metadata headers, added related records to KB-003 and KB-004, added measurement frequency column to metrics table, added Ticket Samples Repository to related documents |
