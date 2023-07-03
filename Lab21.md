# Lab 21

## Lab Intent:
Changing the root priority on a VLAN for load balancing.
![Lab21 screenshot](/Lab21.jpg)

## Thoughts:
Using the CLI we check the current Spanning-Tree Protocol (STP) topology. I have included the screenshots of the topology, note the SW2 as the root bridge.
![Lab21Step3 screenshot](/Lab21Step3.jpg)
We can see each role/state of the ports of each switch. Then we change the configuration on SW1 to become VLAN 1 root primary and VLAN 2 root secondary. As we can see the change annotated in port roles. 
