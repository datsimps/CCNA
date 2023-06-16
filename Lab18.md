# Lab 18

## Lab Intent:
Introduction of the layer 3 switching.
![Lab18 screenshot](/Lab18.jpg)

## Thoughts:
The lab starts where the previous lab ends (lab covering the router on a stick). However, this lab aims to introduce the layer 3 switch. So, we need to dismantle the router on a stick configuration and use the layer 3 switch to route VLAN traffic, alleviating the extra traffic on the router.
![Lab18 Ping screenshot](/Lab18Ping.jpg)

![Lab18 screenshot](/Lab18NoSwitchport.jpg)

I set the router to default setting on the g0/0 interface and assigned it the IP address 10.0.0.194. This ends the trunk set between the router and the second switch. Then on the second switch, we delete the trunk ports on the g1/0/2 and use the “no switchport” command to end the trunk port. We can then activate the “ip routing” on the layer 3 switch to enable it to “ip route” for VLAN traffic. We assigned it the IP address of 10.0.0.193 to allow the routing of traffic to the router. Now we can ping from one end host on one VLAN, to another end host on another VLAN. Then if we enter the simulation mode, we can see layer 3 switch is the device regulating the VLAN traffic.
Notice that we are actually still sending the pings shown above, but the router is never actually used. For proof I have included the simulation of the ping, in the first screen shot below.
![Lab18 screenshot](/Lab18Switch.jpg)
The ping is actually send from the PC to the layer 3 switch and then sent to the correct VLAN as neeeded. The picture below is from the simulation where the ping is sent from the PC in VLAN 110 and then sent to a PC in VLAN 30. Showing the entirety of the ping proved to difficult when I am trying to keep these updates brief.
![Lab18 screenshot](/Lab18SwitchSend.jpg)