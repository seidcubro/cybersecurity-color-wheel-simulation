\# Network Architecture



\## Overview



The WVRUS network environment includes internal servers, user workstations, identity infrastructure, and remote access systems.



Users authenticate through the identity provider and may access internal systems through VPN connections.



---



\# Core Components



\## Identity Provider



The identity provider handles authentication and multi-factor authentication.



It records:



\- login attempts

\- risk flags

\- MFA challenges

\- device fingerprints



---



\## VPN Gateway



The VPN gateway allows remote users to access internal systems.



When users authenticate successfully, they receive an internal IP address.



Example:



```

VPN IP: 10.44.18.23

```



---



\## Internal Workstations



Employees use internal workstations or laptops.



Example endpoint in the scenario:



```

FIN-LT-033

```



This workstation belongs to the compromised finance user.



---



\## File Server



Sensitive research files are stored on:



```

FS-RES-02

```



This server hosts the crown-jewel share:



```

\\\\FS-RES-02\\Research\_Contracts

```



---



\# Network Segmentation



Network segmentation in the scenario is minimal.



VPN users land on an internal subnet with access to several internal resources.



This allows compromised accounts to potentially reach sensitive servers.



---



\# Monitoring Points



Security telemetry exists at several points in the architecture.



Monitoring includes:



\- identity authentication logs

\- MFA challenge logs

\- VPN authentication logs

\- DNS queries

\- proxy traffic

\- file share access logs



These logs allow investigators to reconstruct attacker behavior.



---



\# Investigation Strategy



Blue Team investigators correlate activity across:



\- identity logs

\- VPN logs

\- DNS queries

\- proxy traffic

\- file server access



This multi-source correlation helps identify:



\- compromised identities

\- lateral movement

\- data staging

\- potential exfiltration.

