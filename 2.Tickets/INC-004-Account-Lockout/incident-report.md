# INC-004 — User Account Lockout

## Incident Summary

**User:** Priya Patel
**Department:** HR
**Device:** HR-PC-03
**Priority:** Medium
**Category:** Account / Authentication
**Status:** Investigated

## User Report

User reported that the account was locked despite entering the correct password.

## Troubleshooting Performed

### 1. Local Account Status

The test account was inspected using:

    Computer Management
    → Local Users and Groups
    → Users

Result: Account was not marked as locked out.

### 2. Security Event Log

Windows Event Viewer was inspected:

    Windows Logs
    → Security

Event ID 4624 was observed.

Finding: Successful logon activity was present.

### 3. Failed Logon Events

Event ID 4625 was searched for.

Result: No relevant 4625 event was identified during the investigation.

## Root Cause

A local account-lockout condition could not be reproduced or confirmed on the lab workstation.

## Resolution

No account changes were performed.

In a real enterprise environment, the Help Desk would verify the user's account status in Active Directory and investigate authentication failures before unlocking or resetting the account.

## Preventive Actions

- Verify account status before resetting passwords.
- Check authentication logs when repeated failures occur.
- Investigate devices or applications using outdated credentials.
- Document repeated lockouts for escalation.

## Technician Notes

The investigation demonstrated the importance of validating the reported symptom using account status and security logs rather than assuming that a failed login indicates an account lockout.