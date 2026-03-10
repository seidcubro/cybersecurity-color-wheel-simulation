# Cybersecurity Color Wheel Simulation

A structured **incident response case study** investigating an identity compromise involving MFA fatigue, VPN access abuse, lateral movement, and probable data exfiltration.

This project documents a simulated enterprise security incident and demonstrates how a Blue Team investigation can reconstruct attacker activity using identity, network, and file-access telemetry.

---

## Overview

The scenario centers on a suspicious **2:13 AM VPN login** tied to a compromised finance employee account.

After repeated MFA push prompts, the attacker gained remote access through the organization’s VPN gateway and began interacting with internal systems.

Evidence indicates the attacker then:

- abused a service account  
- accessed a crown-jewel research file share  
- created a compressed archive of sensitive files  
- transferred data to a suspicious external cloud domain  

The project demonstrates how defenders correlate evidence across multiple systems to determine whether a **data breach occurred**.

---

## Key Investigation Themes

This simulation focuses on several real-world attack techniques:

- phishing and credential compromise  
- MFA fatigue attacks  
- suspicious VPN logins  
- service account abuse  
- lateral movement within the network  
- data staging and exfiltration indicators  

---

## Repository Structure

cybersecurity-color-wheel-simulation/

README.md  
LICENSE  
.gitignore  

blue-team/  
- CS 355 Practical Blue Team Running Log.pdf  
- Blue Team.pdf  
- playbook.md  

white-team/  
- White Team Evidence Catalog.pdf  

scenario/  
- attack-scenario.md  
- organization-profile.md  
- network-architecture.md  

docs/  
- incident-response-framework.md  
- simulation-overview.md  
- training-program-notes.md  

assets/  
- attack-chain-diagram.md  
- network-architecture-diagram.md  
- incident-timeline-diagram.md  
- README.md  

---

## Blue Team Investigation

The Blue Team conducted the investigation using a structured incident response process.

Primary responsibilities included:

- detecting suspicious authentication activity  
- requesting evidence from available telemetry sources  
- correlating identity and network events  
- identifying attacker movement within the environment  
- determining whether sensitive data was accessed or exfiltrated  

The full investigation log is documented in:

blue-team/CS 355 Practical Blue Team Running Log.pdf

---

## Evidence Sources

The investigation relied on multiple telemetry sources.

### Identity Logs

- IdP authentication logs  
- MFA challenge records  
- risk-based login alerts  

These logs revealed the initial suspicious login attempt and MFA fatigue attack.

### VPN Logs

- authentication records  
- assigned internal IP address  
- session duration and data transfer statistics  

These logs confirmed remote access to the internal network.

### DNS and Proxy Logs

DNS and proxy telemetry revealed connections to a suspicious external cloud storage domain.

These connections coincided with large outbound network transfers.

### File Share Audit Logs

File access logs revealed activity on the organization’s crown-jewel file server.

Evidence included:

- bulk reads from the research contracts directory  
- archive creation  
- file staging in temporary directories  

---

## Crown Jewel Systems

The most sensitive assets in the environment include:

\\FS-RES-02\Research_Contracts  
Sensitive research contracts and deliverables.

Student_Records  
Academic and personal student information.

Access to these systems is treated as a potential breach event.

---

## Visual Diagrams

The repository includes diagrams explaining the attack and investigation.

Attack Chain  
assets/attack-chain-diagram.md

Network Architecture  
assets/network-architecture-diagram.md

Incident Timeline  
assets/incident-timeline-diagram.md

---

## Training Program Potential

This simulation can be adapted into a cybersecurity training exercise for organizations.

Possible training audiences include:

- SOC analysts  
- security engineers  
- IT administrators  
- incident response teams  

Learning objectives may include:

- identifying identity-based attacks  
- investigating MFA abuse  
- correlating security telemetry  
- balancing containment actions with business risk  
- documenting incidents clearly and professionally  

---

## Skills Demonstrated

This project demonstrates practical cybersecurity skills including:

- incident response investigation  
- identity compromise detection  
- MFA fatigue attack analysis  
- VPN telemetry analysis  
- lateral movement detection  
- data exfiltration indicators  
- security documentation and reporting  

---

## Author

Seid Cubro

Cloud Computing student with interests in:

- cybersecurity  
- security operations  
- cloud infrastructure  
- incident response
