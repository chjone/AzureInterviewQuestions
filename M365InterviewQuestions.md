What is the update freuqency of Windows 10 updates
--
- quality updates are cumulative and delivered monthly
- feature updates are delievered every 6-months

How long are Windows 10 builds support?
--
- Pro = 18 months
- Enterprise - Spring builds = 18-months, Fall builds 30-months

List the core security features of Windows 10
--
- Application Control
- Windows Defender
- Microsoft Defender for Endpoint
- Application Guard*
- Credential Guard*
- Windows Hello
- Attack Surface Reduction Rules (ASR's)*
- Secure Boot
- Measure Boot
- Bitlocker
- Applocker
- Device Guard
- GPO
- Baselines

Describe the process for provisioning a Windows OS for broad deployment.
--
- Answers will vary greatly.
- Looking for key points on OS configs, lockdown policies, app installs, app removals, domian/OU join, patching, etc.
- Provision with SCCM, Intune, 3rd party, etc.

What solutions are available to monitor and report on OS deployment and readiness.
--
- Desktop Analytics
- SETUP.EXE /Auto Upgrade /Quiet /NoReboot /DynamicUpdate Disable /Compat ScanOnly

What are key differences in Pro vs. Enterprise?
Security features (starred in 2nd question of this doc), update cycles, MDOP, LTSC, Resilient File System (ReFS), Unified Write Filter, Desktop Analytics, Persistent Memory, SMB Direct...

What is co-management?
--
Co-management enables you to concurrently manage Windows 10 devices by using both Configuration Manager and Microsoft Intune. It lets you cloud-attach your existing investment in Configuration Manager by adding new functionality. By using co-management, you have the flexibility to use the technology solution that works best for your organization.

What is AutoPilot?
--
Windows Autopilot is a collection of technologies used to set up and pre-configure new devices, getting them ready for productive use. You can also use Windows Autopilot to reset, repurpose, and recover devices

How do you enable Azure Hybrid-Join?
--
- Azure AD Connect - configure device options, and OS type support
- Configure service connection point (SCP)
- Configure the local intranet settings for device registration
- Configure SSO

What is Enterprise State Roaming?
--
When you enable Enterprise State Roaming, your organization is automatically granted a free, limited-use license for Azure Rights Management protection from Azure Information Protection. This free subscription is limited to encrypting and decrypting enterprise settings and application data synced by Enterprise State Roaming.

What are key differences between Intune and SCCM?
--
- Intune: cloud based, only supports Windows clients and mobile OS's. Does not support bare-metal imaging, limited patching capabilities
- SCCM: on-prem with some cloud capabilities (CMG), supports servers, granular patching capabilities

What are the core Microsoft Defender solutions and what are they used for?
--
- Defender for Endpoint - Endpoint Detection and Response - use to provide post-breach protection to endpoints, servers and mobile devices
- Defender for Identity - (formerly Azure Advanced Threat Protection, also known as Azure ATP) is a cloud-based security solution that leverages your on-premises Active Directory signals to identify, detect, and investigate advanced threats, compromised identities, and malicious insider actions directed at your organization.
- Defender for Office 365 - safeguards your organization against malicious threats posed by email messages, links (URLs), and collaboration tools.

What is Conditional Access?
--
At their simplest are if-then statements, if a user wants to access a resource, then they must complete an action. Example: A payroll manager wants to access the payroll application and is required to perform multi-factor authentication to access it. By using Conditional Access policies, you can apply the right access controls when needed to keep your organization secure and stay out of your user's way when not needed.

Administrators are faced with two primary goals:

- Empower users to be productive wherever and whenever
- Protect the organization's assets

When are Conditinoal Access policies applied?
--
Conditional Access policies are enforced after first-factor authentication is completed. Conditional Access isn't intended to be an organization's first line of defense for scenarios like denial-of-service (DoS) attacks, but it can use signals from these events to determine access.


What is the difference between Azure AD and Active Directory?
--
Microsoft's cloud-based identity solution that allows you to leverage users, groups, applications and security principal concepts. It supports web-based OAuth 2.0, SAML 2.0 and Open ID authentication frameworks. AAD does not have capabilities like Group Policies or Application Containers or extensible schema, which is sometimes required by some workloads, among other capabilities.

What are the identity models available in Microsoft Office 365?
--
Cloud identity, federated identity, and synchronized identity

How can Cloud App Security Brokers prevent shadow IT?
--
It allows you to monitor and or block access to apps and resouces on managed devices. Evaluate against compliance standards, prevent leaks, and limit access to regulated data.

What are billing administrators?
--
- makes purchases, manages subscriptions, manages support tickets, monitors service health

What is used to configure the O365 installation?
--
- Office Customization Tool

What type of DNS record helps protect messages from being flagged as spam?
--
TXT record

What is DMARC, DKIM, and SPF?
--
- DMARC: Domain-Based Message Authentication Reporting and Conformance, is an added authentication method that uses both SPF and DKIM to verify whether or not an email was actually sent by the owner of the “Friendly-From” domain that the user sees.
- DKIM: DomainKeys Identified Mail, lets an organization (or handler of the message) take responsibility for a message that is in transit.
- SPF: Sender Policy Framework, is an email validation protocol designed to detect and block email spoofing. It allows mail exchangers to verify that incoming mail from a specific domain comes from an IP Address authorized by that domain’s administrators
