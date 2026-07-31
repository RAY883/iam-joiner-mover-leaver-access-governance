# Joiner, Mover and Leaver Processes and Operational Templates

## 1. Purpose

This document defines how Meridian Crest Services Ltd. manages employee access throughout the employment lifecycle.

It covers:

- New employees joining the organisation
- Employees changing department or job role
- Employees leaving the organisation
- Access requests and approvals
- Account provisioning and modification
- Account termination
- Operational evidence
- Sample employee scenarios

All access actions must be supported by an approved request and retained evidence.

---

# 2. Joiner Process

## 2.1 Objective

The Joiner process ensures that new employees receive only the access required for their role before or on their approved start date.

## 2.2 Joiner Workflow

1. Human Resources creates the employee record.
2. HR confirms the employee's:
   - Full name
   - Employee ID
   - Department
   - Job title
   - Manager
   - Employment type
   - Start date
3. The employee manager selects the appropriate role-based access.
4. Additional access is requested only where there is a documented business need.
5. The system owner approves access to sensitive systems.
6. Information Security approves privileged or exceptional access.
7. IT verifies the approvals.
8. IT creates the user account.
9. IT assigns approved groups, applications and licences.
10. Multi-factor authentication is enabled where required.
11. The user must change the initial password at first login.
12. IT records the completed provisioning actions.
13. The employee manager confirms that the access is correct.

## 2.3 Joiner Control Requirements

- No account may be created without confirmed HR information.
- Access must match the employee's approved role.
- Sensitive access requires system-owner approval.
- Privileged access requires Information Security approval.
- The employee must receive an individual account.
- Shared accounts must not be used for normal employee access.
- Access must not be activated earlier than necessary.
- All provisioning actions must be documented.

## 2.4 Joiner Process Result

The new employee receives appropriate access based on role, business need and documented approval.

## 2.5 Why It Matters

A controlled Joiner process reduces excessive access, unapproved permissions and inconsistent account creation.

---

# 3. Mover Process

## 3.1 Objective

The Mover process ensures that access is updated when an employee changes department, job role, responsibility or location.

## 3.2 Mover Events

The process applies when an employee:

- Transfers to another department
- Receives a promotion
- Changes job responsibilities
- Changes manager
- Moves to another location
- Starts or ends a temporary assignment
- Requires additional access
- No longer requires existing access

## 3.3 Mover Workflow

1. HR records the approved role or department change.
2. HR notifies the employee's current manager, new manager and IT.
3. The new manager identifies the access required for the new role.
4. The current manager identifies access that is no longer required.
5. System owners review requests for sensitive applications.
6. Information Security reviews privileged or high-risk access.
7. IT removes access linked to the previous role.
8. IT assigns access approved for the new role.
9. Segregation-of-duties conflicts are checked.
10. Temporary access receives an expiry date.
11. IT documents all removed and added permissions.
12. The new manager confirms the final access.

## 3.4 Mover Control Requirements

- Previous-role access must not remain active without justification.
- New access must not be added before approval.
- Access removal and access addition must be recorded separately.
- Segregation-of-duties checks must be completed.
- Privileged access must be reviewed again after a role change.
- Temporary access must include an expiry date.
- Role changes should be completed by the effective transfer date.

## 3.5 Mover Process Result

The employee retains only the access required for the new role.

## 3.6 Why It Matters

A controlled Mover process prevents permission accumulation and reduces the risk of employees retaining outdated or conflicting access.

---

# 4. Leaver Process

## 4.1 Objective

The Leaver process ensures that access is removed promptly when an employee or contractor leaves the organisation.

## 4.2 Leaver Types

The process covers:

- Resignation
- Retirement
- Contract completion
- Dismissal
- Redundancy
- End of temporary assignment
- Long-term suspension
- Immediate termination

## 4.3 Standard Leaver Workflow

1. HR confirms the employee's final working date.
2. HR submits the termination notification.
3. The employee manager confirms:
   - Required data transfer
   - Ownership of documents
   - Return of company assets
   - Removal from shared resources
