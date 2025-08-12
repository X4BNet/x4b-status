---
section: issue
title: Recaptcha Depreciation
date: 2025-08-12T04:29:29.110Z
resolved: true
draft: false
informational: false
pin: false
resolvedWhen: 2025-08-12T04:29:29.120Z
affected:
  - WEB
severity: notice
---
We are depreciating Recaptcha & recaptcha fallback for validation pages. Currently recaptcha is in use for less than 0.01% of all verification page requests so far in 2025 and with the exception of an attack utilizing a captcha solver (a growing risk that will be mitigated by removal) was similarly represented in 2024.

If any customer requires a no-javascript verification page they may contact us and we will see what we can do, however its our current belief given the analytics gathered from user agents and usage of the default PoW verification system that this is below a significant number.

We will of course be adding an appropriate message for clients without javascipt enabled when Recaptcha fallback & support is removed before the end of 2025.