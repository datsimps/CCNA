# Lab 23

## Lab Intent:
Configure and use EtherChannel for load balancing.
![Lab23 screenshot](/Lab23.jpg)

## Thoughts: 
If we want to configure an EtherChannel to another switch we need to group the interfaces together using the “int range” command, then create the port channel with the channel-group command. When we create the group, we must give it a number, like a VLAN, and assign a mode.  Next, we have to go into the interface of the port-channel and set the switchport mode to trunk. After this we copy the steps to the connected interfaces.

The switches in this lab use a MAC address load balancing mode but the lab required us to set the mode to source-destination-IP. This deviates the load balancing from using source MAC addresses to using IP addresses to split the load. This allows loads to be balanced based on routes opposed to source devices. If one device does all the traffic, it won’t balance the load with the first option.
![Lab23Step62 screenshot](/Lab23Step62.jpg)