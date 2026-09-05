# VPN Troubleshooting Guide

## Purpose

This document records the VPN troubleshooting process performed during the Help Desk simulation.

## Tests Performed

### 1. Check Network Connections

Tool:

Network Connections (`ncpa.cpl`)

Purpose:

Used to check available network adapters and VPN connections.

Result:

The computer had a working network connection, but no VPN connection was configured.

---

### 2. Check Windows VPN Settings

Location:

Settings → Network & Internet → VPN

Purpose:

Used to determine whether a VPN profile was configured.

Result:

No organizational VPN profile was configured.

---

### 3. Check Remote Access Connection Manager

Tool:

Services (`services.msc`)

Service:

Remote Access Connection Manager

Result:

The service was running and configured for Automatic startup.

Conclusion:

The Windows VPN-related service was available, but an organizational VPN profile was not configured.

## Final Diagnosis

The simulated VPN issue was caused by a missing VPN profile/configuration.

## Resolution

No VPN software or organizational VPN profile was installed on the lab computer.

In a real enterprise environment, the Help Desk would deploy or configure the approved corporate VPN according to company procedures.

## Help Desk Troubleshooting Process

1. Verify Internet connectivity.
2. Check available network adapters.
3. Check whether a VPN profile exists.
4. Check VPN-related Windows services.
5. Verify VPN credentials and configuration in an enterprise environment.
6. Escalate if the VPN server or authentication system is unavailable.
7. Document the findings.