# Risk, Audit and Executive Summary

## 1. Purpose

This document records the main IAM risks, recommended treatments, control mapping, audit evidence, performance indicators and final management recommendations for Meridian Crest Services Ltd.

It provides the final risk and governance view of the Joiner, Mover and Leaver process.

---

# 2. Risk Assessment Method

Each risk is assessed using:

- Likelihood: Rare, Unlikely, Possible, Likely or Almost Certain
- Impact: Insignificant, Minor, Moderate, Major or Severe
- Risk Level: Low, Medium, High or Critical

Risk ratings represent the level of exposure before and after recommended controls are applied.

---

# 3. IAM Risk Register

| Risk ID | Risk Description | Likelihood | Impact | Inherent Risk | Existing or Proposed Control | Residual Risk | Owner |
|---|---|---|---|---|---|---|---|
| IAM-001 | New employees receive excessive access | Likely | Major | High | RBAC, manager approval and system-owner approval | Medium | HR Manager and IT Manager |
| IAM-002 | Employees retain old access after changing roles | Likely | Major | High | Mover checklist, removal of previous access and manager confirmation | Medium | Employee Manager and IT Manager |
| IAM-003 | Former employees retain active accounts | Possible | Severe | Critical | HR termination notice, timed disablement and termination checklist | Low | HR Manager and IT Manager |
| IAM-004 | Access is provisioned without approval | Likely | Major | High | Mandatory access request and approval records | Medium | IT Manager |
| IAM-005 | Privileged access is misused | Possible | Severe | Critical | Separate administrator accounts, MFA, logging and monthly reviews | Medium | Information Security Manager |
| IAM-006 | Dormant accounts remain active | Likely | Moderate | High | Monthly dormant-account review and disablement | Low | IT Manager |
| IAM-007 | Segregation-of-duties conflicts are not detected | Possible | Major | High | SoD matrix, pre-provisioning review and quarterly recertification | Medium | Compliance Manager |
| IAM-008 | Access reviews are incomplete or unsupported by evidence | Likely | Moderate | High | Quarterly review template, completion tracking and escalation | Medium | Compliance Manager |
| IAM-009 | Account termination is delayed | Possible | Severe | Critical | Defined termination timelines and immediate escalation | Low | HR Manager and IT Manager |
| IAM-010 | Temporary access remains active after expiry | Likely | Moderate | High | Mandatory expiry dates and monthly exception reviews | Low | System Owner |
| IAM-011 | IT personnel approve their own privileged access | Possible | Major | High | Independent Information Security approval | Low | Information Security Manager |
| IAM-012 | Shared accounts reduce accountability | Possible | Major | High | Named accounts and formal exception approval | Medium | IT Manager |

---

# 4. Risk Treatment Plan

| Risk ID | Treatment Action | Responsible Owner | Priority | Target Timeframe | Expected Result |
|---|---|---|---|---|---|
| IAM-001 | Implement approved RBAC profiles for standard job roles | IT Manager | High | 30 days | New employees receive consistent role-based access |
| IAM-002 | Require access removal before new-role access is confirmed | HR and IT Managers | High | Immediate | Outdated permissions are removed during transfers |
| IAM-003 | Disable all user access at the approved departure time | HR and IT Managers | Critical | Immediate | Former employees cannot access company systems |
| IAM-004 | Prevent provisioning without recorded approvals | IT Manager | High | 14 days | Every access action has valid authorisation |
| IAM-005 | Require separate privileged accounts, MFA and monthly review | Information Security Manager | Critical | 30 days | Privileged access is restricted and monitored |
| IAM-006 | Generate and review dormant-account reports monthly | IT Manager | Medium | 30 days | Unused accounts are investigated and disabled |
| IAM-007 | Check requested roles against the SoD matrix | Compliance Manager | High | 30 days | Conflicting access is detected before provisioning |
| IAM-008 | Track quarterly reviews and escalate overdue responses | Compliance Manager | High | Quarterly | Reviews are completed and supported by evidence |
| IAM-009 | Establish immediate escalation for delayed disablement | IT Manager | Critical | Immediate | Termination delays are resolved promptly |
| IAM-010 | Apply expiry dates to all temporary permissions | System Owners | High | 14 days | Temporary access is removed automatically or reviewed |
| IAM-011 | Separate approval and provisioning responsibilities | Information Security Manager | High | Immediate | IT staff cannot approve their own elevated access |
| IAM-012 | Replace shared accounts with named accounts where possible | IT Manager | Medium | 60 days | User activity can be linked to an individual |

---

# 5. Control Mapping

## 5.1 NIST Cybersecurity Framework 2.0 Mapping

