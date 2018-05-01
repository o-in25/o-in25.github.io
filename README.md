# Networking Portfilio

# Homework 1
**R1** Hosts and end systems are usually used interchangeably. Hosts are often divided into two subsets, that is, clients and servers. Moreover, servers are typically used to describe more powerful computers than those of clients. End systems, however, include all hosts (and therefore all clients and servers), as well as desktop computers, phones, tablets, and laptops. Since a Web sever is a type of host, and hosts are usually interchangeable with end systems, Web servers are then considered end systems.

**R3** Standard of protocols are important because without a standardized method of communication, sending and receiving information would prove difficult. This would be analogous of two people attempting a conversation, but in different languages.

**R4**
Dial-up – home access
Cable Internet access – home access
Cellular mobile lines – WAWA
Wireless LAN – WAWA
Ethernet – enterprise
DSL –home access
##R7 Ethernet LAN’s transmission rates can often be between 10 Mpbs and 10 Gbps

**R8** Ethernet can be transmitted very quickly using fiber optic links and coaxial cables with thick radii. It can also be transmitted less quickly, however, through any twisted-pair copper wire

**R11** Since he total delay would be L/R from the sender and the switch and the delay from the switch and the receiver is L/R, the total time is 2L/R.

**R12** With a circuit-switched network, network quality is guaranteed since a dedicated, persistent connection must be acquired prior to establishing connection, where as, with a packet-switched network, as soon as a connection is established, data can be sent; however, since an indefinite of users can transmit over the network, bottlenecking occurs. In a CSN, TDM provides to be a more powerful and flexible form of multiplexing, because multiple digital signals can sent be transmitted over a single medium, whereas with FDM, there must be delay because only one transmission can be sent at any given time.

# Homework 2
**1** For the protocol, the following communications would be made
Client (ATM) to server (Mainframe)
Name:
INIT<id>
PASS<password>
BALE
WDRL <amount>
EXIT

Function:
Submit the username
Submit the password 
Get the balance
Withdraw an amount
Exit

Server to client 
Name:
PASS
VERF
ERNO
AMNT
EXIT

Function:
Get the password
Operation successful
Operation failed
The amount in the operation
Exit 

**R16** The delays are processing delays, propogation delays, transmission delays, and queuing delays. Queing is variable

**R18** 10 m/sec; d/s; no; no

**R19** 500kbps; 64 seconds; 100kbps; 320 seconds


# Homework 3
# Homework 4
# Homework 5
# Homework 6
**R19** With a mail exchanger record, which specifies the server responsible for managing incoming mail in the DNS, can link a host name with an IP address, therefore making it possible to have the same alias for a hostname and Web server.

**2** The response contains the sever name, the protocol method and the domain name, which are used by an MX to retrieve the information necessary to display the page.

**3** Using the type as MX, when sending the request to www.xavier.edu, what is returned is the protocol method, as well as postmaster which then identifies the administrator of the mail sever. I learned that this was different than other types used, for example Reverse.
# Homework 7
# Homework 8
# Homework 9
# Homework 10
**R6** From the text, to appreciate why a hardware implementation is needed, with a router's input ports, output ports, and switching fabric being handled by hardware, consider a 10Gbps input link and a 64-byte IP datagram; the input port has only 51.2ns to process the datagram before another datagram may arrive. If N ports are combined on a line card, the datagram-processing pipeline must operate N times faster - far too fast for software implementation. Similarly, executing routing protocols, performing management functions and comunicating with a SDN, are delt in much longer (by comparison) timeframes, making software a good choice. Additionally, the data plane is the physical forwarding of datagrams, while the control plane is the network-wide logic that routes them.

**R9** It is possible for for a destination address to match more than one entry. When there are multiple matches, the router uses the longest prefix matching rule, where it will find the longest matching entry in the table and forwards the packet to the link associated with the longest prefix match.

