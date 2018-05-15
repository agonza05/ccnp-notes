Core Knowledge
--------------
* The Control Plane is responsible for the routing protocols, creating the routing table and building the ARP table
* Based on the information of the Control Plane, devices build the tables of the Data Plane
* Multilayer Switch have an special type of hardware for forwarding packets or frames at wirespeed. These are called ASICs
* Majority of the forwarding is done on the Data Plane. Fast lookup and wirespeed is possible thanks to ASICs
* CAM and TCAM tables are stored in the ASICs

Content Addressable Memory (CAM)
--------------------------------
* The CAM table stores L2 information
  - Source MAC address
  - Interface where MAC was learned
  - VLAN that belongs to the MAC address
* Can match two values:
  - 0 = Do not compare
  - 1 = Compare
* Useful for when we need an exact match (MAC address lookup)

Ternary Content Addressable Memory (TCAM)
-----------------------------------------
* The CAM table stores L3 information (and above)
    - ACL
    - QoS
    - Routing table
* Can match three values:
  - 0 = Do not compare
  - 1 = Compare
  - x = Don't care
* Useful for when we do NOT need an exact match (subnet lookup)