| NIST CSF Function | Project Control | Application |
|---|---|---|
| Govern | IAM roles and responsibilities | Defines responsibility for HR, managers, system owners, IT, Security and Compliance |
| Identify | Systems and access classification | Identifies systems, information sensitivity and access owners |
| Protect | RBAC and least privilege | Restricts access according to approved business roles |
| Protect | Segregation of duties | Prevents conflicting access combinations |
| Protect | Privileged-access controls | Requires separate accounts, MFA, approval and monitoring |
| Protect | Joiner, Mover and Leaver processes | Controls account creation, modification and termination |
| Detect | Dormant-account monitoring | Identifies inactive and unused accounts |
| Detect | Privileged activity logging | Supports identification of suspicious administrative actions |
| Respond | Escalation procedure | Defines actions for former-employee accounts, misuse and control failures |
| Recover | Emergency-access control | Supports controlled restoration activities during emergencies |

## 5.2 ISO/IEC 27001 Access-Control Alignment

| Control Area | Project Application |
|---|---|
| Identity management | Unique user accounts and verified employee records |
| Access rights | Formal request, approval, provisioning and removal |
| Privileged access rights | Independent approval, separate accounts and periodic review |
| Information access restriction | Need-to-know and role-based permissions |
| Secure authentication | Password controls and multi-factor authentication |
| Segregation of duties | Prevention of conflicting business responsibilities |
| Logging and monitoring | Retention of account and privileged-access records |

This is a conceptual control alignment for portfolio demonstration. It is not a certification assessment.

---

# 6. Audit Evidence Checklist

| Evidence ID | Required Evidence | Source | Review Status |
|---|---|---|---|
| EVD-001 | Approved Joiner request | HR or access-management record | Available / Missing |
| EVD-002 | Manager approval | Access request record | Available / Missing |
| EVD-003 | System-owner approval | Access request record | Available / Missing |
| EVD-004 | Information Security approval | Privileged or exceptional-access record | Available / Missing |
| EVD-005 | Account creation evidence | Active Directory or application record | Available / Missing |
| EVD-006 | Assigned group and role evidence | System access report | Available / Missing |
| EVD-007 | Mover notification | HR role-change record | Available / Missing |
| EVD-008 | Previous-role access removal evidence | Access modification record | Available / Missing |
| EVD-009 | Leaver notification | HR termination record | Available / Missing |
| EVD-010 | Account-disablement timestamp | Active Directory or system record | Available / Missing |
| EVD-011 | Privileged-account review | Monthly review record | Available / Missing |
| EVD-012 | Quarterly access-review report | Access-review template | Available / Missing |
| EVD-013 | Recertification decisions | System-owner review record | Available / Missing |
| EVD-014 | SoD review result | SoD assessment record | Available / Missing |
| EVD-015 | Exception approval and expiry | Exception register | Available / Missing |
| EVD-016 | Escalation and resolution evidence | Security or compliance record | Available / Missing |
| EVD-017 | Dormant-account report | IT account report | Available / Missing |
| EVD-018 | User and manager completion confirmation | Access ticket or email record | Available / Missing |

## 6.1 Evidence Quality Tests

Audit evidence should be:

- Complete
- Readable
- Dated
- Linked to the correct employee
- Linked to the correct system
- Approved by the correct authority
- Consistent with the access provided
- Protected from unauthorised alteration
- Retained according to company requirements

---

# 7. Key Performance Indicators

KPIs measure whether the IAM process is operating effectively.

| KPI ID | Indicator | Target |
|---|---|---|
| KPI-001 | Joiner accounts completed by the approved start date | At least 95% |
| KPI-002 | Mover access changes completed by the effective date | At least 95% |
| KPI-003 | Standard leaver accounts disabled by the approved departure time | 100% |
| KPI-004 | Immediate-termination accounts disabled at the required time | 100% |
| KPI-005 | Quarterly access reviews completed by the due date | At least 95% |
| KPI-006 | Privileged accounts reviewed monthly | 100% |
| KPI-007 | Access requests containing complete approval evidence | 100% |
| KPI-008 | Temporary access removed or renewed before expiry | At least 95% |
| KPI-009 | High-risk access issues resolved within the required timeframe | At least 90% |
| KPI-010 | Access-review actions completed after reviewer decisions | At least 95% |

---

# 8. Key Risk Indicators

KRIs identify increasing IAM risk or possible control failure.

