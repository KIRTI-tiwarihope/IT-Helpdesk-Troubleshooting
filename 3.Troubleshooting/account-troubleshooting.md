# Account Troubleshooting Guide

## Purpose

This document records the account troubleshooting process performed during the Help Desk simulation.

The troubleshooting was conducted in a controlled Windows lab environment using a dedicated test account.

---

## Troubleshooting Process

### 1. Check Local User Accounts

**Tool:**

Computer Management (`compmgmt.msc`)

**Location:**

Local Users and Groups → Users

**Purpose:**

Review local user accounts and account properties.

**Result:**

The dedicated test account was present on the computer.

**Finding:**

The account existed locally and could be reviewed through Windows account management tools.

---

### 2. Check Account Lockout Status

**Tool:**

User account Properties

**Purpose:**

Determine whether the account was currently marked as locked out.

**Result:**

The account was not marked as locked out.

**Finding:**

No active local account lockout was identified.

---

### 3. Review Security Events

**Tool:**

Event Viewer (`eventvwr.msc`)

**Location:**

Windows Logs → Security

**Purpose:**

Review authentication activity and identify evidence of successful or failed logon attempts.

**Result:**

A successful logon event (Event ID 4624) was observed.

No relevant failed logon event (Event ID 4625) was identified during the test.

**Finding:**

The available Security log evidence did not indicate repeated failed authentication attempts or a confirmed account lockout.

---

## Final Diagnosis

An actual account lockout could not be reproduced or confirmed on the lab computer.

The account was present, was not marked as locked out, and no relevant failed authentication events were identified during testing.

---

## Resolution

No account unlock or password reset was required because no active account lockout was identified.

The troubleshooting process was completed after verifying the account status and reviewing available authentication events.

---

## Verification

The following items were verified:

- The test account existed on the computer.
- The account was not marked as locked out.
- A successful logon event (4624) was present.
- No relevant failed logon event (4625) was identified.
- No account unlock or password reset was required.

---

## Enterprise Help Desk Procedure

In a real Active Directory environment, the Help Desk would:

1. Verify the user's identity according to company policy.
2. Check the user's account status.
3. Determine whether the account is locked.
4. Review authentication failures.
5. Identify possible stale credentials or repeated failed logons.
6. Check for other systems or devices generating failed authentication attempts.
7. Unlock or reset the account according to company policy.
8. Verify that the user can authenticate successfully.
9. Document the troubleshooting steps and resolution.

---

## Help Desk Best Practices

Account troubleshooting should protect user security and follow the organization's identity verification and password-reset procedures.

Help Desk personnel should avoid disabling security controls or resetting credentials without appropriate authorization.

---

## Evidence and Limitations

This incident was a controlled troubleshooting simulation rather than a production account-lockout incident.

The lab environment used local Windows account management rather than an enterprise Active Directory environment. Therefore, domain-level account lockout behavior and centralized authentication systems were not available for testing.

The diagnosis is based on the account status and Windows Security log evidence observed during the lab exercise.