# Lab 15

## Lab Intent:
Given an IP address subnet the IP into five networks with various number of hosts (VLSM). After assigning the VLAN an IP address, assign the default gateway and IP address to PC 1 and PC 4. The test is PC 1’s ability to ping PC 4.
![Lab15 screenshot](/Lab15.jpg)

## Thoughts:
Given the nature of the subnet I made a lot of errors by mismatching the IP address to the subnet. I wrote the subnets down on a piece of paper in descending order by the host requirements but the VLANs were obviously not already in that order. So, I mismatched the IP to the wrong VLAN, led to some troubleshooting but it wasn’t too bad. Something for me to keep an eye on moving forward. The static route was easy to set, allowing for safeguards with invalid inputs not being accepted if you are assigning things that aren’t viable networks.
![Lab15 screenshot](/Lab15Ping.jpg)