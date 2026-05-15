# Problem Management Register
### Richmond Solutions Inc. — IT Service Management

**Document Version:** 1.1
**Last Updated:** 2026  
**Owner:** Senior IT Analyst  
**ITIL Practice Area:** Problem Management, Continual Improvement

---

### 1. Purpose

To record, track, and manage problems — the underlying causes of one or more incidents — 
in order to reduce the likelihood and impact of recurring incidents at Richmond Solutions.

This process focuses on:
- Identifying root causes
- Reducing repeat incidents
- Documenting known errors
- Improving service stability
- Supporting continual service improvement

Problem Management operates separately from Incident Management:
- Incident Management restores service quickly
- Problem Management investigates why incidents occurred

---

### 2. Scope

This register applies to recurring or high-impact issues involving:
- Microsoft 365 services
- Endpoint devices
- VPN connectivity
- Business applications
- Identity and access systems
- Network infrastructure
- Printing services

---

### 3. Definitions

| Term | Definition |
|:-----|:-----------|
| **Problem** | A cause, or potential cause, of one or more incidents |
| **Known Error** | A problem that has been analysed and its root cause is understood |
| **Workaround** | A temporary solution that reduces impact without fixing the root cause |
| **Root Cause Analysis (RCA)** | The process of identifying the underlying cause of a problem |
| **Trend Analysis** | The process of ticket reviewing to identify recurring issues |

---

### 4. Problem Management Lifecycle

Identify → Analyze → Workaround → Known Error → Raise Change → Resolution → Review

---

### 5. Problem Identification Sources

Problems may be identified through:
- Recurring incidents
- Monitoring alerts
- SLA breach analysis
- Major incident reviews
- User satisfaction feedback
- Trend reporting
- Technician escalation

---

### 6. Problem Prioritization
| Priority	| Description	| Typical Impact |
|:----------|:------------|:---------------|
|P1 — Critical	| Organization-wide recurring issue	| Major service disruption |
|P2 — High	| Department-wide recurring issue	| Significant operational impact |
|P3 — Medium	| Limited recurring issue	| Moderate productivity impact |
|P4 — Low	| Minor recurring issue	| Minimal operational impact |

---

### 7. Problem Register

### PRB-001 — VPN Disconnections During Teams Meetings


| Field | Detail |
|:------|:-------|
| **Problem ID** | PRB-001 |
| **Date Raised** | 2026-01-08 |
| **Raised By** | Service Desk Analyst |
| **Priority** | P2 — High |
| **Status** | Known Error — Change in progress |
| **Title** | Recurring VPN disconnections during video calls |
| **Linked Incidents** | INC-0023, INC-0031, INC-0045, INC-0052 |
| **Users Affected** | ~15 remote workers |
| **Description** | Multiple users report VPN dropping during Microsoft Teams calls. Approximately 8–10 incidents per week. Each incident is resolved by reconnecting to VPN, but the underlying cause is unknown. |

##

### Root Cause Analysis

Investigation identified:
- VPN gateway bandwidth is insufficient when >10 simultaneous video calls are active
- Insufficient capacity during high usage periods

Gateway capacity
- Configured: 50 Mbps
- Actual demand during peak hours: 80–90 Mbps

##

### Workaround

Users instructed to:
- reconnect VPN immediately after drop
- Video quality can be reduced in Teams settings to lower bandwidth demand

##

### Known Error 

Yes — root cause identified

##

### Proposed Permanent Fix
- Upgrade VPN gateway bandwidth allocation from 50 Mbps to 150 Mbps via ISP contract amendment
- Upgrade remote access gateway capacity
- Implement monitoring alerts for bandwidth thresholds

##

### Change Link
- Change Raised CHG-012 — VPN Gateway upgrade (pending CAB review)

##

### PRB-002 — CRM Application Crashes on Windows 11 24H2

