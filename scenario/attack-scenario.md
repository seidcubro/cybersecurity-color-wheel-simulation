# Attack Scenario

## High-level narrative

A finance user receives repeated MFA push notifications after a suspicious sign-in attempt from an unfamiliar location and device. One prompt is approved, allowing VPN access. The attacker gains an internal foothold, pivots using a service account, accesses the Research_Contracts share, stages data into a ZIP archive, and initiates likely outbound transfer activity to a suspicious cloud destination.

## Themes

- phishing
- MFA fatigue
- risky VPN login
- service account abuse
- lateral movement
- exfiltration staging
- incomplete visibility

## Crown jewels

- \\FS-RES-02\Research_Contracts
- Student_Records
