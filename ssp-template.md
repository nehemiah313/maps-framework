# System Security Plan Template (NIST SP 800-171 Rev. 2)

> **Created by AI Tech Pros (aitechpros.ai).** Free 90-second SPRS estimator: https://aitechpros.ai/sprs-score. The Readiness Room newsletter: https://thereadinessroom.substack.com

## How to use this template

Replace every `[bracketed placeholder]` with your company's specifics. Delete nothing: an assessor expects to see all 14 families addressed, even the ones where your answer is "not applicable, here is why." Work through `cui-scoping-worksheet.md` first so your boundary is defined before you describe it in Section 2. Score only after the SSP is complete: no SSP means no valid score (see `HONEST-SCORING.md`). Review this document at least annually and whenever your CUI boundary changes, then have the CEO re-attest.

## 1. Document control

| Field | Value |
|---|---|
| System name | [Your system name, e.g. "Corporate CUI enclave"] |
| Version | [1.0] |
| Date | [YYYY-MM-DD] |
| Author | [Name, title] |
| Approver | [CEO name] |

### Version history

| Version | Date | Author | Change description |
|---|---|---|---|
| 0.1 | [date] | [name] | Initial draft |
| 1.0 | [date] | [name] | CEO review and attestation |

## 2. System description and CUI boundary

[Paste your boundary statement from `cui-scoping-worksheet.md`. Describe what the system does, who uses it, and what types of CUI it handles. Name the facilities involved. If any part of the boundary relies on segmentation (firewall rules, VLANs, access lists), describe the segmentation here.]

## 3. Roles and responsibilities

| Role | Name | Responsibility |
|---|---|---|
| System Owner | [name] | Accountable for the system and this SSP |
| IT / Security lead | [name] | Implements and maintains the technical controls |
| CEO | [name] | Reviews and attests to this SSP |
| All CUI users | [roster or group] | Follow handling procedures, complete training |

## 4. Control implementation statements

For each control: state whether it is Implemented, Planned, or N/A; describe HOW it is met in this environment (name the specific system, tool, policy, or process, not just "we do this"); say where an assessor finds the evidence; and reference the POA&M item if one exists. Vague statements fail. "Access is restricted" fails. "Access to the engineering share is restricted to the Engineering AD group; reviewed quarterly by the IT lead; evidence in ticket SYS-1042" passes.


### Family 3.1: Access Control (22 controls)

#### 3.1.1: Limit system access to authorized users, processes acting on behalf of authorized users, and devices (including other systems).
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.1.2: Limit system access to the types of transactions and functions that authorized users are permitted to execute.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.1.3: Control the flow of CUI in accordance with approved authorizations.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.1.4: Separate the duties of individuals to reduce the risk of malevolent activity without collusion.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.1.5: Employ the principle of least privilege, including for specific security functions and privileged accounts.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.1.6: Use non-privileged accounts or roles when accessing nonsecurity functions.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.1.7: Prevent non-privileged users from executing privileged functions and capture the execution of such functions in audit logs.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.1.8: Limit unsuccessful logon attempts.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.1.9: Provide privacy and security notices consistent with applicable CUI rules.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.1.10: Use session lock with pattern-hiding displays to prevent access and viewing of data after a period of inactivity.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.1.11: Terminate (automatically) a user session after a defined condition.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.1.12: Monitor and control remote access sessions.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.1.13: Employ cryptographic mechanisms to protect the confidentiality of remote access sessions.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.1.14: Route remote access via managed access control points.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.1.15: Authorize remote execution of privileged commands and remote access to security-relevant information.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.1.16: Authorize wireless access prior to allowing such connections.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.1.17: Protect wireless access using authentication and encryption.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.1.18: Control and monitor mobile device access.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.1.19: Encrypt CUI on mobile devices and mobile computing platforms.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.1.20: Verify and control/limit connections to and use of external systems.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.1.21: Limit use of portable storage devices on external systems.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.1.22: Control CUI posted or processed on publicly accessible systems.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

### Family 3.2: Awareness and Training (3 controls)

#### 3.2.1: Ensure that managers, systems administrators, and users of organizational systems are made aware of the security risks associated with their activities and of the applicable policies, standards, and procedures related to the security of those systems.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.2.2: Ensure that personnel are trained to carry out their assigned information security-related duties and responsibilities.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.2.3: Provide security awareness training on recognizing and reporting potential indicators of insider threat.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

### Family 3.3: Audit and Accountability (9 controls)

