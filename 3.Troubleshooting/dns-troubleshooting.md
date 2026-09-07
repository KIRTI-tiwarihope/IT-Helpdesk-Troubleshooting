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

No active DNS fault was identified during the investigation.

The troubleshooting sequence confirmed:

- Working Internet connectivity independent of DNS
- Successful DNS resolution for the tested hostname
- Successful response from the specified DNS server

The original user-reported DNS problem could not be reproduced during the lab investigation. The incident was therefore treated as **No Fault Found (NFF)** pending recurrence with the affected hostname and exact error message.

> **Lab Note:** This investigation was performed in a controlled Windows lab environment. The results demonstrate the DNS troubleshooting methodology and diagnostic process rather than a production DNS incident.