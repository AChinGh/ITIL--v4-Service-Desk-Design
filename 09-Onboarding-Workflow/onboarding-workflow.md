# User Onboarding Workflow & Procedure
### Richmond Solutions Inc. — IT Service Management

**Document Version:** 1.2
**Last Updated:** 2026
**Owner:** IT Support Team
**Practice Area:** Service Request Management, IT Asset Management,
Information Security Management, Continual Improvement

---

## 1. Purpose

The purpose of this procedure is to standardize and control the onboarding
process for all new users at Richmond Solutions Inc.

This ensures:

- consistent identity provisioning
- secure access assignment
- standardized endpoint setup
- controlled application access
- validated user readiness
- reduced onboarding errors
- predictable start-of-work experience

---

## 2. Scope

This process applies to:

- full-time employees
- contractors
- temporary staff
- remote workers
- interns (if applicable)

> **Note:** The reverse of this process — user offboarding and account
> deprovisioning — is managed separately. Offboarding must be initiated by
> HR on or before the employee's last working day to ensure timely access
> revocation in line with Information Security Management controls.

---

## 3. Onboarding Workflow Overview

```text
HR Request Submitted (via hr@richmondsolutions.ca or service portal)
↓
IT Ticket Created (manual — automation planned under CIR-005, target 2026-Q3)
↓
Manager Approval Verified
↓
Identity Provisioning
↓
Endpoint Setup
↓
Access Assignment
↓
Validation
↓
User Activation
↓
Ticket Closure
```

---

## 4. Identity Provisioning

Identity provisioning is the first stage of onboarding and establishes
the user's digital identity.

### 4.1 Tasks

- create Microsoft Entra account
- assign appropriate Microsoft 365 licence
- configure Multi-Factor Authentication (MFA)
- apply identity security policies

### 4.2 Identity Controls

- account naming convention enforced
- temporary password generated securely
- MFA required at first login
- conditional access policies applied based on department
- all identity provisioning actions logged in Microsoft Entra audit logs
  and reviewed by the IT Manager quarterly or upon a security incident

---

## 5. Endpoint Setup

Endpoint setup ensures the user receives a secure and compliant workstation.

### 5.1 Tasks

- assign laptop from asset pool
- install standard corporate image
- apply security baseline configuration
- join device to domain / Entra Join
- install endpoint protection agent

### 5.2 Security Baseline Includes

- disk encryption enabled
- firewall enabled
- endpoint detection and response agent installed
- automatic updates enforced
- local admin rights restricted

---

## 6. Access Assignment

Access is granted based on role and least-privilege principles.

### 6.1 Identity-Based Access

- Microsoft Teams access
- email mailbox activation
- MFA enforcement validation

### 6.2 File & Collaboration Access

- shared drives assigned based on department
- role-based folder permissions applied
- collaboration groups added

### 6.3 Department Application Access

Examples:

- CRM systems
- finance applications
- HR portals
- internal business tools

Access is granted only after manager approval confirmation.

### 6.4 User Type Access Differentiation

| User Type | Account Expiry | Device | Access Restrictions |
|-----------|---------------|--------|---------------------|
| Full-time employee | No expiry | Corporate laptop | Full role-based access |
| Contractor | Set to contract end date | Corporate or BYOD | Restricted to project scope only |
| Temporary staff | Set to assignment end date | Corporate | Standard role, no sensitive systems |
| Intern | Set to internship end date | Shared or corporate | Restricted — manager defined |

---

## 7. Validation Stage

Validation ensures all onboarding steps are completed correctly before
user activation.

### 7.1 Validation Tasks

- test login to Windows device
- confirm Microsoft Entra authentication
- verify mailbox functionality
- validate Teams access
- confirm shared drive visibility
- confirm application access

### 7.2 Acceptance Criteria

Onboarding is not complete unless:

- all authentication systems function correctly
- email is accessible
- device login succeeds
- department access matches approval request

---

## 8. User Activation & Handover

Once validation is complete:

- send welcome instructions to user
- provide login credentials securely
- share IT usage guidelines
- provide support contact information
- confirm onboarding completion with manager

---

## 9. Full Onboarding Workflow (End-to-End)

```text
HR Submission
↓
Manager Approval
↓
Identity Provisioning
   → Create Entra Account
   → Assign Licence
   → Configure MFA
↓
Endpoint Setup
   → Assign Laptop
   → Apply Security Baseline
   → Join Domain / Entra Join
↓
Access Assignment
   → Teams Access
   → Shared Drives
   → Department Applications
↓
Validation
   → Test Login
   → Confirm Mailbox
   → Verify Access
↓
User Activation
   → Send Welcome Instructions
   → Confirm Ready Status
↓
Ticket Closure
```

