# awesome_okapi
Awesome Okapi_v1 is a cybersecurity penetration-testing and security-assessment platform designed for authorized security professionals, penetration testers, cybersecurity students, red teams, blue teams, security researchers, and organizations conducting controlled security assessments.

The platform provides a centralized interface for managing authorized cybersecurity testing activities. Its architecture is designed to connect approved communication channels with controlled security-testing environments, allowing operators to submit predefined testing tasks and receive structured results without giving messaging accounts unrestricted access to operating-system shells.

Awesome Okapi_v1 is designed around a fundamental principle: every security operation must be authorized, scoped, logged, and controlled.

The platform can provide integrations for Discord, Telegram, Slack, Google Chat, WhatsApp, Signal, and a web application. These interfaces act as communication and management clients for the central Awesome Okapi_v1 platform.

The system can be deployed in a cybersecurity laboratory, internal enterprise environment, penetration-testing infrastructure, or other environment where the operator has explicit authorization.

# 2. Core Purpose

The primary purpose of Awesome Okapi_v1 is to simplify authorized penetration testing.

Traditional security assessments often require testers to work across multiple terminals, dashboards, communication platforms, scanners, reporting systems, and documentation tools.

Awesome Okapi_v1 attempts to bring these workflows together.

A tester can authenticate with the platform, select an authorized project, select an approved target, request a supported security-testing operation, monitor the task, and review the resulting information.

The platform is not intended to provide unrestricted access to arbitrary third-party systems.

Instead, Awesome Okapi_v1 should enforce:

Authentication.
Authorization.
Target validation.
Project boundaries.
Command allowlists.
Role-based permissions.
Approval requirements.
Execution limits.
Audit logging.
Secure result handling.
3. Supported Interfaces

# Version 1 can support the following interfaces:

* Discord.
* Telegram.
* Slack.
* Google Chat.
* WhatsApp.
* Signal.
* Web Application.

Each interface communicates with the central Awesome Okapi_v1 backend.

The interfaces should not independently execute commands.

Instead, the architecture can follow this model:

User → Communication Platform → Authentication → Authorization → Policy Engine → Approved Task → Isolated Worker → Results → Audit Log → User

This design allows security policies to remain centralized.

4. Discord Interface

The Discord component can provide a controlled security-testing bot.

An authorized penetration tester can interact with the bot inside an approved Discord server.

Possible functions include:

Display project information.
Display authorized targets.
Start approved assessments.
Check task status.
Retrieve vulnerability summaries.
View training exercises.
View phishing-simulation campaign status.
Generate assessment reports.
Cancel permitted tasks.

Discord roles can be mapped to Awesome Okapi_v1 roles.

For example:

Administrator

Can configure integrations and security policies.

Security Manager

Can create projects and approve selected activities.

Penetration Tester

Can execute authorized testing workflows.

Trainee

Can access restricted laboratory exercises.

Auditor

Can review logs and reports.

5. Telegram Interface

The Telegram integration provides a bot-based interface for authorized users.

A tester can interact with the bot using structured commands.

Instead of accepting arbitrary shell commands, Awesome Okapi_v1 can expose predefined security-testing operations.

For example, conceptual commands could include:

/projects

/targets

/assessment

/status

/findings

/report

/training

The actual operations available to each user depend on their permissions.

Every request should be authenticated and associated with the user's account.

6. Slack Interface

Slack integration allows security teams to coordinate testing activities inside organizational workspaces.

A dedicated security channel can receive assessment notifications.

For example:

Assessment Started

Project: Internal Security Lab

Status: Running

Authorized Target: LAB-NETWORK-01

Operator: Authorized Tester

The system can later provide:

Assessment Completed

Findings: 7

High Severity: 1

Medium Severity: 3

Low Severity: 3

Report: Available in dashboard

This approach keeps communication organized while preventing sensitive technical information from unnecessarily appearing in general channels.

7. Google Chat Interface

Google Chat can provide similar functionality for organizations using Google Workspace.

Authorized users can interact with the Awesome Okapi_v1 service through approved Chat spaces.

The integration can provide:

Assessment notifications.
Security alerts.
Task status.
Finding summaries.
Training notifications.
Report availability.

Administrators can restrict the integration to approved spaces and authorized users.

8. WhatsApp Interface

WhatsApp integration can provide controlled notifications and security-assessment interaction where an approved business integration is available.

