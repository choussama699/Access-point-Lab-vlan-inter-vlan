# Access-point-Lab-vlan-inter-vlan


VLANs with Wireless Access Points and Inter-VLAN Routing


A small campus-style network that segments wired and wireless clients into three VLANs on a single Cisco switch. Two access points connect wireless clients to their own VLANs, and one router provides inter-VLAN routing using the router-on-a-stick method.


Network Design
VLAN	Name	Subnet	        Gateway      	Devices              	Connection
10	VLAN10	192.168.10.0/24	192.168.10.1	Laptop0, PC0, Laptop1	Wireless via Access Point0
20	VLAN20	192.168.20.0/24	192.168.20.1	Laptop2, Laptop3    	Wireless via Access Point4
30	VLAN30	192.168.30.0/24	192.168.30.1	PC2	                  Wired to Switch0

Verification
show vlan brief
show interfaces trunk
show ip interface brief      ! on the router
show ip route                ! on the router