4. IT identifies all user accounts and assigned access.
5. IT schedules account disablement for the approved departure time.
6. Active sessions are terminated.
7. VPN and remote access are disabled.
8. Microsoft 365 access is blocked.
9. Active Directory accounts are disabled.
10. Application accounts are disabled or removed.
11. Administrative accounts are disabled immediately.
12. Security groups and mailing lists are removed.
13. Company devices, tokens and access cards are returned.
14. Mailbox and files are transferred where approved.
15. IT records evidence of all completed actions.
16. The manager and HR confirm completion.

## 4.4 Immediate-Termination Workflow

For high-risk or involuntary departures:

1. HR informs only authorised personnel.
2. IT prepares account disablement before the termination meeting.
3. All accounts are disabled at the approved time.
4. Active sessions are terminated immediately.
5. Physical access is revoked.
6. Company equipment is recovered.
7. Information Security reviews recent activity where required.
8. Evidence is retained.

## 4.5 Leaver Control Requirements

- HR must provide the official termination instruction.
- Accounts must be disabled at the approved departure time.
- Immediate terminations require coordinated access removal.
- Privileged accounts must receive priority.
- Shared credentials known by the departing user must be changed.
- Company assets must be recovered.
- Access-removal evidence must be retained.
- Deleted accounts must follow the approved retention period.

## 4.6 Leaver Process Result

The former employee can no longer access company systems or information.

## 4.7 Why It Matters

A controlled Leaver process prevents orphaned accounts, unauthorised access and misuse of company information after employment ends.

---

# 5. Access Request and Approval Form

## Request Information

| Field | Required Information |
|---|---|
| Request ID | Unique request reference |
| Request Type | Joiner, Mover, Temporary Access or Other |
| Employee Name | Full name |
| Employee ID | Unique employee identifier |
| Department | Employee department |
| Job Title | Approved job title |
| Manager | Employee manager |
| Employment Type | Permanent, temporary or contractor |
| Start or Effective Date | Date access is required |
| End Date | Required for temporary access |

## Access Requested

| System | Requested Role or Permission | Business Justification | Access Level |
|---|---|---|---|
|  |  |  | Standard / Departmental / Sensitive / Privileged |
|  |  |  |  |
|  |  |  |  |

## Approval Section

| Approval Role | Name | Decision | Date |
|---|---|---|---|
| Employee Manager |  | Approve / Reject |  |
| System Owner |  | Approve / Reject / Not Required |  |
| Information Security |  | Approve / Reject / Not Required |  |
| IT Provisioning Officer |  | Completed / Returned |  |

## Approval Conditions

- Access must match the approved business need.
- Temporary access must include an expiry date.
- Privileged access requires independent approval.
- IT must not provision unapproved permissions.
- Rejected requests must include a reason.

---

# 6. Joiner Provisioning Checklist

| Check | Status | Evidence |
|---|---|---|
| HR record confirmed | Complete / Incomplete | HR notification |
| Employee ID verified | Complete / Incomplete | Employee record |
| Department and job role confirmed | Complete / Incomplete | HR record |
| Manager approval obtained | Complete / Incomplete | Approval record |
| System-owner approval obtained where required | Complete / N/A | Approval record |
| Security approval obtained where required | Complete / N/A | Approval record |
| Active Directory account created | Complete / N/A | Account record |
| Microsoft 365 licence assigned | Complete / N/A | Licence record |
| Approved groups assigned | Complete / N/A | Group-membership record |
| Application access provisioned | Complete / N/A | Application record |
| Multi-factor authentication enabled | Complete / N/A | MFA record |
| Initial password reset required | Complete / N/A | Account setting |
| Provisioning evidence retained | Complete / Incomplete | Ticket or request record |
| Manager confirmation completed | Complete / Incomplete | Confirmation record |

---

# 7. Mover Access Modification Checklist

| Check | Status | Evidence |
|---|---|---|
| HR role change confirmed | Complete / Incomplete | HR notification |
| Effective date confirmed | Complete / Incomplete | HR record |
| Previous-role access identified | Complete / Incomplete | Access report |
| New-role access approved | Complete / Incomplete | Approval record |
| System-owner approval obtained | Complete / N/A | Approval record |
| Segregation-of-duties check completed | Complete / Incomplete | SoD review |
| Previous department groups removed | Complete / N/A | Group record |
| Previous application access removed | Complete / N/A | Application record |
| New groups assigned | Complete / N/A | Group record |
| New application access assigned | Complete / N/A | Application record |
| Privileged access reviewed | Complete / N/A | Security review |
| Temporary access expiry recorded | Complete / N/A | Expiry record |
| Modification evidence retained | Complete / Incomplete | Ticket record |
| New manager confirmed access | Complete / Incomplete | Confirmation record |