The platform should not treat a phone number alone as sufficient authorization.

Requests should be associated with an Awesome Okapi_v1 account and verified through the platform's authentication system.

The WhatsApp interface can be restricted to lower-risk functions such as:

Assessment status.
Alerts.
Report notifications.
Security-training exercises.
Approval notifications.
9. Signal Interface

Signal can provide another communication channel for authorized security teams.

The Signal interface can be used for:

Security notifications.
Assessment status.
Approved commands.
Training exercises.
Approval requests.

The same central policy engine should govern Signal requests as all other integrations.

Encryption of a messaging platform does not replace authorization.

10. Web Application

The Awesome Okapi_v1 web application acts as the primary administration and management interface.

The dashboard can contain several sections.

Dashboard

The dashboard can display:

Active assessments.
Completed assessments.
Vulnerability counts.
Security alerts.
Training campaigns.
Connected integrations.
Recent activity.
System health.
Projects

Administrators can create security-testing projects.

A project can contain:

Project name.
Description.
Authorized users.
Authorized targets.
Testing dates.
Security policies.
Reporting settings.
Targets

Targets should be explicitly registered.

Examples include:

Laboratory machines.
Development applications.
Internal test networks.
Authorized domains.
Cloud test environments.
Containers.

Targets outside the project scope should be automatically rejected.

11. Command System

The command system is a central component of Awesome Okapi_v1.

Version 1 should use a controlled command registry.

Each command can contain:

Command identifier.
Description.
Required permission.
Allowed target type.
Risk classification.
Timeout.
Logging requirement.
Approval requirement.

For example:

LOW RISK

Information retrieval.

MEDIUM RISK

Authorized vulnerability assessment.

HIGH RISK

Sensitive validation requiring explicit approval.

Unsupported commands should be rejected.

12. Scope Validation

Scope validation is mandatory.

Before an assessment starts, Awesome Okapi_v1 should determine:

Who requested the operation.
Which project they belong to.
Which target they selected.
Whether the target is authorized.
Whether the requested operation is permitted.
Whether additional approval is necessary.

If any requirement fails, the task should not execute.

This creates an important security barrier against accidental or unauthorized testing.

13. Laboratory Mode

Version 1 can include a dedicated laboratory mode.

Laboratory mode allows students and security professionals to conduct experiments against deliberately vulnerable systems.

A laboratory can contain:

Vulnerable web applications.
Virtual machines.
Containers.
Simulated networks.
Training servers.
Security challenges.

All laboratory assets can be registered within an Awesome Okapi_v1 project.

This allows students to learn penetration-testing techniques without targeting real-world infrastructure.

14. Vulnerability Assessment

Awesome Okapi_v1 can coordinate approved vulnerability-assessment tools.

The platform can collect results and normalize them.

Each vulnerability finding can include:

Finding ID.
Vulnerability name.
Severity.
Affected asset.
Description.
Evidence reference.
Recommended remediation.
Current status.
Assigned analyst.

Findings can be marked:

Open.
Investigating.
Remediated.
Verified.
Accepted Risk.
False Positive.
15. Penetration-Testing Workflow

Version 1 can organize testing into several phases.

Phase 1 — Planning

Define the assessment and authorized scope.

Phase 2 — Reconnaissance

Collect information about approved assets.

Phase 3 — Enumeration

Identify services and application components within scope.

Phase 4 — Vulnerability Assessment

Identify potential security weaknesses.

Phase 5 — Controlled Validation

Validate selected findings using approved non-destructive techniques.

Phase 6 — Documentation

Record evidence and observations.

Phase 7 — Remediation

Provide recommendations.

Phase 8 — Retesting

Verify that identified weaknesses have been addressed.

16. Phishing Simulation

Awesome Okapi_v1 can include a security-awareness simulation module.

The purpose is to train employees to recognize phishing.

Administrators can create controlled campaigns containing:

Campaign name.
Training objective.
Authorized participants.
Simulation template.
Start date.
End date.
Training page.

The simulation should never be used to collect real passwords.

Instead, participants can be directed to an organization-controlled educational page explaining why the message was suspicious.

17. Phishing Training

The educational page can teach users to recognize:

Suspicious domains.
Fake login requests.
Urgent language.
Unexpected attachments.
Impersonation.
Suspicious links.
Requests for sensitive information.
Social-engineering techniques.

