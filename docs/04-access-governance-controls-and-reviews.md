# Access Governance Controls and Reviews

## 1. Purpose

This document defines the access-governance controls used by Meridian Crest Services Ltd.

It covers:

- Role-Based Access Control
- Segregation of duties
- Privileged access
- Periodic access reviews
- Access recertification
- Access exceptions
- Escalation requirements
- Audit evidence

These controls support least privilege, need-to-know access and accountability.

---

# 2. Role-Based Access Control

## 2.1 Role-Based Access Control Matrix

Access is assigned according to approved job responsibilities rather than personal preference.

| Job Role | Microsoft 365 | Department Folder | HRIS | Payroll | Finance System | CRM | VPN | Privileged Access |
|---|---|---|---|---|---|---|---|---|
| HR Officer | Standard | HR Read/Write | HR Standard | No Access | No Access | No Access | Approved Need | No |
| HR Manager | Standard | HR Read/Write | HR Manager | Payroll Read-Only | No Access | No Access | Approved Need | No |
| Payroll Officer | Standard | Finance Read/Write | Limited HR View | Payroll Entry | Limited Finance View | No Access | Approved Need | No |
| Accounts Payable Officer | Standard | Finance Read/Write | No Access | No Access | Payment Entry | No Access | Approved Need | No |
| Finance Manager | Standard | Finance Read/Write | No Access | Payroll Approval | Finance Approval | No Access | Approved Need | No |
| Sales Executive | Standard | Sales Read/Write | No Access | No Access | No Access | Sales Edit | Approved Need | No |
| Compliance Analyst | Standard | Compliance Read/Write | Limited View | Approved Read-Only | Finance Read-Only | CRM Read-Only | Approved Need | No |
| IT Support Analyst | Standard | IT Read/Write | Technical Support Only | No Business Access | No Business Access | Technical Support Only | Yes | Limited |
| Systems Administrator | Standard | IT Read/Write | Technical Administration | Technical Administration | Technical Administration | Technical Administration | Yes | Yes |
| General Employee | Standard | Department Only | Self-Service Only | No Access | No Access | No Access | Approved Need | No |

## 2.2 RBAC Requirements

- Access must correspond to the employee’s current role.
- Department transfers require removal of previous-role access.
- Access outside the approved role requires documented justification.
- Sensitive access requires system-owner approval.
- Privileged access requires Information Security approval.
- Temporary access must include an expiry date.
- Managers must confirm access after provisioning.
- Access must be reviewed periodically.

## 2.3 Expected Result

Employees receive standard access based on their job responsibilities. Additional access requires separate approval and justification.

## 2.4 Why It Matters

Role-based access control reduces inconsistent, excessive and unnecessary permissions.

---

# 3. Segregation of Duties

## 3.1 Purpose

Segregation of duties prevents one person from controlling every stage of a sensitive transaction.

## 3.2 Segregation-of-Duties Matrix

| SoD ID | Access Combination | Conflict | Required Control |
|---|---|---|---|
| SOD-001 | Create vendor and approve vendor | A user could create and approve a fraudulent vendor | Assign the roles to different users |
| SOD-002 | Create payment and approve payment | A user could submit and approve an unauthorised payment | Separate payment-entry and approval roles |
| SOD-003 | Prepare payroll and approve payroll | A user could manipulate and approve payroll | Separate payroll preparation and approval |
| SOD-004 | Request access and approve the same request | A user could approve personal access | Require independent approval |
| SOD-005 | Provision privileged access and approve it | IT could grant itself elevated permissions | Require Information Security approval |
| SOD-006 | Create employee record and approve payroll change | A false employee record could be used for payment fraud | Separate HR administration and payroll approval |
| SOD-007 | Develop a system change and approve its production release | An unreviewed change could enter production | Require independent change approval |
| SOD-008 | Review and certify personal access | The access review would not be independent | Require another manager or system owner to certify |

## 3.3 SoD Review Decisions

When a conflict is identified, one of the following decisions must be recorded:

- Remove one of the conflicting permissions.
- Reassign responsibility to another employee.
- Apply an approved compensating control.
- Approve a time-limited exception.
- Reject the access request.

Unresolved High-risk conflicts must be escalated to Information Security and Compliance.

## 3.4 Expected Result

Conflicting responsibilities are identified before access is granted or during periodic access reviews.

## 3.5 Why It Matters

Segregation of duties reduces the likelihood of fraud, misuse and unauthorised transactions.

---

# 4. Privileged Access Procedure

## 4.1 Privileged Access Definition

Privileged access allows a user to:

- Create or disable accounts.
- Change user permissions.
- Modify security settings.
- Access sensitive system configurations.
- Install software.
- View restricted system information.
- Change audit or logging settings.
- Perform administrative system actions.

## 4.2 Privileged Access Requirements

Privileged access must:

