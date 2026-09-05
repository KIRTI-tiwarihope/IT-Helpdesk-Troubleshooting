# Account Troubleshooting Guide

## Purpose

This document records the account troubleshooting process performed during the Help Desk simulation.

## Tests Performed

### 1. Check Local User Accounts

Tool:

Computer Management (`compmgmt.msc`)

Location:

Local Users and Groups → Users

Purpose:

Used to review local user accounts and account properties.

Result:

The test account was present on the computer.

---

### 2. Check Account Lockout Status

Tool:

User account Properties

Purpose:

Used to determine whether the account was currently locked out.

Result:

The account was not marked as locked out.

---

### 3. Review Security Events

Tool:

Event Viewer (`eventvwr.msc`)

Location:

Windows Logs → Security

Purpose:

Used to investigate successful and failed logon activity.

Result:

A successful logon event (Event ID 4624) was observed.

No relevant failed logon event (Event ID 4625) was identified during the test.

## Final Diagnosis

An actual account lockout could not be reproduced or confirmed on the lab computer.

## Resolution

No account unlock or password reset was required.

## Enterprise Help Desk Procedure

In a real Active Directory environment, the Help Desk would:

1. Verify the user's identity.
2. Check the user's account status.
3. Determine whether the account is locked.
4. Review authentication failures.
5. Identify possible stale credentials or repeated failed logons.
6. Unlock or reset the account according to company policy.
7. Verify that the user can authenticate successfully.
8. Document the resolution.

## Help Desk Best Practice

Account troubleshooting should protect user security and follow the organization's identity verification and password-reset procedures.