# Lab 17

## Lab Intent:
Configure VLANs with the proper interfaces, establish a trunk port, and set up a router on a stick.
![Lab17 screenshot](/Lab17.jpg)

## Thoughts:
If you forget to create the VLAN on both switches, you will not be able to ping across the switches regardless of if the router sends the ping back. The correct way to set up the switches is to allow the VLAN that is connected to the switch access to the trunk. Then the switch connected to the router should have two trunks.
![Lab17 Ping screenshot](/Lab17Ping.jpg)
I can also use "show int trunk" command to verify the actual status on each of the port. Notice the term "trunking" under the status column. This shows that both the g0/1 and g0/2 are both acting as trunks under this particular switch.
![Lab17 Trunk screenshot](/Lab17Trunk.jpg)