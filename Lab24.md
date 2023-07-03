# Lab 24

## Lab Intent:
To configure floating static routes for redundancy.

![Lab24 screenshot](/Lab24.jpg)

## Thoughts: 
We check the current routes to see what routing protocol is being used, which is OSPF.
We ping SRV1 from PC1. Then we ping the IP of 1.1.1.1 from PC1. Then we configure the floating static route between R1 and R2, going across ISP A. When configuring the static route we add the weight of the new route, i.e. the 120. The weight is used to keep this route as a secondary route, weighting it higher than the default route. When we shut down the route between R1 and R2, we still have the secondary route that allows use to still ping the server. 

![Lab24Step2pt1 screenshot](/Lab24Step2pt1.jpg)
