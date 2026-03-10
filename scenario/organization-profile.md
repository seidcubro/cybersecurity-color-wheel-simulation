\# Organization Profile – WV RUS



\## Overview



WVRUS (Wyoming Valley Research and University Services) is a simulated organization used in the Cybersecurity Color Wheel Simulation.



The organization supports academic research, student services, and internal administrative operations.



The environment contains sensitive data including research contracts and student records.



---



\# Organizational Structure



The organization consists of several departments:



\- Finance

\- Research Administration

\- IT Operations

\- Student Services

\- Academic Departments



Each department uses centralized authentication and network infrastructure.



---



\# Core Systems



The simulation environment includes the following key systems.



\## Identity Provider (IdP)



The identity provider manages authentication and multi-factor authentication.



Responsibilities include:



\- user authentication

\- MFA enforcement

\- single sign-on

\- conditional access policies



---



\## VPN Gateway



The VPN gateway allows employees to access internal systems remotely.



VPN connections provide internal network access and may expose internal resources if compromised.



---



\## File Servers



The organization maintains several internal file servers.



The most critical is:



```

FS-RES-02

```



This server hosts sensitive research data.



---



\## Crown Jewel Systems



Crown jewels are the most sensitive assets in the organization.



\### Primary Crown Jewel



```

\\\\FS-RES-02\\Research\_Contracts

```



This share contains:



\- research contracts

\- deliverables

\- partner agreements

\- potentially sensitive information



\### Secondary Crown Jewel



```

Student\_Records

```



This system contains sensitive student data and academic records.



---



\# Key Accounts



Important identities referenced in the scenario include:



\*\*jordan.rivera@wvrus.org\*\*



Finance employee whose credentials were compromised.



\*\*svc-backup-reports\*\*



Service account used for automated reporting and backup processes.



Service accounts often have elevated permissions and may be targeted during lateral movement.



---



\# Security Controls



The organization uses several security controls.



\## Identity Security



\- multi-factor authentication enabled

\- conditional access rules

\- risk-based login alerts



However, MFA uses push notifications without number matching.



---



\## Network Monitoring



Available telemetry includes:



\- VPN authentication logs

\- DNS resolver logs

\- partial proxy logs

\- file share audit logs



---



\## Endpoint Visibility



Endpoint detection and response (EDR) coverage is incomplete.



Some systems are not enrolled in EDR, creating investigation blind spots.



---



\# Business Constraints



The organization has limited tolerance for system downtime.



Critical operations include:



\- payroll processing

\- research administration

\- student services



Security responses must balance containment with operational continuity.