| Field | Detail |
|:------|:-------|
| **Problem ID** | PRB-002 |
| **Date Raised** | 2026-01-15 |
| **Raised By** | Senior IT Analyst |
| **Priority** | P2 — High |
| **Status** | Known Error — Awaiting vendor patch |
| **Title** | CRM application crashes on Windows 11 build 24H2 |
| **Linked Incidents** | INC-0067, INC-0071, INC-0078 |
| **Users Affected** | 6 users (Sales department) |
| **Description** | CRM application crashes within 5 minutes of opening on machines running Windows 11 build 24H2. Affects 6 workstations upgraded in the last patch cycle. Machines on older builds are unaffected. |

##

### Root Cause Analysis

Vendor confirmed:
- Compatibility issue between CRM version 4.2.1 and Windows 11 24H2

##

### Workaround

Users instructed to:
- Access CRM via browser-based version
- Avoid local application until patch availability

##

### Known Error 

Yes — vendor confirmed

##

### Proposed Permanent Fix
- Upgrade CRM to version 4.2.3 when released by vendor 
- Validate compatibility in test environment before deployment

##

### Change Link
- Pending vendor release — CHG to be raised when patch available 

##

### PRB-003 — Floor 2 Printers Offline Monday Mornings

| Field | Detail |
|:------|:-------|
| **Problem ID** | PRB-003 |
| **Date Raised** | 2026-01-22 |
| **Raised By** | Service Desk Analyst (proactive — trend analysis) |
| **Priority** | P3 — Medium |
| **Status** | Problem Control — RCA in Progress |
| **Title** | Printers on Floor 2 offline every Monday morning |
| **Linked Incidents** | INC-0041, INC-0049, INC-0055, INC-0063 |
| **Users Affected** | ~25 Floor 2 staff |
| **Description** | Both network printers on Floor 2 are consistently offline Monday mornings, requiring manual restart. Identified through ticket trend analysis — 8 consecutive Mondays. Does not affect other floors. |

##

### Root Cause Analysis

Investigation ongoing

Hypothesis: 
- Network switch on Floor 2 loses printer DHCP lease during weekend power-saving mode. Switch restores other devices but printer IP renewal fails

Preliminary analysis suggests:
- DHCP lease renewal failure
- Printer network interface instability
- Switch power-saving interaction after weekend inactivity

##

### Workaround

Service Desk performs:
- Proactive Monday morning printer restart
- Connectivity validation before business hours

##

### Known Error

No — root cause not yet confirmed

##

### Proposed Permanent Fix
- Assign static IP addresses (removes dependency on DHCP renewal)
- Disable problematic power-saving profile
- Update printer firmware

##

### Change Link
- CHG-015 — Printer Network Reconfiguration, submitted

##

### PRB-004 — Organization-Wide Email Authentication Failure

| Field | Detail |
|:------|:-------|
| **Problem ID** | PRB-004 |
| **Date Raised** | 2026-02-03 |
| **Raised By** | IT Manager (post-major-incident review) |
| **Priority** | P1 — Critical |
| **Status** | Error Control — Change in progress |
| **Title** | Email service outage — root cause investigation |
| **Linked Incidents** | INC-0091 (Major Incident) |
| **Users Affected** | 150 (organization-wide) |
| **Description** | A P1 major incident caused all users to lose access to email and cloud authentication services for approximately 3.5 hours, this problem record was raised to investigate root cause and prevent recurrence. |

##

### Root Cause Analysis

Investigation identified:
- Incorrect conditional access policy deployment
- Authentication rules unintentionally blocked all users
- Policy applied directly to production tenant without validation

Affected services:
- Microsoft 365
- Microsoft Entra ID

##

### Immediate Resolution
- Rollback of conditional access policy
- Restoration of previous authentication configuration

##

### Workaround

N/A — service was fully restored

##

### Known Error

Yes — cause confirmed

##

### Proposed Permanent Fix
1. Implement change review checklist for M365 admin changes
2. Test conditional access changes in staging tenant before production
3. Enable audit logging for all admin policy changes
4. Implement peer review for identity-related changes

##