1. Have a documented business justification.
2. Be approved by the employee manager.
3. Be approved by the system owner.
4. Be approved by Information Security.
5. Use a separate administrative account.
6. Use multi-factor authentication.
7. Be restricted to approved systems.
8. Be logged and monitored.
9. Be reviewed monthly.
10. Be removed when no longer required.

## 4.3 Privileged Account Naming

Administrative accounts should use a clear naming format.

Example: `adm-firstname.lastname`

The user’s normal account must not be used for administrative work.

## 4.4 Prohibited Activities

Privileged users must not:

- Share administrative credentials.
- Use administrative accounts for email or ordinary browsing.
- Disable logging without approval.
- Create unauthorised accounts.
- Approve their own privileged-access requests.
- Retain privileged access after changing roles.
- Use shared administrator accounts unless formally approved.

## 4.5 Emergency Access

Emergency access may be granted when immediate action is required to protect systems or restore services.

Emergency access must:

- Receive documented approval where possible.
- Be limited to the required system.
- Have a defined expiry time.
- Be logged.
- Be reviewed after use.
- Be removed immediately after the emergency ends.

## 4.6 Expected Result

Privileged access is restricted, independently approved, monitored and reviewed regularly.

## 4.7 Why It Matters

Privileged accounts can make major system changes. Strong controls reduce the risk of misuse and unauthorised administration.

---

# 5. Access Review Procedure

## 5.1 Review Frequency

| Access Type | Review Frequency | Reviewer |
|---|---|---|
| Standard employee access | Quarterly | Employee Manager |
| Departmental access | Quarterly | Department Manager |
| Sensitive application access | Quarterly | System Owner |
| Privileged access | Monthly | IT Manager and Information Security |
| Temporary access | Before expiry | Manager and System Owner |
| Dormant accounts | Monthly | IT and Information Security |
| Contractor access | Monthly or at contract end | Manager and HR |

## 5.2 Quarterly Access Review Process

1. IT generates a list of active accounts and permissions.
2. The list is sent to the responsible manager or system owner.
3. The reviewer compares access against:
   - Current employment status
   - Current department
   - Current job role
   - Business need
   - Approved access level
4. The reviewer selects one decision:
   - Retain
   - Modify
   - Revoke
   - Investigate
5. IT completes the approved access changes.
6. Evidence of completed actions is attached.
7. Compliance tracks overdue reviews.
8. Information Security escalates unresolved High-risk access.

## 5.3 Review Responsibilities

| Role | Responsibility |
|---|---|
| IT | Generates access reports and completes approved changes |
| Employee Manager | Reviews employee access against current duties |
| System Owner | Reviews sensitive system permissions |
| Information Security | Reviews privileged and High-risk access |
| Compliance | Tracks completion and verifies evidence |

## 5.4 Expected Result

Existing access is reviewed regularly and permissions that are outdated, excessive or unnecessary are corrected.

## 5.5 Why It Matters

Periodic reviews help identify dormant accounts, former employees, excessive access and access that no longer matches a user’s role.

---

# 6. Quarterly Access Review Template

## 6.1 Review Information

| Field | Information |
|---|---|
| Review ID |  |
| System |  |
| Review Period |  |
| System Owner |  |
| Reviewer |  |
| Review Start Date |  |
| Review Due Date |  |
| Completion Date |  |

## 6.2 User Access Review

| User | Department | Job Role | Current Access | Decision | Required Action | Reviewer Comment |
|---|---|---|---|---|---|---|
|  |  |  |  | Retain / Modify / Revoke / Investigate |  |  |
|  |  |  |  | Retain / Modify / Revoke / Investigate |  |  |
|  |  |  |  | Retain / Modify / Revoke / Investigate |  |  |

## 6.3 Review Completion

| Check | Status |
|---|---|
| All active users reviewed | Complete / Incomplete |
| Former employees identified | Yes / No |
| Dormant accounts identified | Yes / No |
| Excessive access identified | Yes / No |
| Privileged access reviewed | Yes / No |
| SoD conflicts identified | Yes / No |
| Required changes completed | Yes / No |
| Evidence attached | Yes / No |
| System owner certified review | Yes / No |

## 6.4 Required Evidence

The completed review must include:

- The original access report.
- Reviewer decisions.
- Comments explaining modifications or revocations.
- Evidence of completed access changes.
- Review completion date.
- System-owner certification.
- Escalation records for unresolved issues.

---

# 7. Access Recertification Process

## 7.1 Purpose

Access recertification formally confirms that existing permissions remain appropriate.

## 7.2 Recertification Requirements

The reviewer must confirm that:

- The user is still employed or under contract.
- The user belongs to the correct department.
- The access matches the current job role.
- The access remains necessary.
- Sensitive permissions remain justified.
- Privileged access remains necessary.
- No segregation-of-duties conflict exists.
- Temporary access has not expired.
- Dormant accounts are investigated.

