**Answer paper for 360ct exam 2019**
>This module teaches Advanced Network Management and Design 

*Question 1a) Assuming the Administrative Distance of RIP is 120 and OSPF is 110, answer the following questions regarding the diagram provided.*
 
 ![Image of Diagram 1](https://github.com/uniosm/Coventry-University/blob/master/Exams/360ct/2019/images/diagram%20q1.png?raw=true)

*a1) How many broadcast and collision domains?*

**Solution:** In the diagram provided there are 7 collision domains and 5 broadcast domains. 

![Image of Diagram 1](https://github.com/uniosm/Coventry-University/blob/master/Exams/360ct/2019/images/solution.png?raw=true)


*a2) Which route a packet from PC1 to the Server follow if RIP routing protocol was used and why?*

**Solution:** A packet from PC1 to the Server using RIP routing protocol will follow the path PC1-S1-R1-R3-Server. The reason it
goes R1 to R3 over the serial cable 56Kbps is because RIP choses the path with the least number of hops. 


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

*Question 2a) In the context of network design what is meant by the term “network diameter”? Briefly discuss the effects of increasing this value.*

**Solution:**

*Question 2b) Briefly discuss the advantages of employing a “layered” approach towards network design.*

**Solution:**


*Question 2c) Explain the three-tier hierarchical network design approach. Name the three layers and discuss their role, function and relationship with each other.*

**Solution:** A company called CISCO suggested the tree layer design. Those layers are: core layer which acts as the backbone, distribution layer which implies policies and routing amongst VLANs and access layer that provides the means for connecting devices. Core layer is designed to switch packets as fast as possible and doesn't perform packet manipulation (access list, filtering, etc.). Instead, those function are carried on the distribution layer which can be summarized as the layer providing policy-based connectivty. Finally, access layer is the point where end users are allowed into the network. This layer may implement further policy-based rules or not. There are other alternatives to the three layer design where the core and distribution layer are merged. 

*Question 3a)Explain how the two TCP/IP transport layer protocols (TCP and UDP) are employed in the context of VoIP telephony*

**Solution:** Because voice is a type of data, we don't necessarily need a voice only circuit network. VoIP or Voice over IP is IP telephony. It uses RTP or real-time transport protocol while employing UDP packets. UDP packets compared to TCP packets don't need to be fixed in case they have errors. The H.323 model is a protocol suite used in VoIP telephone which can use both UDP and TCP packets. TCP is used for signalling while UDP is implemented for audio and video transfer. 

*Question 3b) One of the features of PPP is “multilink”. Briefly explain what this involves and what the advantages of this would be.*

**Solution:**

*Question 3c) Briefly explain “connection oriented” and “connectionless” communication.*

**Solution:**

*Question 3d) Explain QoS (Quality of Service) in the context of VoIP and describe the three methods that could be employed.*

**Solution:** In VoIP quality of service helps ensuring a certain standard of service in regards to loss, signal to noise ratio, crosstalk, etc. Quality of Service helps with packet loss, jitter and handling delay. There are three models of QoS and those are: none: best effort delivery; integrated service: reserve bandwidth for voice; differentiated: classifies different types of traffic

*Question 3c) Extended Unique Identifier (EUI), allows a host to assign itself a unique 64-Bit IPv6 interface identifier (EUI-64). Briefly explain the steps involved in doing so and write down the IPv6 address generated given the MAC address FF-11-11-22-22-22.*

**Solution:**


