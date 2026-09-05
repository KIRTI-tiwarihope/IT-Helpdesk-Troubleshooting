# INC-001 — Network Connectivity

## Incident Summary

**User:** Sarah Khan  
**Department:** Finance  
**Device:** FIN-PC-04  
**Priority:** Medium  
**Category:** Network Connectivity  
**Status:** Resolved / No Fault Found

## User Report

User reported being unable to access websites.

## Initial Symptoms

The user believed the workstation had lost Internet connectivity.

## Troubleshooting Performed

### 1. Loopback Test

Command:

    ping 127.0.0.1

Result: Successful.

Finding: The local TCP/IP stack was functioning.

### 2. Default Gateway Test

Command:

    ping 10.211.12.208

Result: Successful.

Finding: The workstation could communicate with the local network gateway.

### 3. External Connectivity Test

Command:

    ping 8.8.8.8

Result: Successful.

Finding: External network connectivity was available.

### 4. DNS Test

Command:

    nslookup google.com

Result: Successful.

Finding: DNS resolution was functioning correctly.

### 5. Route Test

Command:

    tracert google.com

Result: Trace completed successfully.

Finding: The workstation was able to reach the destination.

## Root Cause

No network fault was identified during troubleshooting.

Testing confirmed that local connectivity, Internet connectivity, DNS resolution and routing were functioning normally.

## Resolution

No configuration changes were required.

The user should be asked to reproduce the original problem and provide the specific website/application that failed if the issue occurs again.

## Preventive Action

- Ask users to provide the exact error message when reporting connectivity issues.
- Record the affected website/application.
- Check whether the issue affects other users.
- Follow the standard network troubleshooting procedure before changing configuration.

## Verification

Network connectivity and DNS resolution were successfully verified using standard Windows troubleshooting tools.

## Technician Notes

The investigation demonstrated a structured troubleshooting approach rather than making assumptions based solely on the user's initial report.