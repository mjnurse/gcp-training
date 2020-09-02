# Virtual Private Cloud (VPC) Networks

Contained within in a project.
Global Scope.
Subnets in regions.
Subnets can span zones.

Have routing tables to forward traffic
Have a global firewalls
Have define rules based on metadata tags (eg tag all webserevers as 'web' and open all port 80 on these).

VPC peering - allow two VPC to share traffic.
Shared VPC.

### Cloud Load Balancing

- Users get a single, global anycast IP address.
- Cross region load balancing.
- Traffic over Google backbone to closest point-of-presence.
- Traffic route based on backend load.
- Only healthy backends get traffic.
- No pre-warming required.

#### 5 VPC Load-balancing Options

(For external traffic)
1. **Global HTTP(S)** - Layer 7 based on load, Can route different URLS to different backends.
2. **Global SSL Proxy** - Layer 4 of non-HTTPS SSL based on load.  Supported on specific port numbers.
3. **Global TCP Proxy** - Layer 4 non-SSL TCP.  Supported on specific port numbers.
4. **Regional** - Any traffic (TCP, UDP).  Any port number.

(For internal traffic)

5. **Regional Internal** - Load bal' inside a VPC.  Use for internal tiers of multi-tier apps .  (eg between presentations and business layers).

### Cloud DNS

Create managed zones then add, edit, delete.
Programmable using API.

### Cloud CDN (content Delivery Network)

Uses distributed edge caches to cache content close to users.
Can use CDN interconnect to use of CDN.

### Interconnect Options

- **VPN** - Secure multi-Gbps over VPN tunnels.
- **Direct Peering** - Private connection between you and Google.  (No SLA).
- **Carrier Peering** - Connect through largest partners network of service providers.
- **Dedicated Interconnect**- Connect N x 10G transport circuits at Google POPs.










<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE1MTQ2NDc5NjgsLTE0MzA0NzcyOThdfQ
==
-->