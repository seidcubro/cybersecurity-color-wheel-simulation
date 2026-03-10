# Simulation Overview

This repository contains a structured incident response case study based on a cybersecurity color wheel simulation centered on a suspicious 2:13 AM VPN login, MFA fatigue, service-account abuse, lateral movement, and probable exfiltration.

## Core scenario

An attacker successfully gained access to the identity account of a finance user after repeated MFA push prompts were approved. After VPN access was established, the attacker pivoted internally, abused a service account, accessed a crown-jewel file share, staged sensitive files into an archive, and initiated outbound transfer activity to a suspicious cloud destination.

## Learning objectives

- Practice evidence-driven incident response
- Distinguish facts from hypotheses
- Build a defensible incident timeline
- Prioritize containment during identity-driven attacks
- Identify detection and visibility gaps
- Understand how business constraints affect security decisions

## Teams in the color wheel model

- Blue Team: detection, triage, containment, and incident documentation
- White Team: facilitation and evidence release
- Red Team: attacker perspective and likely next steps
- Purple Team: detection engineering and control improvement
- Green Team: architecture and segmentation improvement
- Orange Team: business risk, approvals, and communication tradeoffs
