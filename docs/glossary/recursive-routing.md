Router process of doing multiple lookups to reach a certain network.

Example
-------

```
R1#show ip route
[...]
Gateway of last resort is not set
C 192.168.12.0/24 is directly connected, FastEthernet0/0
 3.0.0.0/24 is subnetted, 1 subnets
S 3.3.3.0 [1/0] via 192.168.23.3
S 192.168.23.0/24 [1/0] via 192.168.12.2
```

Lookups
-------

1. Next hop for 3.3.3.0/24
2. Next hop for 192.168.23.3
3. Next hop for 192.168.12.2