## 7.3 Recertification Decisions

| Decision | Required Action |
|---|---|
| Recertify | Retain access with reviewer approval |
| Modify | Reduce or change permissions |
| Revoke | Remove access |
| Investigate | Suspend the decision and escalate for review |
| Exception | Record an approved temporary exception |

A lack of response is not considered approval.

## 7.4 Recertification Completion

The review is complete only when:

- Every account has a recorded decision.
- Required changes have been completed.
- Exceptions have approved expiry dates.
- Evidence has been retained.
- The system owner has certified the results.

## 7.5 Why It Matters

Recertification provides formal proof that managers and system owners reviewed and accepted continuing user access.

---

# 8. Exception Management Process

## 8.1 Exception Definition

An access exception occurs when requested access does not follow the standard role, approval or segregation-of-duties requirements.

Examples include:

- Temporary access outside the employee’s normal role.
- Emergency privileged access.
- A temporary segregation-of-duties conflict.
- Access to a restricted system.
- Use of a shared technical account.
- Continued access after a temporary assignment.

## 8.2 Exception Request Requirements

Every exception must include:

- Requester
- Affected user
- System and access requested
- Business justification
- Identified risk
- Reason the standard control cannot be followed
- Compensating control
- Start date
- Expiry date
- Manager approval
- System-owner approval
- Information Security approval

## 8.3 Exception Register

| Exception ID | User | System | Exception | Risk Level | Compensating Control | Expiry Date | Status |
|---|---|---|---|---|---|---|---|
| EXC-001 |  |  |  | Low / Medium / High |  |  | Open / Closed |
| EXC-002 |  |  |  | Low / Medium / High |  |  | Open / Closed |

## 8.4 Exception Monitoring

- Exceptions must have expiry dates.
- Open exceptions must be reviewed monthly.
- Expired exceptions must be removed or formally renewed.
- High-risk exceptions require Information Security approval.
- Exceptions must not remain open indefinitely.
- Compensating controls must be verified.

## 8.5 Why It Matters

Exception management prevents temporary or unusual access from becoming permanent and unmonitored.

---

# 9. Escalation Procedure

## 9.1 Escalation Triggers

An issue must be escalated when:

- A former employee account remains active.
- Privileged access lacks approval.
- A High-risk segregation-of-duties conflict is identified.
- An access review is overdue.
- A manager refuses to complete recertification.
- Temporary access passes its expiry date.
- A dormant privileged account is found.
- Access-removal evidence is missing.
- Suspicious privileged activity is detected.
- IT cannot complete urgent account disablement.

## 9.2 Escalation Levels

| Level | Issue | Escalation Recipient | Target Response |
|---|---|---|---|
| Level 1 | Standard access error | IT Service Desk and Manager | One business day |
| Level 2 | Sensitive access or overdue review | System Owner and Compliance | Same business day |
| Level 3 | Privileged access, former employee or High-risk SoD conflict | Information Security and IT Manager | Immediate |
| Level 4 | Suspected misuse, fraud or major control failure | Senior Management and Incident Response Team | Immediate |

## 9.3 Escalation Evidence

The escalation record must contain:

- Issue description
- Affected user and system
- Risk level
- Date and time identified
- Immediate action taken
- Person notified
- Required corrective action
- Resolution date
- Supporting evidence

## 9.4 Expected Result

High-risk access issues are communicated quickly to the appropriate decision-makers and tracked until resolved.

## 9.5 Why It Matters

Escalation prevents serious access-control failures from remaining unresolved.

---

# 10. Required Audit Evidence

The following evidence must be retained:

- Approved access requests
- Manager approvals
- System-owner approvals
- Information Security approvals
- RBAC assignments
- Segregation-of-duties review results
- Privileged-access records
- Monthly privileged-access reviews
- Quarterly access-review reports
- Recertification decisions
- Exception approvals
- Exception expiry records
- Escalation records
- Access modification evidence
- Access revocation evidence
- Dormant-account reports
- Former-employee account checks

## 10.1 Evidence Quality Requirements

Evidence must be:

- Complete
- Readable
- Dated
- Linked to the affected user
- Linked to the relevant system
- Approved by the correct authority
- Retained in the approved location
- Protected against unauthorised modification

---

# 11. Expected Business Result

These controls help Meridian Crest Services Ltd. ensure that:

- Employees receive access appropriate to their roles.
- Conflicting financial and administrative permissions are identified.
- Privileged access is independently approved and reviewed.
- Existing access is periodically recertified.
- Temporary exceptions expire.
- High-risk access issues are escalated.
- Access decisions are supported by evidence.
- Audit and compliance reviews can be completed efficiently.

---

# 12. Why It Matters

Strong access governance reduces the risk of excessive, outdated, unauthorised and orphaned access.

It also provides clear evidence that access decisions are approved, reviewed and corrected when necessary.
