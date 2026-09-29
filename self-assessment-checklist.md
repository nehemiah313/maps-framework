# NIST SP 800-171 Self-Assessment Checklist

Part of the MAPS framework by AI Tech Pros. Plain English, zero fluff.

## How scoring works

You start at 110. Every control you have not implemented subtracts its weight:
5, 3, or 1 point. Two controls (3.5.3 multifactor authentication and 3.13.11
FIPS-validated encryption) score 5 or 3 depending on how fully they are implemented.
The floor is -203. There is no extra credit.

Rules that decide everything:

- A POA&M does not raise your score. The score reflects what is implemented today.
- Partial implementation scores the same as not implemented, except the two specials above.
- Controls marked Not Applicable subtract nothing, with documented justification.
- No System Security Plan means no valid score. The methodology assesses the SSP.
- Six controls can never sit on a POA&M: 3.1.20, 3.1.22, 3.10.3, 3.10.4, 3.10.5, 3.12.4.

How to use this file: work through each control, check the box only when the control
is implemented with evidence you could show an assessor, and record your status in
`controls-assessment.csv`. Your score is 110 minus the weights of every unchecked control.

## 3.1 Access Control (22 controls)

- [ ] **3.1.1** (5 pts): Limit system access to authorized users, processes acting on behalf of authorized users, and devices (including other systems).
  - Assessor looks for: A current list of authorized users and devices, and proof that only those can access systems.

- [ ] **3.1.2** (5 pts): Limit system access to the types of transactions and functions that authorized users are permitted to execute.
  - Assessor looks for: Role definitions showing each user can only run the transactions their job needs.

- [ ] **3.1.3** (1 pts): Control the flow of CUI in accordance with approved authorizations.
  - Assessor looks for: A diagram or policy showing where CUI is allowed to flow, with technical enforcement behind it.

- [ ] **3.1.4** (1 pts): Separate the duties of individuals to reduce the risk of malevolent activity without collusion.
  - Assessor looks for: Evidence that no one person can both execute and approve sensitive actions without a second set of eyes.

- [ ] **3.1.5** (3 pts): Employ the principle of least privilege, including for specific security functions and privileged accounts.
  - Assessor looks for: Admin accounts limited to the fewest people possible, with a periodic review record.

- [ ] **3.1.6** (1 pts): Use non-privileged accounts or roles when accessing nonsecurity functions.
  - Assessor looks for: Proof that daily work happens on standard accounts, not admin accounts.

- [ ] **3.1.7** (1 pts): Prevent non-privileged users from executing privileged functions and capture the execution of such functions in audit logs.
  - Assessor looks for: System settings that block standard users from privileged functions, plus logs capturing any attempts.

- [ ] **3.1.8** (1 pts): Limit unsuccessful logon attempts.
  - Assessor looks for: Lockout configured (for example, after 5 failed attempts), demonstrated on endpoints and key systems.

- [ ] **3.1.9** (1 pts): Provide privacy and security notices consistent with applicable CUI rules.
  - Assessor looks for: Logon banners or notices displayed before access, consistent with CUI handling rules.

- [ ] **3.1.10** (1 pts): Use session lock with pattern-hiding displays to prevent access and viewing of data after a period of inactivity.
  - Assessor looks for: Session lock enabled with hidden screen contents after inactivity, verified on endpoints.

- [ ] **3.1.11** (1 pts): Terminate (automatically) a user session after a defined condition.
  - Assessor looks for: Sessions that terminate automatically after a defined idle period or condition.

- [ ] **3.1.12** (5 pts): Monitor and control remote access sessions.
  - Assessor looks for: Remote access sessions logged, and able to be monitored or terminated.

- [ ] **3.1.13** (5 pts): Employ cryptographic mechanisms to protect the confidentiality of remote access sessions.
  - Assessor looks for: Remote sessions encrypted (VPN or equivalent), with the mechanism named.

- [ ] **3.1.14** (1 pts): Route remote access via managed access control points.
  - Assessor looks for: Remote access routed through managed entry points, not direct connections.

