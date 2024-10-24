---
section: issue
title: Paypal payments delayed
date: 2024-10-15T00:53:48.552Z
resolved: false
draft: false
informational: false
pin: false
resolvedWhen: 2024-10-24T09:47:45.711Z
affected:
  - WEB
severity: disrupted
---
*Update* - Still yet to receive any solution from Paypal. Only an acknowledgement of suspected fault on their end.

We are processing payments through our workaround as per normal. However there is still some element of unknown until paypal resolve the actual issue (which appears to be issues specifically with our x4b.net domain name)

As this issue does not have any known customer impact we are going to bring it to a close now.

Should you experience any delayed payments (either immeidately, or after 3 hours when the new correlation script can recover any missed payments) via paypal let us know and we will sort it out.

*Update* - Still yet to receive any solution from Paypal.

Our Transaction log check job remains in place. Having discovered a suspected workaround to the Paypal IPN system bug have implemented a workaround that appears to enable IPNs to be sent again. We will continue to run both.

*Update* - Still yet to receive any solution from Paypal.

We have implemented a payment check job which is able to import payments made once they are available via Paypal REST api (up to 3 hours). We understand this is inconvenient however at this time it is what we have available to us.

Paypal's IPN system has abruptly stopped communicating with us and we await a serious response from Paypal on this matter.

Stripe (Credit Card) and Crypto payments are unaffected. If you need to make an urgent payment we strongly recommend using Stripe until this matter can be resolved.

*Investigating* - Still yet to receive any solution from Paypal.

Transactions are being manually processed in a priority queue. Open a support ticket if you need manual processing urgently.

We are working on a temporary solution to reduce the delay to ~5-10 minutes while we wait on a fix from Paypal.

*Investigating* - We are aware of delays processing paypal payments. We have contacted Paypal merchant support for a fix and are awaiting a response.

If you need a payment manually processed open a support ticket including a screenshot of your payment and we will get to it ASAP.