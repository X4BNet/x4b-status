---
section: issue
title: Lumen APAC Upgrade
date: 2021-07-19T04:29:53.262Z
resolved: false
draft: false
informational: false
resolvedWhen: 2021-07-19T04:29:53.276Z
affected:
  - SGP1
  - TOK1
severity: notice
---
We are currently in the process of onboarding our new (replacement) transit provider Lumen (formerly Level3). Due to delays in port turn up the NTT turn down date for APAC is scheduled to occur prior to the turn up of ports in US and EU. 

To ensure the Anycast network remains balanced we have done extensive traffic engineering works over the past week which were applied this hour. We expect most customer routes will be unaffected.

We do note some troublesome routes, particularly those of AS6939 (Hurricane Electric) who peers very poorly with both NTT and GTT (not at all) our current US & EU transits. We are discussing mitigation strategies with our upstream provider however in the interim we expect some Asian HE traffic to be direct to the US (specifically LA). This is a problem which will affect singlehomed HE networks. This issue and any others like it should be resolved fully within the month as Lumen lights the remaining ports.

Please feel free to report bad routes to support and we will see what we can do about them.