# Windows-server-homelab
This repo documents the setup and configurations for Active Directory in a virtual environment.

Active Directory Home Lab (Windows Server 2022)
Overview:
This project documents a Windows Server 2022 home lab built in VirtualBox to practice real-world help desk and Jr. system administration tasks.

Lab Environment:
Host OS: Windows 11 evaluation
Hypervisor: VirtualBox
Server OS: Windows Server 2022
Domain Controller: DC01
Domain: homelab.local



Initial Setup and Configuration:
Installed Windows Server 2022 in VirtualBox
Renamed the server to DC01
Configured static IPv4 networking



Active Directory Installation and User Management:
Installed and promoted Active Directory Domain Services
Verified domain functionality
Created organizational units (OUs) and user accounts
Performed password reset and account unlock tasks

## Overview
This project demonstrates the creation of a Windows Server homelab environment using VirtualBox. The lab simulates a real-world enterprise environment where Active Directory is used to manage users, enforce security policies, and monitor authentication events.

The goal of this lab was to gain hands-on experience with system administration and basic security monitoring techniques.

---

## Lab Environment

- Virtualization: VirtualBox
- Server: Windows Server (Domain Controller)
- Tools Used:
  - Active Directory Users and Computers
  - Group Policy Management
  - Event Viewer

---

## Active Directory Setup

- Created Organizational Units (OUs) to structure the environment
- Created multiple users and groups
- Assigned users to appropriate groups
- Simulated a real-world domain environment

---

## Security Configuration

Implemented password policies using Group Policy:
- Minimum password length
- Password complexity requirements
- Account lockout policies

These settings help protect against unauthorized access and brute-force attacks.

---

## Attack Simulation

Simulated a password attack by attempting multiple failed logins on user accounts.

This allowed me to observe how the system responds to suspicious authentication activity.

---

## Log Analysis (Event Viewer)

Used Event Viewer to analyze authentication logs:

- Event ID 4625 → Failed login attempt
- Event ID 4624 → Successful login

### Key Findings:
- Multiple failed login attempts were logged during the attack simulation
- Logs provide valuable insight into potential brute-force activity
- Event logs can be used by SOC analysts to detect suspicious behavior

---

## Skills Demonstrated

- Active Directory Administration
- User & Group Management
- Group Policy Configuration
- Windows Security Monitoring
- Log Analysis (Event Viewer)
- Basic Threat Detection

