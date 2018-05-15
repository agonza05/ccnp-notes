Switching methods
-----------------

* Process switching: CPU process every packet -> Very slow
* Fast switching: CPU process the first packet and rest are cached in hardware -> Faster
* Cisco Express Forwarding (CEF): Forwarding is done in hardware -> Fastest

Cisco Express Forwarding
------------------------

* Also known as topology based switching
* Multilayer Switches create the forwarding tables in hardware
* Control Plane builds the Routing Table for L3
* Control Plane builds the ARP table for L2
* Data Plane builds the Forwarding Information Base (FIB) for L3
* Data Plane builds the Adjacency Table for L2

Commands
--------

1. Display Routing Table (Control Plane)
```
R1#show ip route
```
2. Display Forwarding Table (Data Plane)
```
R1#show ip cef
```
3. Display ARP Table (Control Plane)
```
R1#show mac address-table
```
4. Display Adjacency Table (Data Plane)
```
R1#show adjacency
```
