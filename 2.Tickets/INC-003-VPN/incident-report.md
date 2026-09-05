# INC-003 — VPN Connection Failure

## Incident Summary

**User:** Rahul Sharma  
**Department:** Sales  
**Device:** SALES-PC-07  
**Location:** Remote  
**Priority:** Medium  
**Category:** VPN / Remote Access  
**Status:** Resolved

## User Report

User reported being unable to connect to the company VPN while working remotely.

## Initial Investigation

### 1. Internet Connectivity

Command:

    ping 8.8.8.8

Result: Successful.

Finding: Internet connectivity was available.

### 2. VPN Configuration

Windows Network Connections and VPN settings were inspected.

Result: No VPN connection/profile was configured.

Finding: The workstation did not have an organizational VPN connection configured.

### 3. VPN Service

Service checked:

    Remote Access Connection Manager

Result: Running.

Startup Type: Automatic.

Finding: The Windows VPN-related service was operational.

## Root Cause

The workstation did not have the required company VPN profile/configuration.

## Resolution

In a real enterprise environment, the approved VPN client/profile would be deployed according to company procedures.

No VPN configuration was installed on the personal lab computer.

## Verification

Internet connectivity was confirmed and the Windows VPN-related service was running.

## Preventive Actions

- Maintain documented VPN onboarding procedures.
- Verify VPN access is provisioned before remote work begins.
- Provide users with approved VPN client/profile instructions.
- Document VPN troubleshooting and escalation procedures.

## Technician Notes

The investigation ruled out a basic Internet connectivity problem and an obviously stopped Windows VPN service. The missing VPN configuration was identified as the primary issue in the simulated environment.