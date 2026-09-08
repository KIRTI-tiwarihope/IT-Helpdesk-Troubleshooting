# VPN Troubleshooting Guide

## Purpose

This document records the VPN troubleshooting process performed during the Help Desk simulation.

The troubleshooting was conducted in a controlled Windows lab environment. No corporate VPN client or organizational VPN profile was configured on the test computer.

---

## Troubleshooting Process

### 1. Verify Network Connectivity

**Tool:**

Network Connections (`ncpa.cpl`)

**Purpose:**

Verify that the computer has an active network adapter and determine whether a VPN connection is present.

**Result:**

The computer had an active network connection, but no VPN connection was configured.

**Finding:**

Basic network connectivity was available, but there was no configured VPN connection to test.

---

### 2. Check Windows VPN Settings

**Location:**

Settings → Network & Internet → VPN

**Purpose:**

Determine whether a VPN profile is configured on the computer.

**Result:**

No organizational VPN profile was configured.

**Finding:**

The computer did not contain a corporate VPN configuration.

---

### 3. Check Remote Access Connection Manager

**Tool:**

Services (`services.msc`)

**Service:**

Remote Access Connection Manager

**Result:**

The service was running and configured for Automatic startup.

**Finding:**

The Windows VPN-related service was available and running. However, the presence of the service does not confirm that a corporate VPN profile or client configuration is installed.

---

## Final Diagnosis

The simulated VPN issue was associated with a missing VPN profile/configuration.

Because no organizational VPN profile was configured, a successful corporate VPN connection could not be established or tested on the lab computer.

---

## Resolution

No VPN software or organizational VPN profile was installed on the lab computer.

For the simulation, the missing VPN configuration was identified as the limiting factor.

In a real enterprise environment, the Help Desk would verify the approved VPN client, profile, authentication requirements, and deployment procedure before configuring the user's device.

---

## Verification

The following items were verified during troubleshooting:

- Network connectivity was available.
- A VPN-capable Windows service was running.
- No organizational VPN profile was present.
- No corporate VPN connection could be established because the required configuration was not available.

---

## Enterprise Help Desk Workflow

For a real VPN incident, the Help Desk should:

1. Verify Internet connectivity.
2. Check available network adapters.
3. Confirm whether the approved VPN client is installed.
4. Check whether the required VPN profile exists.
5. Verify VPN-related Windows services.
6. Verify VPN credentials and authentication requirements.
7. Check for VPN client or connection errors.
8. Determine whether the issue affects one user or multiple users.
9. Escalate if the VPN server, authentication system, or network service is unavailable.
10. Document troubleshooting steps, findings, and resolution.

---

## Evidence and Limitations

This incident was a controlled troubleshooting simulation rather than a production VPN outage.

The lab environment did not contain a corporate VPN client or organizational VPN profile. Therefore, an actual successful or failed corporate VPN connection could not be reproduced.

The diagnosis is based on the configuration observed during the lab exercise.