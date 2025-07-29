---
section: issue
title: Cloud Service outage
date: 2025-07-27T11:08:06.977Z
resolved: false
draft: false
informational: false
pin: false
resolvedWhen: 2025-07-28T01:46:53.712Z
affected:
  - WEB
severity: disrupted
---
*Update* No update from Akamai yet but we are seeing Kubernetes nodes that were offline return to function slowly starting around 5 minutes ago.

*Update* We currently await Akamai to fix their internal networking. 4/12 of our cluster nodes are currently online. The panel is up but slow. Some non essential services that rely on inter-node communication are degraded. 

*Update* Panel is currently very slow due to 70% of cloud nodes being offline currently. We await Akamai's resolution to their datacenter outage.

We apologise for the inconvenience and are doing everything we can to return to 100%. Even including moving our services to another vendor.

If you would like to follow the [upstream issue](https://status.linode.com/incidents/6yw88b0ft94g) you may.

*Update* We will be keeping this incident open for now as we are still seeing substantially lowered performance in the region and half of our cluster nodes are still unavailable. The panel is however online.

We continue to monitor the [upstream issue](https://status.linode.com/incidents/6yw88b0ft94g) and await resolution.

*Update* We will be keeping this incident open for now as we are still seeing substantially lowered performance in the region and some of our cluster nodes are still unavailable. The panel is however online.

*Update* Holy Smokes Akamai that was a long one. Services are restored. We are going through and checking everything in line with our DRP.


Upstream Update - 
Our SMEs continue to work bringing our services back online, and we will provide an update as progress is made.

Upstream Update - 
Identified - Our team has identified the issue affecting connectivity in our US-EAST (Newark) data center. The issue is related to heating/cooling complications in the data center due to a power outage . The power outage has been fixed and we are working quickly to bring our services back online, and we will provide an update as soon as the solution is in place.

Upstream currently has an outage affecting their US-EAST PoP where our core cloud (web panel, data collection, etc) is homed. This does not affect customer services are all essential services (BGP, route validation, mitigation analysis) is multi-homed. Email delivery (i.e on DDoS attack) will not be available until service restored.

"Investigating - Our team is investigating an emerging service issue affecting All Services in US-EAST (Newark). We will share additional updates as we have more information."