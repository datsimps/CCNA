# Lab 28

## Lab Intent: 
Troubleshoot the OSPF routers.

![Lab28 screenshot](/Lab28.jpg)

## Thoughts: 
A troubleshooting lab over OSPF, I feel as if it is another key lab. The lab starts off by telling you to configure the serial connection between two routers then enabling OSPF. Then you must uncover the problem on R3. The problem took some time to find but it ended up being a mismatched network. One router was using the “point-to-point” network and the other was not, so it didn’t dynamically add the network to the route table.

![Lab28Step2 screenshot](/Lab28Step2.jpg)

The next problem was a different hello and dead timer on either side of the routers. The difference will result in a route not being added. But it is an easy fix. 

![Lab28Step3 screenshot](/Lab28Step3.jpg)

The final problem was with the fifth router. The router did annotate it would have a default route outside of the network, but no route was ever set. Including the default route cleared the issue and allowed both PCs on the network to communicate with the router on the outside of the network.

![Lab28Step4 screenshot](/Lab28Step4.jpg)
