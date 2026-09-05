# INC-005 — Permission Denied

## Incident Summary

A simulated user reported being unable to access a confidential Finance file.

## User Report

User reported receiving a permission-related access problem when attempting to access:

`Finance-Confidential.txt`

## Troubleshooting Performed

1. Verified that the Finance-Confidential.txt file existed.
2. Reviewed the Security permissions on the lab folder.
3. Verified that the Finance-TestUser account was a standard local user.
4. Reviewed NTFS permissions assigned to the test account.
5. Tested file access using the Finance-TestUser account.

## Findings

The incident was investigated as a simulated NTFS permissions issue.

The Finance-TestUser account was configured with limited permissions to demonstrate how Windows file and folder access is controlled.

## Root Cause

Insufficient NTFS permissions assigned to the test user.

## Resolution

Permissions were reviewed and adjusted as part of the Help Desk troubleshooting simulation.

## Verification

File access was tested again after reviewing the permissions configuration.

## Preventive Actions

- Follow least-privilege principles.
- Review folder permissions regularly.
- Avoid granting unnecessary Full Control permissions.
- Use security groups rather than assigning permissions individually where possible.
- Document permission changes.

## Technician Notes

This incident demonstrates the importance of checking NTFS permissions when a user reports "Access Denied" or inability to open a file or folder.