#### 3.3.1: Create and retain system audit logs and records to the extent needed to enable the monitoring, analysis, investigation, and reporting of unlawful or unauthorized system activity.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.3.2: Ensure that the actions of individual system users can be uniquely traced to those users so they can be held accountable for their actions.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.3.3: Review and update logged events.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.3.4: Alert in the event of an audit logging process failure.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.3.5: Correlate audit review, analysis, and reporting processes for investigation and response to indications of inappropriate, suspicious, or unusual activity.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.3.6: Provide audit reduction and report generation to support on-demand analysis and reporting.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.3.7: Provide a system capability that compares and synchronizes internal system clocks with an authoritative source to generate time stamps for audit records.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.3.8: Protect audit information and audit logging tools from unauthorized access, modification, and deletion.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.3.9: Limit management of audit logging functionality to a subset of privileged users.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

### Family 3.4: Configuration Management (9 controls)

#### 3.4.1: Establish and maintain baseline configurations and inventories of organizational systems (including hardware, software, firmware, and documentation) throughout the respective system development life cycles.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.4.2: Establish and enforce security configuration settings for information technology products employed in organizational systems.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.4.3: Track, review, approve or disapprove, and log changes to organizational systems.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.4.4: Analyze the security impact of changes prior to implementation.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.4.5: Define, document, approve, and enforce physical and logical access restrictions associated with changes to organizational systems.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.4.6: Employ the principle of least functionality by configuring organizational systems to provide only essential capabilities.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.4.7: Restrict, disable, or prevent the use of nonessential programs, functions, ports, protocols, and services.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.4.8: Apply deny-by-exception (blacklisting) policy to prevent the use of unauthorized software; or apply allow-by-exception (whitelisting) policy to allow the execution of authorized software.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.4.9: Control and monitor user-installed software.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

### Family 3.5: Identification and Authentication (11 controls)

#### 3.5.1: Identify system users, processes acting on behalf of users, and devices.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.5.2: Authenticate (or verify) the identities of those users, processes, or devices, as a prerequisite to allowing access to organizational systems.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.5.3: Use multifactor authentication for local and network access to privileged accounts and for network access to non-privileged accounts.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.5.4: Employ replay-resistant authentication mechanisms for network access to privileged and non-privileged accounts.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.5.5: Prevent reuse of identifiers for a defined period.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.5.6: Disable identifiers after a defined period of inactivity.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.5.7: Enforce a minimum password complexity and change of characters when new passwords are created.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.5.8: Prohibit password reuse for a specified number of generations.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.5.9: Allow temporary password use for system logons with an immediate change to a permanent password.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.5.10: Store and transmit only cryptographically-protected passwords.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.5.11: Obscure feedback of authentication information.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

### Family 3.6: Incident Response (3 controls)

#### 3.6.1: Establish an operational incident-handling capability for organizational systems that includes preparation, detection, analysis, containment, recovery, and user response activities.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.6.2: Track, document, and report incidents to designated officials and/or authorities both internal and external to the organization.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.6.3: Test the organizational incident response capability.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

### Family 3.7: Maintenance (6 controls)

#### 3.7.1: Perform maintenance on organizational systems.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.7.2: Provide controls on the tools, techniques, mechanisms, and personnel used to conduct system maintenance.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.7.3: Ensure equipment removed for off-site maintenance is sanitized of any CUI.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.7.4: Check media containing diagnostic and test programs for malicious code before the media are used in organizational systems.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.7.5: Require multifactor authentication to establish nonlocal maintenance sessions via external network connections and terminate such connections when nonlocal maintenance is complete.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.7.6: Supervise the maintenance activities of personnel without required access authorization.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

### Family 3.8: Media Protection (9 controls)

#### 3.8.1: Protect and control [organization-defined types of] system media.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.8.2: Limit access to CUI on system media to authorized users.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.8.3: Sanitize or destroy system media containing CUI prior to disposal or release for reuse.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.8.4: Mark media with necessary CUI markings and distribution limitations.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.8.5: Control access to media containing CUI.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.8.6: Control the use of removable media on system components.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.8.7: Prohibit the use of portable storage devices when such devices have no identifiable owner.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.8.8: Protect the authenticity of media during transport.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.8.9: Protect and control [organization-defined types of] backup media.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

### Family 3.9: Personnel Security (2 controls)

#### 3.9.1: Screen individuals prior to authorizing access to organizational systems containing CUI.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.9.2: Ensure that organizational systems containing CUI are protected during and after personnel actions such as terminations and transfers.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

### Family 3.10: Physical Protection (6 controls)

#### 3.10.1: Limit physical access to organizational systems, equipment, and the respective operating environments to authorized individuals.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.10.2: Protect and monitor the physical facility and support infrastructure for organizational systems.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.10.3: Escort visitors and monitor visitor activity.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.10.4: Maintain audit logs of physical access.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.10.5: Control and manage physical access devices.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.10.6: Enforce safeguarding measures for CUI at alternate work sites.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

