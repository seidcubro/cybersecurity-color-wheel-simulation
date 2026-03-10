# Network Architecture

## Overview

The WVRUS environment includes internal servers, employee workstations, identity infrastructure, and remote access systems.

Users authenticate through the identity provider and may access internal systems through the VPN gateway.

---

## Core Components

### Identity Provider

The identity provider handles authentication and MFA.

It records:

- login attempts
- geographic risk indicators
- device fingerprints
- MFA challenge events

---

### VPN Gateway

The VPN gateway allows remote employees to connect to the internal network.

After authentication, users receive an internal IP address.

Example VPN address:

10.44.18.23

---

### Employee Workstations

Employees access the network using internal laptops or desktops.

Example endpoint referenced in the simulation:

FIN-LT-033

This workstation belongs to the compromised finance user.

---

### File Server

Sensitive research data is stored on the file server:

FS-RES-02

This server hosts the crown-jewel share:

\\FS-RES-02\Research_Contracts

---

## Network Segmentation

Network segmentation in the simulation environment is limited.

VPN users are placed on an internal subnet that allows access to multiple internal resources.

This weak segmentation allows compromised accounts to potentially access sensitive servers.

---

## Monitoring Points

Security telemetry exists at several locations:

- identity authentication logs
- MFA challenge logs
- VPN authentication records
- DNS queries
- proxy traffic
- file share audit logs

These logs allow investigators to reconstruct attacker activity.

---

## Investigation Strategy

Blue Team investigators correlate activity across:

- identity logs
- VPN session activity
- DNS queries
- proxy traffic
- file server access logs

This correlation helps identify:

- compromised identities
- lateral movement
- data staging
- possible exfiltration activity.

