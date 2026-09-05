# IT Help Desk & Troubleshooting Simulation

## Project Overview

This project simulates the day-to-day activities of an IT Help Desk technician in a small enterprise environment.

The objective was to investigate common technical support incidents, perform structured troubleshooting, identify root causes, document resolutions, and recommend preventive actions.

The simulated organization is **Northstar Technologies**, a fictional company with approximately 50 employees across departments such as IT, HR, Finance, Sales, Operations, and Management.

---

## Project Objectives

- Investigate common IT support incidents.
- Apply structured troubleshooting methodologies.
- Use Windows administrative and diagnostic tools.
- Collect technical evidence before making configuration changes.
- Identify probable root causes.
- Document incidents professionally.
- Verify troubleshooting results.
- Recommend preventive actions.

---

## Incidents Investigated

| Ticket | Incident | Primary Skills |
|---|---|---|
| INC-001 | Network Connectivity | TCP/IP, Ping, IP Configuration, Tracert |
| INC-002 | DNS Resolution | DNS, Nslookup, Network Testing |
| INC-003 | VPN Connection | Windows VPN, Network Services |
| INC-004 | Account Lockout | Local Users, Event Viewer, Security Logs |
| INC-005 | Permission Denied | NTFS Permissions, User Access |
| INC-006 | Software Issue | Application Troubleshooting, Event Viewer |

---

## Tools Used

### Windows Tools

- Command Prompt
- `ipconfig`
- `ping`
- `nslookup`
- `tracert`
- Event Viewer
- Computer Management
- Local Users and Groups
- Services
- Network Connections
- Windows Settings
- Task Manager
- NTFS Security Permissions

---

## Troubleshooting Methodology

The project followed a structured troubleshooting process:

1. Understand the reported symptoms.
2. Gather information.
3. Reproduce the problem when possible.
4. Start with the simplest possible checks.
5. Collect technical evidence.
6. Identify the likely root cause.
7. Apply an appropriate resolution.
8. Verify the result.
9. Document the incident.
10. Recommend preventive actions.

---

## Project Structure

```text
IT-Helpdesk-Troubleshooting/
│
├── README.md
│
├── 01-Environment/
│
├── 02-Tickets/
│   ├── INC-001-Network-Connectivity/
│   ├── INC-002-DNS-Resolution/
│   ├── INC-003-VPN/
│   ├── INC-004-Account-Lockout/
│   ├── INC-005-Permissions/
│   └── INC-006-Software-Issue/
│
├── 03-Troubleshooting/
│   ├── network-troubleshooting.md
│   ├── dns-troubleshooting.md
│   ├── vpn-troubleshooting.md
│   ├── account-troubleshooting.md
│   └── software-troubleshooting.md
│
├── 04-Root-Cause-Analysis/
│   └── incident-summary.md
│
└── 05-Preventive-Actions/
    └── recommendations.md