The purpose is education rather than credential collection.

The platform can measure safe training metrics such as whether a participant visited the training page or reported the simulated message.

18. Security Reports

Awesome Okapi_v1 can generate penetration-testing reports.

Reports can include:

Executive Summary

A management-friendly overview.

Scope

The assets that were authorized for assessment.

Methodology

The general testing approach.

Findings

Security weaknesses discovered during the assessment.

Severity

Risk classification for each finding.

Evidence

References to approved assessment evidence.

Recommendations

Suggested remediation.

Retesting

Results after remediation.

19. Audit Logging

Every important action should generate an audit event.

Examples include:

Login.
Logout.
Failed login.
Command request.
Blocked command.
Approved task.
Rejected task.
Assessment started.
Assessment completed.
Finding created.
Finding modified.
Report generated.
Integration configured.
User permissions changed.

Audit records should be protected against unauthorized modification.

20. Role-Based Access Control

Awesome Okapi_v1 should implement role-based access control.

Administrator

Full platform administration.

Security Manager

Assessment management and approval.

Penetration Tester

Authorized testing.

Analyst

Finding and report management.

Trainee

Laboratory-only access.

Auditor

Read-only audit access.

Permissions should be assigned according to the principle of least privilege.

21. Authentication

The platform should support strong authentication.

Potential mechanisms include:

Password authentication.
Multi-factor authentication.
Secure sessions.
API tokens.
Integration credentials.
Token expiration.
Credential rotation.

Secrets should never be embedded directly inside source code.

Credentials should be stored using secure secret-management mechanisms.

22. API

Awesome Okapi_v1 can expose a secure API.

Potential resources include:

/users

/projects

/targets

/assessments

/tasks

/findings

/campaigns

/reports

/audit

Every API endpoint should enforce authentication and authorization.

API requests should also be validated and rate limited.

23. Job Queue

Security-testing operations can be placed into a job queue.

A task can have states such as:

Queued

Waiting for execution.

Running

Currently being processed.

Completed

Successfully finished.

Failed

Execution encountered an error.

Rejected

Policy prevented execution.

Cancelled

Authorized operator cancelled the task.

This architecture prevents communication integrations from directly controlling execution infrastructure.

24. Isolated Workers

Testing operations should execute in isolated environments where possible.

Workers can be implemented using containers or dedicated virtual machines.

Isolation can provide:

Restricted filesystem access.
Restricted networking.
CPU limits.
Memory limits.
Execution timeouts.
Temporary environments.
Limited privileges.

Higher-risk testing should use dedicated laboratory environments.

25. Monitoring

Awesome Okapi_v1 can monitor system activity.

The monitoring dashboard can show:

Active jobs.
Worker health.
Integration health.
Authentication activity.
Failed authorization attempts.
Assessment progress.
Security findings.
System errors.

Suspicious administrative activity can generate alerts.

26. Rate Limiting

Rate limiting protects the platform from excessive requests.

Limits can be applied to:

Users.
Bots.
API tokens.
IP addresses.
Projects.
Communication channels.

Repeated unauthorized requests can trigger security alerts.

27. Error Handling

The platform should provide safe error messages.

Users should not receive internal stack traces, secret values, database credentials, filesystem paths, or other sensitive implementation details.

Errors can instead provide a simple identifier such as:

Operation failed. Reference: OKAPI-1027.

Administrators can use the reference identifier to investigate the detailed event in the secure logs.

28. Data Protection

Security assessment information can be highly sensitive.

Awesome Okapi_v1 should therefore protect:

Credentials.
API tokens.
Assessment results.
Vulnerability information.
Internal network information.
Audit records.
Security reports.

Data should be encrypted during transmission and appropriately protected at rest.

Only authorized project members should be able to access project information.

29. Notification System

The platform can send notifications through supported communication channels.

Examples include:

Assessment Started

Assessment Completed

Critical Finding Identified

Approval Required

Task Rejected

Report Available

Notifications should contain only the information necessary for the destination channel.

Sensitive evidence can remain accessible through the authenticated web dashboard.

30. Security Awareness Dashboard

The phishing-simulation module can provide campaign-level statistics.

Metrics can include:

Messages sent.
Messages delivered.
Training pages visited.
Simulations reported.
Training completed.

The dashboard can help organizations identify areas where additional security awareness may be useful.

31. Configuration

