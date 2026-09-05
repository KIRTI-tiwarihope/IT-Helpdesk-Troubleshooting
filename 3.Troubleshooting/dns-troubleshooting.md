# DNS Troubleshooting Guide

## Purpose

This document records the DNS troubleshooting process performed during the Help Desk simulation.

## Tests Performed

### 1. Test Internet Connectivity

Command:

ping 8.8.8.8

Purpose:

Used to determine whether Internet connectivity was available independently of DNS.

Result:

Successful replies were received.

Conclusion:

Internet connectivity was working.

---

### 2. Test DNS Resolution

Command:

nslookup example.com

Purpose:

Used to determine whether DNS could resolve a domain name into an IP address.

Result:

DNS successfully returned an IP address.

Conclusion:

DNS resolution was working.

---

### 3. Test the Configured DNS Server

Command:

nslookup example.com 10.211.12.208

Purpose:

Used to test DNS resolution through the specified DNS server.

Result:

The DNS server successfully returned an IP address.

Conclusion:

The configured DNS server was responding to DNS queries.

## Final Diagnosis

No DNS fault was identified during testing.

The reported DNS problem could not be reproduced.

## Help Desk Troubleshooting Process

1. Test Internet connectivity by IP address.
2. Test DNS name resolution.
3. Test the configured DNS server directly.
4. Compare the results.
5. Document the findings.