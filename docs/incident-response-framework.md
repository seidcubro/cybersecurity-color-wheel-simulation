# Incident Response Framework

## Overview

The Cybersecurity Color Wheel Simulation follows an incident response framework similar to those used in enterprise security operations.

The framework focuses on evidence-driven investigation and coordinated response.

---

## Incident Response Lifecycle

### Detection

Detection begins when suspicious activity is identified.

Examples include:

- risky authentication attempts
- MFA fatigue attacks
- unusual VPN logins
- abnormal file access

---

### Triage

Triage determines:

- which systems are involved
- which identities may be compromised
- whether crown-jewel systems may be at risk

This phase focuses on quickly determining the scope of the incident.

---

### Investigation

Investigators collect and correlate evidence across multiple telemetry sources.

These sources include:

- identity authentication logs
- MFA challenge logs
- VPN logs
- DNS queries
- proxy traffic
- file share audit logs

The goal is to reconstruct attacker behavior and timeline.

---

### Containment

Once attacker activity is confirmed, containment actions may include:

- disabling compromised accounts
- revoking active authentication sessions
- blocking malicious domains
- restricting access to sensitive systems

Containment must balance security risk with business continuity.

---

### Impact Assessment

Investigators determine whether sensitive data was accessed or exfiltrated.

Indicators include:

- access to crown-jewel data
- archive creation
- large outbound transfers
- suspicious external destinations

---

### Recovery

Recovery actions may include:

- credential resets
- enhanced monitoring
- configuration updates
- improved security controls

---

### Lessons Learned

After the incident, teams evaluate:

- detection gaps
- architectural weaknesses
- monitoring limitations
- response improvements

These lessons strengthen future defenses.

