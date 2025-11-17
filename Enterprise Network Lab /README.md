Here is a Packet Tracer lab that I worked on over the weekend. The goal was to configure 
the devices so that network traffic could traverse the access-layer, distribution-layer, 
and core-layers of the network without any issues. 

-I configured five VLANs (10-Staff, 20-IT ,30-Admin, 90-Server, and 99-Management) on each 
switch. As well as enabling each switch to use RSTP.

-I configured access ports on ports connects to end hosts, and trunk ports that connected 
to other switches. Ensuring that traffic could move between the different layers of the network, 
on both primary and redudent links.

-I then configured the SVIs on the two core-layer switches (primary on the left, secondary 
on the right) to be the primary and secondary gateways for the individual VLANs. 

-Moving on the router, I included NAT configurations in this lab so that I could simulate a 
LAN that uses port address translation (PAT), which would convert public IPs from the ISP to 
private IPs on the private network, and visa-versa. 

-I also configured the router as the DHCP server, using the SVIs I configured on the core-layer 
switches as DHCP relays to the router. 

-OSPF was configured on the core-layer switches, and the router to ensure that all traffic 
could be routed in, out of, and across the network.
