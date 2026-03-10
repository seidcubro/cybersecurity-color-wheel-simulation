# Cybersecurity Color Wheel Simulation

A structured incident response case study based on a cybersecurity color wheel practical focused on identity compromise, MFA fatigue, VPN abuse, lateral movement, and probable exfiltration.

## Overview

This repository documents a Blue Team investigation for a simulated enterprise security incident. The scenario centers on a suspicious 2:13 AM VPN login tied to a compromised finance user account. After repeated MFA pushes, the attacker gained access, pivoted through a service account, reached a crown-jewel file share, staged an archive, and initiated likely data exfiltration.

The project is organized as both a portfolio artifact and a foundation for future cybersecurity training use.

## Scenario Summary

The simulated organization, WV RUS, faced an identity-driven attack that unfolded in several stages:

1. A high-risk sign-in attempt originated from an unfamiliar geographic region and a new device.
2. Multiple MFA push notifications were sent to the victim.
3. One MFA request was approved, allowing VPN access.
4. Internal access was established and correlated to a new VPN session.
5. A service account was then used across multiple hosts, indicating lateral movement.
6. Sensitive data on the `\\FS-RES-02\Research_Contracts` share was accessed and staged into an archive.
7. DNS, proxy, and VPN byte-count evidence suggested probable exfiltration to a suspicious cloud storage destination.

## Repository Structure

```text
cybersecurity-color-wheel-simulation/
├── README.md
├── LICENSE
├── .gitignore
├── docs/
│   ├── simulation-overview.md
│   └── training-program-notes.md
├── blue-team/
│   ├── README.md
│   └── blue-team-running-log.pdf
├── white-team/
│   └── evidence-catalog-summary.md
├── scenario/
│   └── attack-scenario.md
└── assets/
Blue Team Deliverable

The main artifact in this repository is the completed Blue Team running log:

blue-team/blue-team-running-log.pdf

The running log includes:

success criteria

incident summary

known facts

hypotheses

evidence requests by phase

visibility and coverage analysis

default containment package

decision log

timeline

collaboration notes

end-of-phase outcomes

Skills Demonstrated

This project demonstrates practical skills in:

incident response

identity and access security analysis

MFA fatigue detection

VPN abuse investigation

lateral movement analysis

service account risk analysis

exfiltration detection

security documentation

cross-functional collaboration

Why This Matters

This practical is useful as both:

a cybersecurity portfolio project

a reusable tabletop-style training exercise

a foundation for security awareness and response training in organizations

It reflects real-world security operations themes, especially around identity compromise, incomplete telemetry, business tradeoffs, and evidence-driven containment.

Training Program Potential

This simulation can be adapted into a repeatable training program for teams inside companies.

Possible audience

SOC analysts

help desk and IAM teams

incident commanders

security engineers

IT managers

cross-functional technical staff

Possible learning outcomes

identifying identity-based attack signals

responding to MFA abuse

correlating logs across multiple systems

making containment decisions under uncertainty

balancing security response against business continuity

documenting incidents clearly and professionally

Possible progression model

Level 1: identity compromise and MFA fatigue

Level 2: VPN access and lateral movement

Level 3: data staging, exfiltration indicators, and breach determination

Notes

This repository is intended for educational, portfolio, and training design purposes. It does not include exploit code or offensive tooling. The focus is on defense, evidence handling, response workflow, and security training design.

Author

Seid Cubro

Cloud Computing student with interests in cybersecurity, incident response, infrastructure, and practical security operations.