**R10** The first of the three types of switching fabrics is switching via memory. Here, switching between input and output ports are done under the control of the CPU and are traditional I/O devices. An input port with an arriving packet first signaled the routing CPU with an interrupt. Then, the packet was copied from the input port into processor memory. The routing CPU then extracted the destination address from the header, looked up the appropriate output port in the forwarding table, and then copied the packet to the output port's buffers. The second fabric is switching via bus. Here, an input port transfers a packet directly to the output port over a shared bus - with no CPU intervention needed. This is done by having the input port prepend a switch-internal header to the packet indicating the local output port to which the packet is being transfered and transmitting thr packet onto the bus. All output ports recieve the packet, but only the port that matches the label will keep it. Finally, the third fabric is switching via an interconnection network. A crossbar switch is an interconnection network consisting of 2n buses that connect N input ports to N output ports. Each vertical bus intersects each horizontal bus at a crosspoint, which can be opened and closed at any time by the switch fabric controller. When a packet arrives from point A and needs to be forwarded to port B, the switch controller closes the crosspoint at the intersection of A and Y, and then port A sends the packet onto its bus, which is picked up by Y. This, unlike its other two variants, supports parallel packet forwarding.

**R11** Packet loss occurs at the input ports when the traffic load or the relative speed of the switching fabric causes the router’s memory to become exhausted, with no room left for another packet. This can be avoided by making the input rate equal to the output rate via linespeed.

**R12** Packet loss occurs at the output ports when there are delays from the switching fabric takes too long to look up address in the table or when there is much demand. This can be circumvented with the use of output queues.

**R13** In an input queued switch, head-of-line blocking occurs when two packets at the front of their input queues are destined for the same output port. Suppose that the switch fabric chooses to transfer another packet. In this case, it must wait for the one before it be outputted. However, the packet that is waiting for 2 packets to "fight" for the same port must wait for an open, uncontested port.
# Homework 11
# Homework 12
# Homework 13
# Homework 14
# Homework 15


# Project 1
# Project 2
# Project 3

# Lab 1
# Lab 2
# Lab 3
# Lab 4 
## Part 1
**Question 1:** The difference between the protocol downgrade attack and Cain’s SSL MITM is that the protocol downgrade performed in the lab simply reroutes the traffic from the node to the machine, whereas Cain’s attack collects certificates that “contain the same parameters of the real ones except for asymmetric encryption keys; this deceives a lot of users to accept the server certificate and continue with the session.” The advantages of the protocol downgrade is that the attacker does not know that he or she has traffic that is being rerouted if the IP address and Gateway are exposed. With Cain’s method, SSL must be breached.
![image tooltip here](/docs/imgs/1an.png)
![image tooltip here](/docs/imgs/1bn.png)
![image tooltip here](/docs/imgs/1cn.png)

## Part 2
**Question 1:** Using protocols such as SSH with port forwarding is a much more secure alternative than with plain telnet.
![image tooltip here](/docs/imgs/2an.png)
![image tooltip here](/docs/imgs/2bn.png)
![image tooltip here](/docs/imgs/2cn.png)
![image tooltip here](/docs/imgs/2dn.png)
![image tooltip here](/docs/imgs/2en.png)
![image tooltip here](/docs/imgs/2fn.png)

## Part 3
**Question 1:** From bewaret.net
![image tooltip here](/docs/imgs/3an.png)
**Question 2:** Automatic drive by downloads can be by running browsers in restricted mode and by using tools such as Sandboxie
![image tooltip here](/docs/imgs/3bn.png)
![image tooltip here](/docs/imgs/3cn.png)

## Part 4
 **Question 1:** No; hiding SSID broadcasts are not a more reliable way to insure security as it simply will not display the SSID; the SSID can be found using tools like Wireshark and can be easily exposed
 **Question 2:** WPA2 > WPA > WEP
 **Question 3:** AES as it is an encrypting algorithm
![image tooltip here](/docs/imgs/4an.png)


