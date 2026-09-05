# INC-002 — DNS Resolution Failure

## Incident Summary

**User:** Sarah Khan
**Department:** Finance
**Device:** FIN-PC-04
**Priority:** Medium
**Category:** DNS / Network

## User Report

User reported that websites could not be opened by hostname.

## Troubleshooting

### 1. Test Internet Connectivity

Command:

    ping 8.8.8.8

Result: Successful.

Finding: Internet connectivity was available.

### 2. Test DNS Resolution

Command:

    nslookup example.com

Result: IP address returned.

Finding: DNS resolution was functioning.

### 3. Test DNS Server Directly

Command:

    nslookup example.com 10.211.12.208

Result: IP address returned.

Finding: The configured DNS server was reachable and successfully resolving queries.

## Root Cause

No DNS fault was identified during the investigation.

The available evidence showed that:

- Internet connectivity was working.
- DNS resolution was working.
- The configured DNS server was responding.

## Resolution

No DNS configuration changes were made.

The user would be asked to reproduce the issue and provide the affected website and exact error message.

## Preventive Actions

- Record the exact hostname that fails.
- Test connectivity separately from DNS.
- Verify the configured DNS server.
- Test DNS resolution using `nslookup`.
- Avoid changing DNS configuration without evidence.

## Verification

Successful DNS resolution was confirmed using `nslookup`.