Administrators can configure:

Users.
Roles.
Projects.
Targets.
Integrations.
Security policies.
Command permissions.
Audit settings.
Notification settings.
Training campaigns.

Configuration changes should be logged.

32. Version 1 Security Principles

Awesome Okapi_v1 should follow these principles:

Default Deny

Unknown operations are rejected.

Least Privilege

Users receive only the permissions required for their role.

Explicit Scope

Testing targets must be registered.

Centralized Authorization

All interfaces use the same authorization engine.

Isolation

Testing operations run in controlled environments.

Auditability

Security-relevant activity is recorded.

Approval

Sensitive activities can require additional authorization.

Safe Simulation

Phishing exercises are designed for training rather than credential theft.

33. Example Operational Flow

An authorized penetration tester opens the Awesome Okapi_v1 interface.

The tester authenticates.

The system identifies the user's role.

The tester selects a project.

The platform displays authorized targets.

The tester selects an approved laboratory target.

The tester requests a predefined assessment operation.

The policy engine validates the request.

If permitted, the task enters the job queue.

An isolated worker performs the approved operation.

The worker returns structured results.

The results are processed by the backend.

The event is recorded in the audit log.

The tester receives a summary through the selected interface.

Detailed evidence remains available through the secure dashboard.

34. Administration

Administrators can manage the entire platform through the web interface.

Administrative capabilities can include:

User management.
Role management.
Project management.
Integration management.
Policy management.
Audit-log review.
Worker management.
System-health monitoring.
Report configuration.

Administrative functions should require elevated authentication.

35. Extensibility

Although Awesome Okapi_v1 focuses on the initial platform architecture, its design can support future integrations.

Potential future additions include:

SIEM platforms.
Ticketing systems.
Cloud-security platforms.
Vulnerability-management platforms.
Additional messaging platforms.
Security scanners.
Threat-intelligence services.
Training platforms.

Each integration should inherit the central authentication, authorization, and logging model.

36. Educational Mission

Awesome Okapi_v1 can be particularly valuable for cybersecurity education.

Students can use the platform to practice:

Security assessment.
Vulnerability analysis.
Security awareness.
Incident-response exercises.
Security reporting.
Defensive analysis.

Instructors can create projects and assign laboratory tasks.

The platform can then provide measurable progress information.

37. Production Deployment

For production environments, Awesome Okapi_v1 should be deployed using appropriate security controls.

Recommended controls include:

HTTPS.
Network segmentation.
Strong administrator authentication.
Multi-factor authentication.
Secure secret management.
Regular backups.
Centralized monitoring.
Vulnerability management.
Access reviews.
Log protection.
Software updates.

The execution environment should be separated from the web and messaging layers whenever possible.

38. Future Evolution

Awesome Okapi_v1 establishes the foundation for future versions of the Awesome Okapi platform.

Future versions could introduce more advanced:

Policy engines.
Automated reporting.
Security analytics.
Laboratory orchestration.
Threat detection.
Workflow automation.
Integration management.
Compliance reporting.
Security-awareness analytics.

However, the foundational security principles of authorization, scope enforcement, isolation, and auditing should remain central.


Awesome Okapi_v1 is a controlled cybersecurity penetration-testing and security-assessment platform that brings authorized security operations into a centralized environment.

Through integrations with Discord, Telegram, Slack, Google Chat, WhatsApp, Signal, and a web application, security professionals can manage approved testing workflows, monitor assessments, review vulnerabilities, coordinate security-awareness exercises, and generate professional reports.

The platform is designed to prevent communication integrations from becoming unrestricted remote shells. Commands are processed through authentication, authorization, scope validation, policy enforcement, controlled execution, and audit logging.

Its phishing functionality is intended for authorized security-awareness simulations and educational campaigns. Simulated phishing pages should be controlled by the organization conducting the exercise and should not collect real passwords or authentication#  tokens.

The result is a foundation for a professional cybersecurity platform that combines penetration testing, security assessment, security-awareness training, laboratory exercises, workflow management, reporting, and centralized security controls.

Awesome Okapi_v1

Authorized Testing • Controlled Execution • Secure Operations • Comprehensive Auditing

# How to clone the repo
```bash
git clone https://github.com/Iankulani/awesome_okapi.git
cd awesome_okapi
```

# How to run
```bash
python awesome_okapi.py
```

# Star History
```bash

