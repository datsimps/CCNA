# Lab 20

# Lab Intent:
Identify the root bridge, and the status/roles of ports on all switches.
![Lab20 screenshot](/Lab20.jpg)

## Thoughts: 
The switch with the lowest priority becomes the root bridge. Ties in the priority will be resolved with the lowest MAC address. This leaves SW3 as the root bridge. From the root bridge all ports become designated ports. From the root bridge, SW1 connects two separate ports. Port F0/3 is across from the F0/2 port from SW1. Since the neighbor port is higher than the connection from SW1’s F0/1, then it blocks. This allows the F0/4 port to receive over the F0/3 port. SW4 receives from the root bridge. Since the SW4 mac address is lower than the MAC address of SW2, it possesses the designated port. The cost coming from to gigabit routes is less than the cost coming from an ethernet, so SW2 receives from SW4 and blocks from the root bridge. SW2 has a lower MAC address so it possesses the designated ports connected to SW1. SW1 blocks these ports as it has already found the lowest cost from the root bridge. Looking at the screenshot below we can see that on SW1 ports 0/1 - 3 are blocking and forward from the root bridge.
![Lab20SW1Port screenshot](/Lab20SW1Port.jpg)