### Change Link
- CHG-017 — Identity Change Control Improvements (Normal change, pending CAB)

##

### PRB-005 — Slow Login Times for Finance Department

| Field | Detail |
|:------|:-------|
| **Problem ID** | PRB-005 |
| **Date Raised** | 2026-02-10 |
| **Raised By** | Senior IT Analyst |
| **Priority** | P3 — Medium |
| **Status** | Problem Control — RCA in progress |
| **Title** | Slow login times on Finance department workstations |
| **Linked Incidents** | None (user-reported via satisfaction survey) |
| **Users Affected** | 12 (Finance department) |
| **Description** | Finance staff report login times of 3–5 minutes, compared to <1 minute for other departments. Issue is consistent across all 12 Finance workstations. No incidents raised — users adapted by arriving earlier. Identified through satisfaction survey feedback. |

##

### Root Cause Analysis

Investigation ongoing

Hypothesis: 
- Network switch on Floor 2 loses printer DHCP lease during weekend power-saving mode. Switch restores other devices but printer IP renewal fails

Preliminary analysis suggests:
- Legacy Group Policy Objects (GPOs)
- Outdated mapped drive references
- Authentication timeout delays to decommissioned systems

##

### Workaround

No temporary workaround currently implemented.

##

### Known Error

No — investigation ongoing

##
 
### Proposed Permanent Fix

- Removelegacy GPO mappings
- Validate login script dependencies
- Audit departmental authentication policies

##

### Change Link
- Not yet — pending RCA confirmation 

---

### 8. Problem Register / Known Error Summary

| ID | Title | Status | Priority | Change Raised |
|:---|:------|:-------|:---------|:--------------|
| PRB-001 | VPN disconnections during video calls | Known Error — Change in progress | P2 | CHG-012 |
| PRB-002 | CRM crash on Windows 11 24H2 | Known Error — Awaiting vendor patch | P2 | Pending |
| PRB-003 | Floor 2 printers offline Mondays | Problem Control — RCA in progress | P3 | CHG-015 |
| PRB-004 | Email outage root cause | Known Error (Error Control) — Change in progress | P1 | CHG-017 |
| PRB-005 | Slow Finance workstation logins | Problem Control — RCA in progress | P3 | Pending |

---

### 9. Trend Analysis & Reporting

Problem Management reporting includes:
- Recurring incident categories
- High-volume service disruptions
- Known error tracking
- SLA breach correlation
- Root cause trends

Trend reviews occur:
- Monthly during IT operational reviews
- After all major incidents
- During continual improvement meetings

---

### 10. Problem Escalation Criteria

Problems are escalated when:
- Recurring incidents continue increasing
- Business-critical services are impacted
- Workaround no longer effective
- Major financial or operational risk exists

---

### 11. Relationship to Other Processes
| Process |	Relationship |
|:--------|:-------------| 
| Incident Management	| Recurring incidents trigger problems |
| Change Management	| Permanent fixes require approved changes |
| Continual Improvement	| Problem trends identify improvement opportunities |
| Knowledge Management	| Known errors documented for Service Desk use |

---

### 12. Continual Improvement Integration

Problem trends support:
- Proactive monitoring improvements
- Automation opportunities
- Operational optimization
- Knowledge base development
- Infrastructure planning

Examples:
- VPN capacity upgrades
- Login optimization
- Monitoring enhancement
- Onboarding improvements

---

### 13. ITIL v4 Guiding Principles Applied

| Principle	| Application |
|:----------|:------------|
| Focus on Value	| Reducing recurring incidents restores productivity |
| Think and Work Holistically	| Problems analyzed across systems and services |
| Progress Iteratively with Feedback	| RCA updated continuously during investigation |
| Start Where You Are	| Existing ticket trends used to identify recurring issues (PRB-003 and PRB-005 identified through trend analysis of existing ticket data) |

---

### 14. Related Documents
- Incident Management Process
- SLA & OLA Document
- Change Management Procedure
- Continual Improvement Register
- Knowledge Base Articles




