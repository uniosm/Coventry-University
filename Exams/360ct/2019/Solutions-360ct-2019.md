**Answer paper for 360ct exam 2019**
>This module teaches Advanced Network Management and Design 

*Question 1a) Assuming the Administrative Distance of RIP is 120 and OSPF is 110, answer the following questions regarding the diagram provided.*
 
 ![Image of Diagram 1](https://github.com/uniosm/Coventry-University/blob/master/Exams/360ct/2019/images/diagram%20q1.png?raw=true)

*a1) How many broadcast and collision domains?*

**Solution:** In the diagram provided there are 7 collision domains and 5 broadcast domains. 

![Image of Diagram 1](https://github.com/uniosm/Coventry-University/blob/master/Exams/360ct/2019/images/solution.png?raw=true)


*a2) Which route a packet from PC1 to the Server follow if RIP routing protocol was used and why?*

**Solution:** A packet from PC1 to the Server using RIP routing protocol will follow the path PC1-S1-R1-R3-Server. The reason it
goes R1 to R3 over the serial cable 56Kbps is because RIP choses the path with the last number of hops. 


*a3) Which route a packet from PC1 to the Server follow if OSPF routing protocol was used and why?*

**Solution:** A packet from PC1 to the Server using OSPF routing protocol will follow the path PC1-S1-R1-R2-R3-Server. The reason it
differs from the previous protocol is because OSPF choses the path with the fastest bandwidth, therefore it avoids the serial cable
56Kbps which is slow. 


*a3) Assuming both RIP and OSPF were used simultaneously, which routes would be preferred and why?*

**Solution:** In complex company networks it's normal to have multiple routing protocols operating simulatenously. While it truly depends
on which protocol is set up to work on top of the other, in this particular case there is a high chance that OSPF will be used over
RIP as OSPF delivers higher performance. The route preferred would be R1-R2-R3 to R1-R3 because the last does not have the same
performance. 


*Question 1b) Discuss how OSPF (Open Shortest Path First) operates and the advantages of that approach. Would this protocol work for a small network with only a handful of networking devices?*

**Soluton:** 

*Question 1c) Due to a problem a routing loop has formed between four routing devices. What will happen to any packets entering it?*

**Solution:** When packets enter any of those four routing devices, they will not be able to reach the supposed destination because of the loop situation. Usually TTL (Time to live) is a mechanism implemented as a counter to limit the timespan of data and thuse those packets trapped in the loop may be discarded. 