---

# 8. Account Termination Checklist

| Check | Status | Evidence |
|---|---|---|
| HR termination instruction received | Complete / Incomplete | HR notification |
| Final working date confirmed | Complete / Incomplete | HR record |
| Active Directory account disabled | Complete / N/A | Account record |
| Microsoft 365 sign-in blocked | Complete / N/A | Account record |
| VPN access disabled | Complete / N/A | VPN record |
| Application accounts disabled | Complete / N/A | Application records |
| Administrative accounts disabled | Complete / N/A | Privileged-account record |
| Active sessions terminated | Complete / N/A | Security record |
| Group memberships removed | Complete / N/A | Group record |
| Mailbox and files transferred | Complete / N/A | Manager approval |
| Shared passwords changed | Complete / N/A | Change record |
| Devices and tokens returned | Complete / N/A | Asset record |
| Physical access removed | Complete / N/A | Access-card record |
| Evidence retained | Complete / Incomplete | Termination ticket |
| HR and manager confirmation received | Complete / Incomplete | Completion record |

---

# 9. Sample Employee Scenarios

## Scenario 1: New Finance Employee

### Employee Information

- Name: Daniel Mensah
- Employee ID: MCS-241
- Department: Finance
- Job Title: Accounts Payable Officer
- Manager: Finance Operations Manager
- Employment Type: Permanent

### Requested Access

- Active Directory standard account
- Microsoft 365
- Finance departmental folder
- Finance System payment-entry role
- VPN access

### Approval Decision

The manager approves the standard and departmental access.

The Finance System owner approves payment-entry access.

Payment-approval access is not granted because the employee creates payment records. This prevents a segregation-of-duties conflict.

### Result

Daniel receives payment-entry access but cannot approve his own payments.

### Why It Matters

The decision applies least privilege and prevents one employee from creating and approving the same financial transaction.

## Scenario 2: Employee Moves from Sales to Compliance

### Employee Information

- Name: Akosua Boateng
- Employee ID: MCS-184
- Previous Department: Sales
- New Department: Compliance
- Previous Role: Sales Executive
- New Role: Compliance Analyst

### Required Changes

Remove:

- CRM sales-edit access
- Sales departmental folder
- Sales mailing lists

Add:

- CRM read-only access
- Compliance departmental folder
- Compliance reporting access

### Result

Sales permissions are removed before Compliance access is assigned.

### Why It Matters

The process prevents Akosua from retaining unnecessary sales permissions after changing departments.

## Scenario 3: Departing IT Administrator

### Employee Information

- Name: Kwame Asare
- Employee ID: MCS-097
- Department: Information Technology
- Job Title: Systems Administrator
- Departure Type: Resignation

### Required Actions

- Disable standard account
- Disable separate administrator account
- Disable VPN access
- Terminate active sessions
- Remove administrative group memberships
- Recover company laptop and security token
- Transfer system documentation
- Change shared emergency credentials
- Review recent privileged activity

### Result

All standard and privileged access is disabled at the approved departure time.

### Why It Matters

Privileged users can make significant system changes. Their access must be removed promptly and fully documented.

---

# 10. Required Evidence

For every Joiner, Mover and Leaver event, retain:

- HR notification
- Access request
- Manager approval
- System-owner approval
- Information Security approval where required
- Provisioning or removal record
- Before-and-after access details
- Completion date and time
- Name of the IT officer
- Manager confirmation
- Exception approval where applicable

---

# 11. Expected Business Outcome

The Joiner, Mover and Leaver processes provide a consistent method for managing employee access.

They help the organisation:

- Grant appropriate access to new employees
- Remove outdated access after role changes
- Disable accounts when employees leave
- Prevent excessive permissions
- Maintain approval records
- Support audit testing
- Improve accountability
- Reduce orphaned and dormant accounts
