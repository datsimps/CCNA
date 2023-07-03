# Lab 25

## Lab Intent:
Configure a loopback interface and EIGRP on each router.

![Lab25 screenshot](/Lab25.jpg)

## Thoughts:
We can create the loopback interface by just interfacing the loopback and giving it a number, i.e., “int loopback 0” to enter the loopback. Then we can assign it an IP address and the subnet mask, as shown in the screenshot on router 4. 

![Lab25Step3 screenshot](/Lab25Step3.jpg)

We activate the EIGRP with the router command. Following that, we assign the network to be included in the EIGRP with the network command. Using the passive interface command will tell the router not to send LSA’s to that interface, like the loopback interface. And we need to turn off auto summary to prevent the router from summarizing in classful updates. A screenshot from the exercise shows the routing protocol used, number of paths, the networks used and the passive interfaces.

![Lab25Step4 screenshot](/Lab25Step4.jpg)