- [ ] **3.1.15** (1 pts): Authorize remote execution of privileged commands and remote access to security-relevant information.
  - Assessor looks for: Written authorization required before anyone runs privileged commands remotely.

- [ ] **3.1.16** (5 pts): Authorize wireless access prior to allowing such connections.
  - Assessor looks for: A record authorizing each wireless network before it carries CUI.

- [ ] **3.1.17** (5 pts): Protect wireless access using authentication and encryption.
  - Assessor looks for: Wireless protected with strong authentication and encryption (WPA2 or WPA3 enterprise, not open networks or home pre-shared keys).

- [ ] **3.1.18** (5 pts): Control and monitor mobile device access.
  - Assessor looks for: Mobile devices enrolled in management or otherwise controlled and monitored.

- [ ] **3.1.19** (3 pts): Encrypt CUI on mobile devices and mobile computing platforms.
  - Assessor looks for: CUI encrypted on phones, tablets, and laptops.

- [ ] **3.1.20** (1 pts) **NEVER DEFERRABLE**: Verify and control/limit connections to and use of external systems.
  - Assessor looks for: A list of approved external systems and connections, with unauthorized ones blocked. Never deferrable.

- [ ] **3.1.21** (1 pts): Limit use of portable storage devices on external systems.
  - Assessor looks for: Policy and enforcement limiting USB drives and portable storage on external systems.

- [ ] **3.1.22** (1 pts) **NEVER DEFERRABLE**: Control CUI posted or processed on publicly accessible systems.
  - Assessor looks for: Proof that no CUI sits on public-facing systems, or the controls protecting it there. Never deferrable.

## 3.2 Awareness and Training (3 controls)

- [ ] **3.2.1** (5 pts): Ensure that managers, systems administrators, and users of organizational systems are made aware of the security risks associated with their activities and of the applicable policies, standards, and procedures related to the security of those systems.
  - Assessor looks for: Training records showing managers, admins, and users were informed of their security responsibilities.

- [ ] **3.2.2** (5 pts): Ensure that personnel are trained to carry out their assigned information security-related duties and responsibilities.
  - Assessor looks for: Role-based training records for people with assigned security duties.

- [ ] **3.2.3** (1 pts): Provide security awareness training on recognizing and reporting potential indicators of insider threat.
  - Assessor looks for: Security awareness training covering phishing and insider threats, with completion records.

## 3.3 Audit and Accountability (9 controls)

- [ ] **3.3.1** (5 pts): Create and retain system audit logs and records to the extent needed to enable the monitoring, analysis, investigation, and reporting of unlawful or unauthorized system activity.
  - Assessor looks for: Audit logs actually being generated and retained for systems handling CUI.

- [ ] **3.3.2** (3 pts): Ensure that the actions of individual system users can be uniquely traced to those users so they can be held accountable for their actions.
  - Assessor looks for: Logs that tie every action to an individual user. No shared anonymous accounts.

- [ ] **3.3.3** (1 pts): Review and update logged events.
  - Assessor looks for: A defined list of auditable events that is reviewed and kept current.

- [ ] **3.3.4** (1 pts): Alert in the event of an audit logging process failure.
  - Assessor looks for: Alerts that fire when logging itself fails, so a blind spot gets noticed.

- [ ] **3.3.5** (5 pts): Correlate audit review, analysis, and reporting processes for investigation and response to indications of inappropriate, suspicious, or unusual activity.
  - Assessor looks for: Audit data from different sources correlated for investigations, not sitting in isolated silos.

- [ ] **3.3.6** (1 pts): Provide audit reduction and report generation to support on-demand analysis and reporting.
  - Assessor looks for: The ability to reduce and report on audit data on demand for analysis.

- [ ] **3.3.7** (1 pts): Provide a system capability that compares and synchronizes internal system clocks with an authoritative source to generate time stamps for audit records.
  - Assessor looks for: System clocks synchronized to a common time source so log timestamps line up.

- [ ] **3.3.8** (1 pts): Protect audit information and audit logging tools from unauthorized access, modification, and deletion.
  - Assessor looks for: Audit logs protected from tampering, deletion, or unauthorized viewing.

