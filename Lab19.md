# Lab 19

## Lab Intent: 
Introduction of Dynamic Trunking Protocol (DTP) and VLAN Trunking Protocol (VTP)
![Lab19 screenshot](/Lab19.jpg)

## Thoughts:
There are two different modes of DTP, auto or desirable. desirable wants to set up a trunking protocol, allowing desirable to establish trunks with other desirables, trunks, or autos. However, autos will set up trunks only with other switches that are desirable or trunks. We want to disable the DTP. In this lab we disable the DTP and confirm with the “show interface g0/1 switchport” command and looking at the “negotiation of trunking…” line.
![Lab19 screenshot](/Lab19DisableDTP.jpg)

VTP stands for VLAN Trunking Protocol and is used to update VLANs across different switches to ensure uniformity. It sounds great on paper but should be disabled. If we add a switch to the network that is outdated but has this feature enabled, it can overwrite the current VLAN settings in effect. VTP has three different modes: server, client and transparent. Server can create the different VLANs and delete, whereas client can only update according to the server. Servers can also take the information from a client (if the client has a higher revision number) and update their own VLAN settings. Transparent does not broadcast its revision number to change the VLAN settings of other switches. In this lab we show the difference between the modes. The lab asks you to perform the task then see the changes in the VLANs afterwards. We disable the VTP at the end of the lab for best practice reasons. 
![Lab19 screenshot](/Lab19VLAN.jpg)