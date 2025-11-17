Here is a fun lab I did were I set up a network that utilizes OSPF, VLANs, LACP, 
Access Control Lists, and a DHCP server.

See my github link on my profile to download the file and see the full config.

 
This lab was about redundancy and security. This network has multiple routers 
that would connect to two different ISPs for redundancy. If one ISP had an outage 
and lost services, or if there were to be an issue with one of the routers, the 
network would still be able to reach the internet via the second router and ISP 
connection. OSPF was configured on the two routers and the two multi-layer switches, 
I configured a four-link port channel between the two multi-layer switches for more 
bandwidth and redundancy. 

Behind the Multi-layer switches I configured four layer 2 switches, each with a port 
channel connected to one of the multi-layer switches. I have also configured five 
VLANs on this network. Three of the VLANs are for different company departments, one 
is for the DHCP server and any additional servers, and one is for a guest network that 
is unable to reach the other subnets on the network except for the DHCP server, due to 
an ACL placed on SVI for the VLAN. 