- [ ] **3.3.9** (1 pts): Limit management of audit logging functionality to a subset of privileged users.
  - Assessor looks for: Only a small set of privileged users can change logging settings.

## 3.4 Configuration Management (9 controls)

- [ ] **3.4.1** (5 pts): Establish and maintain baseline configurations and inventories of organizational systems (including hardware, software, firmware, and documentation) throughout the respective system development life cycles.
  - Assessor looks for: Baseline configurations documented for every system, plus a current hardware and software inventory.

- [ ] **3.4.2** (5 pts): Establish and enforce security configuration settings for information technology products employed in organizational systems.
  - Assessor looks for: Security hardening settings applied and enforced on systems and devices.

- [ ] **3.4.3** (1 pts): Track, review, approve or disapprove, and log changes to organizational systems.
  - Assessor looks for: A change log showing changes were reviewed and approved before implementation.

- [ ] **3.4.4** (1 pts): Analyze the security impact of changes prior to implementation.
  - Assessor looks for: Security impact considered before changes go live, not after.

- [ ] **3.4.5** (5 pts): Define, document, approve, and enforce physical and logical access restrictions associated with changes to organizational systems.
  - Assessor looks for: Physical and logical access restrictions on who can change system configurations.

- [ ] **3.4.6** (5 pts): Employ the principle of least functionality by configuring organizational systems to provide only essential capabilities.
  - Assessor looks for: Least functionality: only needed services and ports enabled, the rest off.

- [ ] **3.4.7** (5 pts): Restrict, disable, or prevent the use of nonessential programs, functions, ports, protocols, and services.
  - Assessor looks for: Nonessential programs, functions, and services disabled or removed.

- [ ] **3.4.8** (5 pts): Apply deny-by-exception (blacklisting) policy to prevent the use of unauthorized software; or apply allow-by-exception (whitelisting) policy to allow the execution of authorized software.
  - Assessor looks for: A blacklist policy blocking unauthorized software, with enforcement in place.

- [ ] **3.4.9** (1 pts): Control and monitor user-installed software.
  - Assessor looks for: User-installed software controlled and monitored, not a free-for-all.

## 3.5 Identification and Authentication (11 controls)

- [ ] **3.5.1** (5 pts): Identify system users, processes acting on behalf of users, and devices.
  - Assessor looks for: Every user, process, and device identified before being granted access.

- [ ] **3.5.2** (5 pts): Authenticate (or verify) the identities of those users, processes, or devices, as a prerequisite to allowing access to organizational systems.
  - Assessor looks for: Identities verified (authenticated) before access is granted.

- [ ] **3.5.3** (5 or 3 pts (see scoring)): Use multifactor authentication for local and network access to privileged accounts and for network access to non-privileged accounts.
  - Assessor looks for: MFA on privileged and network access at minimum. Full marks only with MFA for all users. Special scoring: 5 or 3.

- [ ] **3.5.4** (1 pts): Employ replay-resistant authentication mechanisms for network access to privileged and non-privileged accounts.
  - Assessor looks for: Authentication resistant to replay attacks for network access to privileged accounts.

- [ ] **3.5.5** (1 pts): Prevent reuse of identifiers for a defined period.
  - Assessor looks for: Old usernames and identifiers not recycled for a defined period.

- [ ] **3.5.6** (1 pts): Disable identifiers after a defined period of inactivity.
  - Assessor looks for: Dormant accounts disabled after a defined period of inactivity.

- [ ] **3.5.7** (1 pts): Enforce a minimum password complexity and change of characters when new passwords are created.
  - Assessor looks for: Password complexity enforced (length, character mix) on account creation and changes.

- [ ] **3.5.8** (1 pts): Prohibit password reuse for a specified number of generations.
  - Assessor looks for: Password history enforced so users cannot rotate between the same few passwords.

- [ ] **3.5.9** (1 pts): Allow temporary password use for system logons with an immediate change to a permanent password.
  - Assessor looks for: Temporary passwords that force an immediate change on first use.

- [ ] **3.5.10** (5 pts): Store and transmit only cryptographically-protected passwords.
  - Assessor looks for: Passwords stored hashed and transmitted encrypted, never in clear text.

