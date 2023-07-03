# Lab 22

## Lab Intent:
Introduction and identification of Rapids Spanning-Tree Protocol (RSTP). This also introduces the RSTP link types.
![Lab22 screenshot](/Lab22.jpg)

## Thoughts: 
We can see that SW1 is the root bridge, tied priorities goes to the lowest MAC address. 
![Lab22Step1 screenshot](/Lab22Step1.jpg)
On the first step we need to identify what is different about this root bridge, my understanding is the fact that both F0/2 and F0/3 are designated ports. But one should be “blocking”, upon further investigation it is a PT error with the hub. One should be blocking, which would make this the answer because all ports should typically be designated not blocking.  

I have identified the roles/states of each port in the screenshot listed below.
![Lab22Step2 screenshot](/Lab22Step2.jpg)
For the link types I have configured: SW1 f0/1, SW2 f0/1 – 2 and g0/1, SW3 f0/1 – 2 and g0/1, and SW4 f0/1 – 2 as link-type point-to-point. I set: SW2 f0/23 -24, SW3 f0/24, and SW4 f0/24 to spanning tree portfast.  I set SW1 f0/2 – 3 to link-type shared, for the hub connections. Since SW1 f0/24 is connected to a hub on edge ports, it will be considered an edge, but with half duplex.