| KRI ID | Indicator | Warning Threshold | Escalation Threshold |
|---|---|---|---|
| KRI-001 | Active accounts belonging to former employees | 1 account | More than 1 account |
| KRI-002 | Dormant accounts inactive for more than 90 days | 5 accounts | More than 10 accounts |
| KRI-003 | Privileged accounts without valid approval | 1 account | More than 1 account |
| KRI-004 | Overdue quarterly access reviews | 5% overdue | More than 10% overdue |
| KRI-005 | Temporary access beyond expiry date | 2 cases | More than 5 cases |
| KRI-006 | Unresolved High-risk SoD conflicts | 1 conflict | More than 2 conflicts |
| KRI-007 | Leaver accounts disabled late | 1 case | More than 2 cases |
| KRI-008 | Access requests without complete evidence | 5% incomplete | More than 10% incomplete |
| KRI-009 | Shared accounts without approved exceptions | 1 account | More than 2 accounts |
| KRI-010 | Privileged accounts not reviewed monthly | 1 account | More than 1 account |

---

# 9. Sample Audit Test

## 9.1 Audit Objective

Determine whether employee access is approved, appropriate, reviewed and removed on time.

## 9.2 Sample Selection

Select a sample containing:

- Three Joiner records
- Three Mover records
- Three Leaver records
- Two privileged-access records
- One temporary-access exception
- One completed quarterly access review

## 9.3 Audit Procedures

For each selected record:

1. Confirm the employee identity and status.
2. Confirm the request was approved.
3. Compare provisioned access with the approved request.
4. Verify system-owner approval for sensitive access.
5. Verify Security approval for privileged access.
6. Confirm segregation-of-duties checks were completed.
7. Confirm temporary access has an expiry date.
8. Confirm role changes removed previous access.
9. Confirm leaver accounts were disabled on time.
10. Confirm evidence is complete and readable.

## 9.4 Possible Audit Findings

- Missing approval evidence
- Excessive access
- Previous-role permissions still active
- Former-employee accounts still enabled
- Delayed account disablement
- Privileged access without independent approval
- Expired temporary access
- Incomplete recertification
- Unresolved SoD conflicts
- Missing completion evidence

---

# 10. Executive Summary

Meridian Crest Services Ltd. requires a consistent and auditable method for managing employee access throughout the employment lifecycle.

The assessment identified significant risks involving excessive access, outdated permissions, former-employee accounts, privileged access, dormant accounts, segregation-of-duties conflicts and incomplete review evidence.

A complete Joiner, Mover and Leaver governance process was designed to address these risks.

The process requires:

- Verified HR information
- Manager approval
- System-owner approval
- Independent Security approval for privileged access
- Role-based access assignment
- Removal of previous-role access
- Timely account disablement
- Quarterly access reviews
- Monthly privileged-access reviews
- Access recertification
- Exception expiry dates
- Risk-based escalation
- Complete audit evidence

The highest-risk issue is the possibility of former employees or privileged users retaining active access. These risks require immediate and independently verified access removal.

Implementation of the proposed controls should reduce the likelihood of unauthorised, excessive, outdated and orphaned access.

---

# 11. Final Recommendations

Meridian Crest Services Ltd. should:

1. Adopt the documented Joiner, Mover and Leaver processes as the standard access-management procedure.
2. Require HR to initiate all employee lifecycle events.
3. Implement approved RBAC profiles for common job roles.
4. Prevent IT from provisioning access without documented approval.
5. Require system-owner approval for sensitive applications.
6. Require independent Information Security approval for privileged access.
7. Remove previous-role access during every employee transfer.
8. Disable all leaver accounts at the approved departure time.
9. Review privileged access monthly.
10. Conduct formal access reviews quarterly.
11. Investigate dormant accounts every month.
12. Apply expiry dates to temporary and exceptional access.
13. Use the SoD matrix before granting sensitive financial access.
14. Track overdue reviews and unresolved High-risk issues.
15. Retain complete evidence for every access action.

---

# 12. Business Impact

The proposed IAM process can help the organisation:

- Reduce unauthorised access
- Prevent permission accumulation
- Reduce fraud opportunities
- Improve privileged-access control
- Remove former-employee access promptly
- Improve audit readiness
- Strengthen accountability
- Improve compliance evidence
- Reduce operational access errors
- Protect confidential business and employee information

---

# 13. Limitations

This project is a documented simulation using a fictional organisation.

It does not include:

- Deployment of a commercial identity-governance platform
- Live Active Directory configuration
- Automated account provisioning
- Real employee information
- Real access-review records
- Production privileged-access monitoring
- Formal certification or compliance assessment

The project demonstrates process design, risk assessment and governance documentation.

---

# 14. Conclusion

The Joiner, Mover and Leaver access-governance process provides Meridian Crest Services Ltd. with a clear method for managing access throughout the employee lifecycle.

It defines how access is requested, approved, provisioned, modified, reviewed, recertified and revoked.

The project also establishes controls for role-based access, segregation of duties, privileged accounts, temporary exceptions, escalation and audit evidence.

These controls provide a practical foundation for reducing excessive, outdated, unauthorised and orphaned access.
