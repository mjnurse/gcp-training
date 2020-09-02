---


---

<h1 id="virtual-private-cloud-vpc-networks">Virtual Private Cloud (VPC) Networks</h1>
<p>Contained within in a project.<br>
Global Scope.<br>
Subnets in regions.<br>
Subnets can span zones.</p>
<p>Have routing tables to forward traffic<br>
Have a global firewalls<br>
Have define rules based on metadata tags (eg tag all webserevers as ‘web’ and open all port 80 on these).</p>
<p>VPC peering - allow two VPC to share traffic.<br>
Shared VPC.</p>
<h3 id="cloud-load-balancing">Cloud Load Balancing</h3>
<ul>
<li>Users get a single, global anycast IP address.</li>
<li>Cross region load balancing.</li>
<li>Traffic over Google backbone to closest point-of-presence.</li>
<li>Traffic route based on backend load.</li>
<li>Only healthy backends get traffic.</li>
<li>No pre-warming required.</li>
</ul>
<h4 id="vpc-load-balancing-options">5 VPC Load-balancing Options</h4>
<p>(For external traffic)</p>
<ol>
<li><strong>Global HTTP(S)</strong> - Layer 7 based on load, Can route different URLS to different backends.</li>
<li><strong>Global SSL Proxy</strong> - Layer 4 of non-HTTPS SSL based on load.  Supported on specific port numbers.</li>
<li><strong>Global TCP Proxy</strong> - Layer 4 non-SSL TCP.  Supported on specific port numbers.</li>
<li><strong>Regional</strong> - Any traffic (TCP, UDP).  Any port number.</li>
</ol>
<p>(For internal traffic)</p>
<ol start="5">
<li><strong>Regional Internal</strong> - Load bal’ inside a VPC.  Use for internal tiers of multi-tier apps .  (eg between presentations and business layers).</li>
</ol>
<h3 id="cloud-dns">Cloud DNS</h3>
<p>Create managed zones then add, edit, delete.<br>
Programmable using API.</p>
<h3 id="cloud-cdn-content-delivery-network">Cloud CDN (content Delivery Network)</h3>
<p>Uses distributed edge caches to cache content close to users.<br>
Can use CDN interconnect to use of CDN.</p>
<h3 id="interconnect-options">Interconnect Options</h3>
<ul>
<li><strong>VPN</strong> - Secure multi-Gbps over VPN tunnels.</li>
<li><strong>Direct Peering</strong> - Private connection between you and Google.  (No SLA).</li>
<li><strong>Carrier Peering</strong> - Connect through largest partners network of service providers.</li>
<li><strong>Dedicated Interconnect</strong>- Connect N x 10G transport circuits at Google POPs.</li>
</ul>

