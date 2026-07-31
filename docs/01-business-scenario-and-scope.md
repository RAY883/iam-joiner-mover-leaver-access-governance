# IAM Joiner, Mover and Leaver Access Governance

## Business Scenario

Meridian Crest Services Ltd. is a fictional medium-sized business-services company operating in Ghana.

The company has approximately 350 employees across the following departments:

- Human Resources
- Finance
- Operations
- Information Technology
- Sales
- Compliance

The organisation depends on several information systems to support employee communication, payroll, financial processing, customer management, document sharing and remote access.

Employee access is currently managed through emails, informal requests and manual account updates. There is no consistent process covering the complete employee-access lifecycle.

This creates the risk that users may receive inappropriate access, retain permissions after changing roles or remain active after leaving the organisation.

> Meridian Crest Services Ltd. is a fictional organisation created for cybersecurity portfolio purposes.

---

## Business Problem

The organisation has identified the following access-governance weaknesses:

- New employees may receive access that exceeds their job responsibilities.
- Access requests may be completed without documented approval.
- Employees who change departments may retain permissions from previous roles.
- Former employees may continue to have active accounts.
- Dormant and unused accounts may not be identified.
- Privileged accounts may not be reviewed consistently.
- Segregation-of-duties conflicts may not be detected.
- Access-review evidence may be incomplete or unavailable.
- Account disablement may be delayed.
- Temporary access may remain active beyond its approved period.

These weaknesses increase the likelihood of unauthorised access, data exposure, fraud, operational disruption and audit findings.

---

## Project Objective

The objective of this project is to design a complete and auditable Joiner, Mover and Leaver access-governance process for Meridian Crest Services Ltd.

The process will show how access is:

1. Requested
2. Approved
3. Provisioned
4. Modified
5. Reviewed
6. Recertified
7. Revoked
8. Documented
9. Escalated
10. Audited

The process will apply:

- Least privilege
- Role-Based Access Control
- Need-to-know access
- Segregation of duties
- Manager approval
- System-owner approval
- Privileged-access restrictions
- Timely account removal
- Periodic access reviews
- Exception approval
- Risk-based escalation

---

## Project Scope

The project covers:

- Permanent employees
- Temporary employees
- Contractors
- Department transfers
- Role changes
- Promotions
- Employee departures
- Privileged administrator accounts
- Remote-access accounts
- Quarterly access reviews
- Access exceptions
- Access evidence and audit records

The project covers process design and documentation. It does not include deployment of a commercial identity-governance platform.

---

## Systems in Scope

| System | Primary Users | Access or Information Involved |
|---|---|---|
| Active Directory | All employees | User accounts, security groups and authentication |
| Microsoft 365 | All employees | Email, Teams and collaboration services |
| HR Information System | HR and managers | Employee and employment records |
| Payroll System | HR and Finance | Payroll and banking information |
| Finance System | Finance | Payments, expenses and financial records |
| CRM System | Sales and Compliance | Customer and sales information |
| File-Sharing Platform | All departments | Departmental and shared documents |
| VPN | Approved remote users | Remote access to company resources |
| Administrative Accounts | IT administrators | Privileged access to systems and infrastructure |

---

## Stakeholders

| Stakeholder | Responsibility |
|---|---|
| Human Resources | Initiates Joiner, Mover and Leaver events |
| Employee Manager | Confirms business need and requested access |
| System Owner | Approves access to sensitive applications |
| Information Technology | Creates, modifies and disables accounts |
| Information Security | Reviews privileged access, exceptions and high-risk requests |
| Compliance | Reviews control evidence and access-review completion |
| Employee | Uses approved access according to company requirements |

---

## Initial Access Risks

| Risk ID | Risk Description | Initial Risk Level |
|:---:|---|---|
| IAM-001 | New employees receive excessive or inappropriate access | High |
| IAM-002 | Employees retain old access after changing roles | High |
| IAM-003 | Former employees retain active accounts | Critical |
| IAM-004 | Access is provisioned without documented approval | High |
| IAM-005 | Privileged access is misused or insufficiently monitored | High |
| IAM-006 | Dormant accounts remain active | Medium |
| IAM-007 | Segregation-of-duties conflicts are not detected | High |
| IAM-008 | Access reviews are incomplete or unsupported by evidence | Medium |
| IAM-009 | Account termination is delayed | High |
| IAM-010 | Temporary or exceptional access is not removed | Medium |

---

## Expected Business Outcome

The completed process should help Meridian Crest Services Ltd. to:

- Reduce unauthorised and excessive access
- Prevent accumulation of outdated permissions
- Disable departing-user accounts promptly
- Improve control over privileged accounts
- Detect segregation-of-duties conflicts
- Maintain clear approval and provisioning evidence
- Support internal and external audits
- Improve accountability between HR, managers, system owners and IT
