# Systems and Access Model

## 1. Purpose

This document defines the systems included in the IAM Joiner, Mover and Leaver process for Meridian Crest Services Ltd.

It identifies:

- The business owner of each system
- The type of information processed
- The access sensitivity
- The required approvers
- The standard user roles
- The access-review frequency

Access must only be granted where there is a valid business need and documented approval.

---

## 2. Access Classification

Meridian Crest Services Ltd. uses four access levels.

| Access Level | Description | Examples |
|---|---|---|
| Standard | Basic access required by most employees | Microsoft 365, standard file access |
| Departmental | Access restricted to a specific department | HR folders, Finance folders, CRM |
| Sensitive | Access to confidential, financial or personal information | Payroll, HRIS, Finance System |
| Privileged | Administrative access capable of changing systems or user permissions | Domain administrator, system administrator |

Privileged access must not be assigned through a standard employee account.

---

## 3. Systems in Scope

| System ID | System | Business Owner | Primary Users | Access Level | Access Review |
|:---:|---|---|---|---|---|
| SYS-001 | Active Directory | IT Manager | All employees | Standard and Privileged | Quarterly |
| SYS-002 | Microsoft 365 | IT Manager | All employees | Standard and Privileged | Quarterly |
| SYS-003 | HR Information System | HR Manager | HR and approved managers | Sensitive | Quarterly |
| SYS-004 | Payroll System | Finance Manager | Payroll officers and approved HR staff | Sensitive | Quarterly |
| SYS-005 | Finance System | Finance Manager | Finance employees | Sensitive | Quarterly |
| SYS-006 | CRM System | Sales Manager | Sales and approved Compliance staff | Departmental | Quarterly |
| SYS-007 | File-Sharing Platform | Relevant Department Manager | All departments | Standard and Departmental | Quarterly |
| SYS-008 | VPN | IT Manager | Approved remote users | Sensitive | Quarterly |
| SYS-009 | Administrative Accounts | IT Manager | Approved IT administrators | Privileged | Monthly |

---

## 4. System Access Requirements

### Active Directory

Active Directory provides employee accounts, authentication and security-group membership.

Standard access requires:

- Confirmed employment or contractor status
- Manager approval
- Verified department and job role
- Unique user account
- Initial password reset at first login

Privileged Active Directory access requires:

- IT Manager approval
- Information Security approval
- Separate administrative account
- Multi-factor authentication
- Documented business justification
- Monthly access review

### Microsoft 365

Microsoft 365 provides email, Teams and collaboration services.

Standard access requires:

- An approved employee or contractor record
- Manager confirmation
- Appropriate licence assignment
- Multi-factor authentication

Administrative roles require separate approval and must not be assigned automatically.

### HR Information System

The HR Information System contains personal and employment information.

Access is restricted to:

- HR employees
- Approved managers with limited employee-view access
- Approved system administrators

Full HR access requires approval from the HR Manager and system owner.

### Payroll System

The Payroll System contains salary, banking and payment information.

Access is restricted to:

- Payroll officers
- Selected Finance employees
- Approved HR employees
- Approved technical administrators

Users who create payroll records should not approve final payroll payments.

### Finance System

The Finance System supports expenses, payments and financial reporting.

Access is assigned according to job responsibility.

Key restrictions include:

- Payment creators must not approve their own payments.
- Vendor creators must not independently approve payments to those vendors.
- Read-only access must be used where transaction access is unnecessary.
- Finance administrator access requires separate privileged approval.

### CRM System

The CRM System contains customer, sales and account information.

Access is primarily assigned to:

- Sales employees
- Sales managers
- Approved Compliance employees
- Approved technical administrators

Users receive access only to the functions required by their role.

### File-Sharing Platform

Departmental folders are restricted by department and business need.

Access requires:

- Employee manager approval
- Folder-owner approval for restricted folders
- Removal of previous departmental access after a transfer

Confidential folders must not be accessible to all employees.

### VPN

VPN access is not automatically provided to every employee.

It requires:

- Confirmed remote-access need
- Manager approval
- IT approval
- Multi-factor authentication
- A company-managed device where applicable

Inactive VPN accounts must be reviewed and removed.

### Administrative Accounts

Administrative accounts provide elevated system access.

Requirements include:

- Separate standard and administrative accounts
- Named accounts instead of shared accounts
- Multi-factor authentication
- Documented approval
- Restricted use
- Activity logging
- Monthly review
- Immediate removal when no longer required

---

## 5. Approval Model

| Access Type | Manager Approval | System-Owner Approval | Information Security Approval |
|---|:---:|:---:|:---:|
| Standard Microsoft 365 access | Required | Not required | Not required |
| Standard departmental folder access | Required | Required where restricted | Not required |
| HRIS access | Required | Required | Required for elevated access |
| Payroll access | Required | Required | Required for elevated access |
| Finance System access | Required | Required | Required for privileged access |
| CRM access | Required | Required | Required for privileged access |
| VPN access | Required | Required | Required for exceptions |
| Privileged access | Required | Required | Required |
| Temporary exceptional access | Required | Required | Required |

IT must not approve its own access request without independent authorization.

---

## 6. Standard Access Principles

All access decisions must follow these principles:

### Least Privilege

Users receive only the minimum access required to complete assigned duties.

### Need to Know

Access to confidential information is limited to employees whose work requires it.

### Role-Based Access Control

Standard access is assigned according to approved job roles.

### Segregation of Duties

Conflicting responsibilities must not be assigned to one user without an approved exception.

### Unique Accountability

Each user must have an individual account. Shared accounts are prohibited unless formally approved and technically necessary.

### Time-Limited Access

Temporary and exceptional access must have an expiry date.

### Independent Approval

Sensitive and privileged access requires approval outside the IT provisioning team.

---

## 7. Access Ownership

| Role | Access-Governance Responsibility |
|---|---|
| Human Resources | Confirms employee status, department, manager, start date and end date |
| Employee Manager | Confirms business need and appropriate role |
| System Owner | Approves access to the system and sensitive functions |
| IT Service Desk | Provisions, modifies and disables approved access |
| Information Security | Reviews privileged access, high-risk access and exceptions |
| Compliance | Reviews evidence, access reviews and control performance |
| User | Protects credentials and uses access only for approved purposes |

---

## 8. Access Evidence Requirements

Every access action must produce evidence showing:

- User name and employee identifier
- Department and job role
- Requested system and role
- Business justification
- Manager approval
- System-owner approval where required
- Security approval where required
- Provisioning date
- Provisioned access
- Name of the person who completed the action
- Review or expiry date
- Revocation date where applicable

The evidence must be retained in the approved access-management record location.

---

## 9. Expected Result

This access model provides a consistent basis for determining:

- Which systems an employee may access
- Who must approve the access
- Whether the access is standard, sensitive or privileged
- How often the access must be reviewed
- What evidence must be retained

It supports controlled and auditable Joiner, Mover and Leaver activities.