- [ ] **3.5.11** (1 pts): Obscure feedback of authentication information.
  - Assessor looks for: Login screens that mask password entry, so no one can read it over a shoulder.

## 3.6 Incident Response (3 controls)

- [ ] **3.6.1** (5 pts): Establish an operational incident-handling capability for organizational systems that includes preparation, detection, analysis, containment, recovery, and user response activities.
  - Assessor looks for: A working incident response capability: named people, a plan, and a way to reach them.

- [ ] **3.6.2** (5 pts): Track, document, and report incidents to designated officials and/or authorities both internal and external to the organization.
  - Assessor looks for: Incidents tracked, documented, and reported to the right officials, including the 72-hour DoD report when required.

- [ ] **3.6.3** (1 pts): Test the organizational incident response capability.
  - Assessor looks for: The incident response plan actually tested, with lessons recorded.

## 3.7 Maintenance (6 controls)

- [ ] **3.7.1** (3 pts): Perform maintenance on organizational systems.
  - Assessor looks for: Maintenance performed on schedule, with records of what was done.

- [ ] **3.7.2** (5 pts): Provide controls on the tools, techniques, mechanisms, and personnel used to conduct system maintenance.
  - Assessor looks for: Controls over who performs maintenance, what tools they bring, and how it is supervised.

- [ ] **3.7.3** (1 pts): Ensure equipment removed for off-site maintenance is sanitized of any CUI.
  - Assessor looks for: Equipment sanitized of CUI before it leaves for off-site maintenance.

- [ ] **3.7.4** (3 pts): Check media containing diagnostic and test programs for malicious code before the media are used in organizational systems.
  - Assessor looks for: Diagnostic media and tools checked for malware before use.

- [ ] **3.7.5** (5 pts): Require multifactor authentication to establish nonlocal maintenance sessions via external network connections and terminate such connections when nonlocal maintenance is complete.
  - Assessor looks for: MFA required for remote (nonlocal) maintenance sessions.

- [ ] **3.7.6** (1 pts): Supervise the maintenance activities of personnel without required access authorization.
  - Assessor looks for: Maintenance by personnel without required access supervised, with activity records.

## 3.8 Media Protection (9 controls)

- [ ] **3.8.1** (3 pts): Protect and control [organization-defined types of] system media.
  - Assessor looks for: System media (drives, USB sticks, printouts) protected and controlled by type.

- [ ] **3.8.2** (3 pts): Limit access to CUI on system media to authorized users.
  - Assessor looks for: Access to CUI on media limited to authorized users.

- [ ] **3.8.3** (5 pts): Sanitize or destroy system media containing CUI prior to disposal or release for reuse.
  - Assessor looks for: Media sanitized or destroyed before disposal or reuse, with a record of it.

- [ ] **3.8.4** (1 pts): Mark media with necessary CUI markings and distribution limitations.
  - Assessor looks for: Media marked with CUI markings and distribution limits.

- [ ] **3.8.5** (1 pts): Control access to media containing CUI.
  - Assessor looks for: Physical control over who can access media containing CUI.

- [ ] **3.8.6** (1 pts): Control the use of removable media on system components.
  - Assessor looks for: Rules and enforcement for removable media plugged into systems.

- [ ] **3.8.7** (5 pts): Prohibit the use of portable storage devices when such devices have no identifiable owner.
  - Assessor looks for: Portable storage devices with no identifiable owner prohibited.

- [ ] **3.8.8** (3 pts): Protect the authenticity of media during transport.
  - Assessor looks for: Media protected from tampering or interception during transport.

- [ ] **3.8.9** (1 pts): Protect and control [organization-defined types of] backup media.
  - Assessor looks for: Backup media protected and controlled like production media.

## 3.9 Personnel Security (2 controls)

- [ ] **3.9.1** (3 pts): Screen individuals prior to authorizing access to organizational systems containing CUI.
  - Assessor looks for: Background screening completed before people get access to systems with CUI.

- [ ] **3.9.2** (5 pts): Ensure that organizational systems containing CUI are protected during and after personnel actions such as terminations and transfers.
  - Assessor looks for: Access revoked promptly when people transfer roles or leave.

