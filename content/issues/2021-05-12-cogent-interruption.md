---
section: issue
title: Cogent interruption
date: 2021-05-12T17:00:00.000Z
resolved: true
draft: false
informational: false
resolvedWhen: 2021-05-12T20:14:36.632Z
affected:
  - LAX1
  - AMS1
severity: disrupted
---
*Investigating* - We are investigating a potential issue that might affect the uptime of one our of services. We are sorry for any inconvenience this may cause you. This incident post will be updated once we have more information.

*Investigating* - We have narrowed the issue down to outgoing routes going over Cogent in two locations (AMS & LAX)

*Identified* - Cogent activated uRPF (without notice) on our upstream ports (2 PoPs) leading to an interruption as we don't use Cogent for Ingress but they are used (if they are the best route) for Egress selectively.

To resolve this we are now exporting ingress routes to Cogent with Cogents own no-export community.