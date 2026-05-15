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

##

### 2. Scope

This register applies to recurring or high-impact issues involving:
- Microsoft 365 services
- Endpoint devices
- VPN connectivity
- Business applications
- Identity and access systems
- Network infrastructure
- Printing services

##

### 3. Definitions

| Term | Definition |
|:-----|:-----------|
| **Problem** | A cause, or potential cause, of one or more incidents |
| **Known Error** | A problem that has been analysed and its root cause is understood |
| **Workaround** | A temporary solution that reduces impact without fixing the root cause |
| **Root Cause Analysis (RCA)** | The process of identifying the underlying cause of a problem |
| **Trend Analysis** | The process of ticket reviewing to identify recurring issues |

##

### 4. Problem Management Lifecycle

Identify → Analyze → Workaround → Known Error → Raise Change → Resolution → Review

##

### 5. Problem Identification Sources

Problems may be identified through:
- Recurring incidents
- Monitoring alerts
- SLA breach analysis
- Major incident reviews
- User satisfaction feedback
- Trend reporting
- Technician escalation

##

### 6. Problem Prioritization
| Priority	| Description	| Typical Impact |
|:----------|:------------|:---------------|
|P1 — Critical	| Organization-wide recurring issue	| Major service disruption |
|P2 — High	| Department-wide recurring issue	| Significant operational impact |
|P3 — Medium	| Limited recurring issue	| Moderate productivity impact |
|P4 — Low	| Minor recurring issue	| Minimal operational impact |

##

### 7. Problem Register

### PRB-001 — VPN Disconnections During Teams Meetings


| Field | Detail |
|:------|:-------|
| **Problem ID** | PRB-001 |
| **Date Raised** | 2026-01-08 |
| **Raised By** | Service Desk Analyst |
| **Status** | Known Error — Change in progress |
| **Priority** | P2 — High |
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

### Proposed Fix
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
| **Status** | Known Error — Awaiting vendor patch |
| **Priority** | P2 — High |
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

### Proposed Fix
- Upgrade CRM to version 4.2.3 when released by vendor 
- Validate compatibility in test environment before deployment

##

### Change Link
- Pending vendor release — CHG to be raised when patch available 

##

### PRB-003 — Floor 2 Printers Offline Monday Mornings