## 3.10 Physical Protection (6 controls)

- [ ] **3.10.1** (5 pts): Limit physical access to organizational systems, equipment, and the respective operating environments to authorized individuals.
  - Assessor looks for: Physical access to systems and equipment limited to authorized individuals.

- [ ] **3.10.2** (5 pts): Protect and monitor the physical facility and support infrastructure for organizational systems.
  - Assessor looks for: The facility and its support infrastructure (power, network closets) protected and monitored.

- [ ] **3.10.3** (1 pts) **NEVER DEFERRABLE**: Escort visitors and monitor visitor activity.
  - Assessor looks for: Visitors escorted and their activity monitored. Never deferrable.

- [ ] **3.10.4** (1 pts) **NEVER DEFERRABLE**: Maintain audit logs of physical access.
  - Assessor looks for: Logs of who entered secure areas and when. Never deferrable.

- [ ] **3.10.5** (1 pts) **NEVER DEFERRABLE**: Control and manage physical access devices.
  - Assessor looks for: Badges, keys, and access devices controlled and managed. Never deferrable.

- [ ] **3.10.6** (1 pts): Enforce safeguarding measures for CUI at alternate work sites.
  - Assessor looks for: CUI safeguarded at home offices and alternate work sites, not just the main office.

## 3.11 Risk Assessment (3 controls)

- [ ] **3.11.1** (3 pts): Periodically assess the risk to organizational operations (including mission, functions, image, or reputation), organizational assets, and individuals, resulting from the operation of organizational systems and the associated processing, storage, or transmission of CUI.
  - Assessor looks for: Risk assessments performed periodically and when the environment changes.

- [ ] **3.11.2** (5 pts): Scan for vulnerabilities in organizational systems and applications periodically and when new vulnerabilities affecting those systems and applications are identified.
  - Assessor looks for: Vulnerability scans run on systems and applications on a defined schedule.

- [ ] **3.11.3** (1 pts): Remediate vulnerabilities in accordance with risk assessments.
  - Assessor looks for: Found vulnerabilities remediated according to risk, with tracking to closure.

## 3.12 Security Assessment (4 controls)

- [ ] **3.12.1** (5 pts): Periodically assess the security controls in organizational systems to determine if the controls are effective in their application.
  - Assessor looks for: Security controls assessed periodically to confirm they still work as intended.

- [ ] **3.12.2** (3 pts): Develop and implement plans of action designed to correct deficiencies and reduce or eliminate vulnerabilities in organizational systems.
  - Assessor looks for: POA&Ms created for deficiencies found, with real milestones.

- [ ] **3.12.3** (5 pts): Monitor security controls on an ongoing basis to ensure the continued effectiveness of the controls.
  - Assessor looks for: Controls monitored continuously, not just at assessment time.

- [ ] **3.12.4** (1 pts) **NEVER DEFERRABLE**: Develop, document, and periodically update system security plans that describe system boundaries, system environments of operation, how security requirements are met, and the relationships with or connections to other systems.
  - Assessor looks for: A current System Security Plan describing how each control is implemented. Never deferrable. No SSP, no valid score.

## 3.13 System and Communications Protection (16 controls)

- [ ] **3.13.1** (5 pts): Monitor, control, and protect communications (i.e., information transmitted or received by organizational systems) at the external boundaries and key internal boundaries of organizational systems.
  - Assessor looks for: Communications monitored, controlled, and protected at system boundaries.

- [ ] **3.13.2** (5 pts): Employ architectural designs, software development techniques, and systems engineering principles that promote effective information security within organizational systems.
  - Assessor looks for: Secure architecture in use: segmentation, layered defenses, secure design principles.

- [ ] **3.13.3** (1 pts): Separate user functionality from system management functionality.
  - Assessor looks for: User functions separated from management functions. Admin interfaces not reachable from user space.

- [ ] **3.13.4** (1 pts): Prevent unauthorized and unintended information transfer via shared system resources.
  - Assessor looks for: Shared resources designed so data cannot leak between users or processes.