---

## 10. Roles & Responsibilities

| Role | Responsibility |
|------|----------------|
| Service Desk Analyst | Account creation, endpoint setup, basic access provisioning |
| Senior IT Analyst | VPN setup, advanced access, troubleshooting |
| IT Manager | Approval oversight, escalations, exceptions |
| HR | Initiates onboarding request |
| Hiring Manager | Confirms access requirements |

---

## 11. Escalation Criteria

Escalate onboarding issues when:

- start date is at risk
- hardware is unavailable
- licensing constraints exist
- access approval is missing
- authentication failures occur
- security policy conflicts arise

---

## 12. Service Targets

> **Lead time requirement:** IT requires a minimum of 5 business days
> notice before a new hire's start date to guarantee full onboarding
> completion. Requests submitted with less than 5 business days notice
> are subject to best-effort delivery and may result in delayed access.

| Activity | Target | Notes |
|----------|--------|-------|
| Account creation | Same business day | Upon receipt of approved request |
| Laptop assignment | 1–3 business days | Same-day possible subject to asset pool availability |
| Access provisioning | 1 business day after approval | Subject to manager approval being received |
| Full onboarding completion | Before start date | Requires 5 business days minimum notice |

---

## 13. Security & Compliance Controls

Onboarding must enforce:

- least privilege access model
- MFA enforcement for all users
- Role-Based Access Control (RBAC)
- audit logging of all identity actions (Microsoft Entra audit logs —
  reviewed quarterly by IT Manager)
- approved software baseline only

---

## 14. Success Metrics

| Metric | Baseline | Target | Measurement Frequency |
|--------|----------|--------|-----------------------|
| Onboarding completed before start date | 78% (current — manual process) | 100% | Per onboarding |
| Failed login issues after onboarding | 8% of onboardings | <2% | Monthly |
| Access misconfiguration rate | Not currently tracked | <1% | Monthly |
| Average onboarding time | 2.5 business days | <1 business day | Monthly |

---

## 15. Relationship to ITIL Practices

| ITIL v4 Practice | How This Document Relates |
|-----------------|--------------------------|
| Service Request Management | Onboarding is triggered by a service request from HR |
| IT Asset Management | Laptop assignment and asset register updates throughout lifecycle |
| Service Configuration Management | Device joined to domain — CI record created in CMDB |
| Information Security Management | MFA, least privilege, RBAC, audit logging enforced throughout |
| Change Enablement | Non-standard access requests may require change authorization |
| Continual Improvement | Onboarding metrics feed the CIR — CIR-005 tracks automation initiative |

---

## 16. Continual Improvement Integration

The following onboarding improvements are actively tracked in the
Richmond Solutions Continual Improvement Register:

- **CIR-005** — Automated user onboarding workflow (target: 2026-Q3)

Additional improvement opportunities identified from onboarding metrics:

- standardized role-based access templates by department
- automated licence assignment based on department
- pre-built device images by role to reduce endpoint setup time
- automated account expiry for contractors and temporary staff

---

## 17. ITIL v4 Guiding Principles Applied

| Guiding Principle | Application |
|------------------|-------------|
| Focus on Value | Structured onboarding ensures users are productive from day one |
| Start Where You Are | Workflow built from existing provisioning steps already performed manually |
| Progress Iteratively with Feedback | Onboarding metrics reviewed monthly — process improved each cycle |
| Keep It Simple and Practical | Single end-to-end workflow reduces missed steps and inconsistency |
| Collaborate and Promote Visibility | HR, hiring manager, and IT work together with clear handoff points |
| Optimize and Automate | Manual steps identified for automation under CIR-005 |

---

## 18. Related Documents

- Incident Management Process
- Service Request Catalogue
- SLA & OLA Document
- Problem Management Register
- Change Management Procedure
- Continual Improvement Register
- Knowledge Management Practice
- Ticket Samples Repository

---

## Document Change Log

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.0 | January 2026 | IT Support Team | Initial document |
| 1.1 | February 2026 | IT Support Team | Added validation acceptance
criteria, security baseline detail, escalation criteria section |
| 1.2 | February 2026 | IT Support Team | Fixed capitalisation throughout,
corrected ITIL practice names in Section 15, added contractor access
differentiation table, added lead time requirement, added offboarding
reference, added audit logging detail, added baselines to metrics table,
added measurement frequency column, linked CIR-005 in Section 16,
replaced summary with guiding principles table, added change log,
corrected Section 3 workflow to reflect manual ticket creation,
added laptop availability note to Section 12 |
