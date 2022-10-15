---
section: issue
title: "Vegas: Offline"
date: 2022-10-14T18:25:00.000Z
resolved: true
draft: false
informational: false
resolvedWhen: 2022-10-15T07:50:10.046Z
affected:
  - LV1
severity: disrupted
---
U﻿pstream Incident Report - 



Short version:\
\
Networks' been crapping itself for the past day. After 2 - 3 hard failures today we did an emergency JunOS downgrade and are cautiously optimistic that it's resolved.\
\
Longer/technical version:\
\
For the past month or so we've been suffering a weird issue where random IP addresses would stop responding. The issue is that our router would lose/expire out the ARP entry for these IP addresses and wouldn't attempt to learn them again unless forced to.\
\
No amount of traffic getting sent to the IP externally (pings, random connection attempts, etc) would make the router issue an ARP "who-has" message. The only fix was to either ping the IP on the LAN (through our speedtest page for instance), forcing the router to see the ARP message on the network, or to login to the router and ping from there.\
\
No amount of limits, tweaks, process restarts, etc, has helped with this. The only way to date has been the above methods.\
\
This morning we had an issue where all users on 209.141.x.x dropped offline. These subnets had been moved down to our new Cisco core switch to help resolve the issue. Our Juniper router dropped the ARP entry for the Cisco switch, killing BGP. After some time it re-learned then entry reestablished connectivity, bringing those subnets back online.\
\
This happened three times in the past 24 hours, each outage lasting anywhere from 5 minutes to 30 minutes.\
\
Las Vegas is the only location suffering this issue. The key difference between all locations being that Vegas was running JunOS 20.4, where as everywhere else is 18.2~4. In JunOS 20.x they made changes to ARP to allow policing. While we did change this policy, it didn't help us any.\
\
As of an hour ago we performed a downgrade to JunOS 18.4. It obviously went terribly. After some research we found the configuration entry causing issues (our 100G ports kept channelizing) and fixed it, bringing things back online.\
\
As of now, ARP's are resolving near instantaneously, even for new IP addresses. We took this as a good time to change the rest of our ports to 100G, giving us a 400Gbit interlink between our router and core switch.\
\
We're cautiously optimistic that this issue is now resolved.\
\
We thank you for your patience.





\-﻿-

U﻿pstream reports that it is conducting emergency maintenance to downgrade the router firmware in an attempt to resolve issues.

\-﻿--

O﻿ffline again, ticket has been sent.

\-﻿--

U﻿pstream restored services.

T﻿he underlying issue (router bug) is still under investigation.

\-﻿--

Vegas upstream is offline. We have ticketed them and contacted staff members. We await response.