- [ ] **3.13.5** (5 pts): Implement subnetworks for publicly accessible system components that are physically or logically separated from internal networks.
  - Assessor looks for: Public-facing components isolated on their own subnetworks (DMZ).

- [ ] **3.13.6** (5 pts): Deny network communications traffic by default and allow network communications traffic by exception (i.e., deny all, permit by exception).
  - Assessor looks for: Firewalls default-deny, with explicit allow rules documented.

- [ ] **3.13.7** (1 pts): Prevent remote devices from simultaneously establishing non-remote connections with organizational systems and communicating via some other connection to resources in external networks (i.e., split tunneling).
  - Assessor looks for: Remote devices blocked from bridging networks: no simultaneous VPN plus open internet or second connection.

- [ ] **3.13.8** (3 pts): Implement cryptographic mechanisms to prevent unauthorized disclosure of CUI during transmission unless otherwise protected by alternative physical safeguards.
  - Assessor looks for: Cryptography protecting CUI in transit where required.

- [ ] **3.13.9** (1 pts): Terminate network connections associated with communications sessions at the end of the sessions or after a defined period of inactivity.
  - Assessor looks for: Network sessions terminated automatically after defined inactivity or conditions.

- [ ] **3.13.10** (1 pts): Establish and manage cryptographic keys for cryptography employed in organizational systems.
  - Assessor looks for: Cryptographic keys generated, distributed, stored, and destroyed under management.

- [ ] **3.13.11** (5 or 3 pts (see scoring)): Employ FIPS-validated cryptography when used to protect the confidentiality of CUI.
  - Assessor looks for: FIPS-validated encryption protecting CUI confidentiality. Partial credit if encrypted but not FIPS-validated. Special scoring: 5 or 3.

- [ ] **3.13.12** (1 pts): Prohibit remote activation of collaborative computing devices and provide indication of devices in use to users present at the device.
  - Assessor looks for: Cameras and microphones on collaborative devices cannot be activated remotely without an indicator.

- [ ] **3.13.13** (1 pts): Control and monitor the use of mobile code.
  - Assessor looks for: Mobile code (scripts, applets, macros) controlled and monitored.

- [ ] **3.13.14** (1 pts): Control and monitor the use of Voice over Internet Protocol (VoIP) technologies.
  - Assessor looks for: VoIP use controlled and monitored.

- [ ] **3.13.15** (5 pts): Protect the authenticity of communications sessions.
  - Assessor looks for: Communications sessions authenticated, so endpoints are who they claim to be.

- [ ] **3.13.16** (1 pts): Protect the confidentiality of CUI at rest.
  - Assessor looks for: CUI encrypted at rest on systems and devices.

## 3.14 System and Information Integrity (7 controls)

- [ ] **3.14.1** (5 pts): Identify, report, and correct information and information system flaws in a timely manner.
  - Assessor looks for: Flaws identified, reported, and corrected within defined timeframes.

- [ ] **3.14.2** (5 pts): Provide protection from malicious code at appropriate locations within organizational information systems.
  - Assessor looks for: Malware protection deployed at endpoints, email, and other appropriate points.

- [ ] **3.14.3** (5 pts): Monitor system security alerts and advisories and take action in response.
  - Assessor looks for: Security alerts and advisories monitored, with action taken and recorded.

- [ ] **3.14.4** (5 pts): Update malicious code protection mechanisms when new releases are available.
  - Assessor looks for: Malware signatures and engines updated when new releases are available.

- [ ] **3.14.5** (3 pts): Perform periodic scans of the information system and real-time scans of files from external sources as files are downloaded, opened, or executed.
  - Assessor looks for: Systems scanned periodically, and files scanned in real time on access or download.

- [ ] **3.14.6** (5 pts): Monitor organizational systems, including inbound and outbound communications traffic, to detect attacks and indicators of potential attacks.
  - Assessor looks for: Inbound and outbound traffic monitored for anomalies and attacks.

- [ ] **3.14.7** (3 pts): Identify unauthorized use of organizational systems.
  - Assessor looks for: Unauthorized use of systems identified: rogue devices, unknown software, unusual accounts.
