---
section: issue
title: Paypal payments delayed
date: 2024-10-15T00:53:48.552Z
resolved: false
draft: false
informational: false
pin: false
resolvedWhen: 2024-10-16T00:53:48.564Z
affected:
  - WEB
severity: disrupted
---
*Update* - Still yet to receive any solution from Paypal.

We have implemented a payment check job which is able to import payments made once they are available via Paypal REST api (up to 3 hours). We understand this is inconvenient however at this time it is what we have available to us.

Paypal's IPN system has abruptly stopped communicating with us and we await a serious response from Paypal on this matter.

Stripe (Credit Card) and Crypto payments are unaffected. If you need to make an urgent payment we strongly recommend using Stripe until this matter can be resolved.

*Investigating* - Still yet to receive any solution from Paypal.

Transactions are being manually processed in a priority queue. Open a support ticket if you need manual processing urgently.

We are working on a temporary solution to reduce the delay to ~5-10 minutes while we wait on a fix from Paypal.

*Investigating* - We are aware of delays processing paypal payments. We have contacted Paypal merchant support for a fix and are awaiting a response.

If you need a payment manually processed open a support ticket including a screenshot of your payment and we will get to it ASAP.