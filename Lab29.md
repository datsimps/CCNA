# Lab 29

## Lab Intent:
Configure and use HSRP on the network.

![Lab29 screenshot](/Lab29.jpg)

## Thoughts: 
HSRP is used to provide redundancy to the network. If you set a route to move traffic outside of the network, then you provide a single way out of the network. If that router goes down for any reason, the traffic that relied on it to contact other networks can no longer reach the outside networks. But if we create a Virtual IP (VIP) then we can use two routers to reach the outside networks. Both routers share a VIP, and they can both be used to forward traffic. If one router goes down, the other router will take over. Using the preempt key word allows for one router to resume the primary role.

![Lab29Step2 screenshot](/Lab29Step2.jpg)

We set R1s priority above the default and R2s to lower than the default. This ensures that R1 becomes the primary router. So, if R1 goes down, R2 will take over. But if R1 comes back up, R2 remains the primary router. If we use the preempt keyword on R1, when it comes back online, it will take back over as the primary router.

![Lab29Step4 screenshot](/Lab29Step4.jpg)