### Family 3.11: Risk Assessment (3 controls)

#### 3.11.1: Periodically assess the risk to organizational operations (including mission, functions, image, or reputation), organizational assets, and individuals, resulting from the operation of organizational systems and the associated processing, storage, or transmission of CUI.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.11.2: Scan for vulnerabilities in organizational systems and applications periodically and when new vulnerabilities affecting those systems and applications are identified.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.11.3: Remediate vulnerabilities in accordance with risk assessments.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

### Family 3.12: Security Assessment (4 controls)

#### 3.12.1: Periodically assess the security controls in organizational systems to determine if the controls are effective in their application.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.12.2: Develop and implement plans of action designed to correct deficiencies and reduce or eliminate vulnerabilities in organizational systems.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.12.3: Monitor security controls on an ongoing basis to ensure the continued effectiveness of the controls.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.12.4: Develop, document, and periodically update system security plans that describe system boundaries, system environments of operation, how security requirements are met, and the relationships with or connections to other systems.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

### Family 3.13: System and Communications Protection (16 controls)

#### 3.13.1: Monitor, control, and protect communications (i.e., information transmitted or received by organizational systems) at the external boundaries and key internal boundaries of organizational systems.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.13.2: Employ architectural designs, software development techniques, and systems engineering principles that promote effective information security within organizational systems.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.13.3: Separate user functionality from system management functionality.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.13.4: Prevent unauthorized and unintended information transfer via shared system resources.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.13.5: Implement subnetworks for publicly accessible system components that are physically or logically separated from internal networks.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.13.6: Deny network communications traffic by default and allow network communications traffic by exception (i.e., deny all, permit by exception).
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.13.7: Prevent remote devices from simultaneously establishing non-remote connections with organizational systems and communicating via some other connection to resources in external networks (i.e., split tunneling).
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.13.8: Implement cryptographic mechanisms to prevent unauthorized disclosure of CUI during transmission unless otherwise protected by alternative physical safeguards.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.13.9: Terminate network connections associated with communications sessions at the end of the sessions or after a defined period of inactivity.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.13.10: Establish and manage cryptographic keys for cryptography employed in organizational systems.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.13.11: Employ FIPS-validated cryptography when used to protect the confidentiality of CUI.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.13.12: Prohibit remote activation of collaborative computing devices and provide indication of devices in use to users present at the device.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.13.13: Control and monitor the use of mobile code.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.13.14: Control and monitor the use of Voice over Internet Protocol (VoIP) technologies.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.13.15: Protect the authenticity of communications sessions.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.13.16: Protect the confidentiality of CUI at rest.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

### Family 3.14: System and Information Integrity (7 controls)

#### 3.14.1: Identify, report, and correct information and information system flaws in a timely manner.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.14.2: Provide protection from malicious code at appropriate locations within organizational information systems.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.14.3: Monitor system security alerts and advisories and take action in response.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.14.4: Update malicious code protection mechanisms when new releases are available.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.14.5: Perform periodic scans of the information system and real-time scans of files from external sources as files are downloaded, opened, or executed.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.14.6: Monitor organizational systems, including inbound and outbound communications traffic, to detect attacks and indicators of potential attacks.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

#### 3.14.7: Identify unauthorized use of organizational systems.
- **Status:** [Implemented / Planned / N/A]
- **Implementation statement:** [How is this control met in this environment? Name the system, tool, policy, or process. If Planned, reference the POA&M item ID. If N/A, give the justification.]
- **Evidence:** [Where does an assessor find proof? Policy document name, configuration screenshot, log location, ticket number.]
- **POA&M reference:** [Item ID, or "none"]

## 5. POA&M summary

[Every control marked Planned above gets a row in your POA&M. Use `poam-template.csv`. The six never-deferrable controls (3.1.20, 3.1.22, 3.10.3, 3.10.4, 3.10.5, 3.12.4) can never sit on a POA&M: if any of them is Planned, stop and fix it before you post a score.]

## 6. Review and attestation

I, [CEO name], [title] of [company legal name], attest that this System Security Plan accurately describes the system, the CUI boundary, and the implementation status of the NIST SP 800-171 controls as of the date below, to the best of my knowledge.

| | |
|---|---|
| Signature | ______________________________ |
| Printed name | [CEO name] |
| Date | [YYYY-MM-DD] |

[Store the signed attestation with this SSP. Re-attest at least annually and after any material change to the CUI boundary.]
