# Organization Profile – WVRUS

## Overview

WVRUS (Wyoming Valley Research and University Services) is a simulated organization used in the Cybersecurity Color Wheel Simulation.

The organization supports research, administrative operations, and student services. Several systems contain sensitive information, including research contracts and student records.

---

## Departments

The organization contains several operational departments:

- Finance
- Research Administration
- IT Operations
- Student Services
- Academic Departments

Employees authenticate through a centralized identity provider.

---

## Core Infrastructure

### Identity Provider

The Identity Provider (IdP) manages authentication and access control.

It provides:

- user authentication
- multi-factor authentication (MFA)
- single sign-on (SSO)
- conditional access policies

---

### VPN Gateway

The VPN gateway allows employees to remotely access internal systems.

Once authenticated, users receive an internal IP address and gain access to internal network resources.

---

### File Servers

Sensitive research documents are stored on internal file servers.

The primary server in the simulation is:

FS-RES-02

---

## Crown Jewel Systems

Crown jewels represent the most sensitive organizational assets.

### Primary Crown Jewel

\\FS-RES-02\Research_Contracts

This share contains:

- research contracts
- deliverables
- partner agreements
- sensitive research documentation

---

### Secondary Crown Jewel

Student_Records

This system contains student data and academic records.

---

## Key Accounts

### jordan.rivera@wvrus.org

Finance employee whose credentials were compromised in the simulation.

### svc-backup-reports

Automated service account used for reporting and backup tasks.

Service accounts often have elevated privileges and may be abused during lateral movement.

---

## Security Controls

### Identity Security

Security measures include:

- multi-factor authentication
- conditional access alerts
- risk-based sign-in detection

However, MFA relies on push approval without number matching.

---

### Monitoring

Available telemetry includes:

- identity authentication logs
- VPN authentication logs
- DNS resolver logs
- partial proxy logs
- file share audit logs

---

### Endpoint Visibility

Endpoint Detection and Response (EDR) coverage is incomplete.

Some endpoints are not enrolled in EDR, creating investigation blind spots.

---

## Business Constraints

The organization has limited tolerance for downtime.

Critical operations include:

- payroll processing
- research administration
- student services

Security responses must balance containment with operational continuity.


