# The OSI Model:
The OSI model or, Open Systems Interconnection Model, describes network communication in various layers. In total, there are Seven Layers to the OSI Model. These layers include:

 1. Physical
 2. Data Link
 3. Network
 4. Transport
 5. Session
 6. Presentation
 7. Application

The first four layers are considered the primitive layers. These layers specifically, and most commonly describe the transportation of data throughout network communication. Layers Five to Seven, the higher-up layers are more associated with Application-Level-Data. Networks typically operate to the rule of "Pass it On" in which, each layer is responsible for a specific task. Once the task is complete, the layer will pass on the data to the next layer in the grid. A terrible analogy for this would be a Spicy Italian sub from Subway. The bread represents the Physical Layer and the additional layers are the food and internal layers which form the architecture of the network. All providing a crucial role in the transfer of food into the mouth of receiver..

This image taken from Webopedia beautifully showcases the OSI Model in a graphical format. 
Despite the format I wrote above, the OSI Model goes in descending order, starting from 7.


![7 Layers of the OSI Diagram](https://www.webopedia.com/imagesvr_ce/8023/7-layers-of-osi-icon.jpg)

## 7 - The Application Layer:
The application layer, the seventh layer in the OSI Model supports application and end-user processes. The application layer is also responsible for identifying processes such as Communication Partners, Quality of Service, User Authentication, Privacy and all syntax constraints which may affect data. As formerly mentioned, layers 5 to 7 are all Application Specific. You will recognize this layer for its utilization in providing application devices for common actions such as File Transfer and E-Mail Communication. Telnet and FTP are applications which exist completely within this layer. Real life examples of this layer in action include URL Search Bars in Browses, the HTTP Protocol, the FTP Protocol, the NFS Protocol and the SNMP Protocol. 

# 6 - The Presentation Layer:
The presentation layer, the sixth layer in the OSI Model transforms data into a presentable form which the application layer can accept. Also known as the Syntax Layer, the presentation layer encrypts application data to network data, and decrypts Network data into Application Data. This layer essentially provides freedom from compatibility problems, converting data from any format into an accessible source.

# 5 - The Session Layer:
The session layer, the fifth layer in the OSI Model provides management for connections between applications. This involves managing and terminating connections between applications. A good example of this would be a website which you Log On to. Logging into a website starts a new session. Apart from managing and terminating connections, the session layer is also responsible for the exchanges and dialog between applications from each end of the network. This involves complex coordination of network infrastructure. 

# 4 - The Transport Layer:
The transport layer, the forth layer in the OSI Model provides the transparent communication of data between end systems. The transport layer is also responsible for end-to-end error recovery and Flow Control which ensures the completion of data communication.

# 3 - The Network Layer:
The network layer, the third layer in the OSI Model provides the switching and routing within network infrastructure. This involves creating virtual circuits for the transfer of data between notes. The main functions of the Network Layer include Routing, forwarding, addressing, inter-networking, error handling, congestion control and packet sequencing.

# 2 - The Data Link Layer:
The Data Link layer, the second layer in the OSI Model is responsible for the encoding and decoding between bits and data packets. The layer manages the transmission protocol knowledge and handles errors in the physical layer, flow control systems and frame synchronization systems. The Data Link Layer is comprised of two internal layers.
## 2(a) - The Media Access Control Layer:
The Media Access Control layer controls how computers within networks gain access to data. This also includes the permissions to receive and transmit data.
## 2(b) - The Logical Link Control Layer:
The Logical Link Control Layer is responsible for the Frame Synchronization, flow control and error checking. 

# 1 - The Physical Layer:
The physical layer, the first layer in the OSI Model manages the communication of bit's throughout a network from an electrical or mechanical level. The Physical Layer provides the hardware means for sending and receiving communication from cables, network interface cards and other physical aspects of network infrastructure. Ethernet is the most well known Protocol from the Physical Layer.

# The Layers and Associated OSI & TSP/IP protocols:

**Layer**|**Name**|**OSI Protocol**|**TCP/IP Protocols**
:-----:|:-----:|:-----:|:-----:
7|Application|FTAM, X.400, X.500, DAP, ROSE, RTSE, ACSE, CMIP| BGP, DHCP, DNS, FTP, HTTP, IMAP, LDAP, MGCP, MQTT, NNTP, NTP, POP, ONC/RPC, RTP, RTSP, RIP, SIP, SMTP, SNMP, SSH, Telnet, TLS/SSL, XMPP
6|Presentation|ISO / IEC 8823, x.226, ISO / IEC 9576-1, X.236|MIME, SSL, TLS, XDR
5|Session|ISO / IEC 8327, X.225, ISO / IEC 9548-1, X.234|SOCKETS ( Session establishment in TCP, RPT, PPTP)
4|Transport|ISO / IEC 8037, TP0, TP1, TP2, TP3, TP4 (X.224), ISO / IEC 8602, X.234|TCP, UDP, SCTP, DCCP, RSVP
3|Network|ISO / IEC 8208, X.25 (PLP), ISO / IEC 8878, X.223, ISO / IEC 8473-1, CLNP X.233, ISO / IEC 10589, IS-IS|IP, Ipsec, ICMP, IGMP, OSPF, RIP
2|Data link|ISO / IEC 7666, X.25 (LAPB), Token Bus, X.222, ISO / IEC 8802-2, LLC (Type 1 & 2)|PPP, SBTV, SLIP, ARP, NDP, OSPF, MAC (Ethernet, DSL, ISDN, FDDI)
1|Physical|X.25 (X.21bis, EIA / TIA-232, EIA / TIA-449, EIA-530, G.703)| 


# Networking Notes
#### Short, subtle notes of interest within Network Infrastructure Revision.

### TTL (Time to Live):
TTL or Time To Live, is a common error typically recorded in network monitors such as Wireshark. The issue occurs when the TTL is exceeded. In short, this error occurs when too many hops to reach a destination have occured, before the TTL has been decremented to zero / 0.

### Packet Changes throughout IP Packet transfer:
When an IP Packet is transferred through a server, from a Router, all fields within the packet will remain the same apart from the TTL and the Checksum in which, the TTL will decremented to Zero while the Checksum will be recalculated.

### how does the Trace-route utility map the path from source to destination?
Typically, the TTL field is used to force an error in each node throughout it's path, these nodes being routers. 

### What is the main cause of Fragmentation within Packets?
Fragmentation of packets occur whe the length of the IP Protocol Data Unit (PDU) exceed the size of the Media Access Control (MAC) Frame.
#### How is Fragmentation Indicated?
Fragmentation flags are set to indicate that further fragments will follow and the offset field is prepared for this fragmentation.

### What is a Subnet within a Network System?
An IP network is split into two sections, the core and the organisation. An organisation is given a block of addresses for its use. Each organisation s free to manage its block in a way it chooses; it an have one internal network or split the single block into smaller subsets. 

### What is the purpose of a Subnet Mask?
#### If a Subnet has a mask of 255.255.255.192, how many hosts does it have?
The Subnet mask indicates which bits in the IP Address are used as the address of the subnet and which are the address of the host on the subnet.

Regarding 255.255.255.192, 6 bits are reserved for the subnet, giving 64 potential addresses however; The first (.0) and last (.255) are reserved as the subnet address and the broadcast address, this gives us a total of 62 hosts.
As an additional note, we're dealing with a Class B Subnet Network. 

Class B Subnet Calculations

| Mask | Binary | Subnets | Hosts per subnet |
|:-------------:|:-------------:|:-------------:|:-------------:|
| 255.255.128.0 | 10000000.00000000 | 2 | 32,766 |
| 255.255.192.0 | 11000000.00000000 | 2 | 16,382 |
| 255.255.224.0 | 11100000.00000000 | 6 | 8,190 |
| 255.255.240.0 | 11110000.00000000 | 14 | 4,094 |
| 255.255.248.0 | 11111000.00000000 | 30 | 2,046 |
| 255.255.252.0 | 11111100.00000000 | 62 | 1,022 |
| 255.255.254.0 | 11111110.00000000 | 126 | 510 |
| 255.255.255.0 | 11111111.00000000 | 254 | 254 |
| 255.255.255.128 | 11111111.10000000 | 510 | 126 |
| 255.255.255.192 | 11111111.11000000 | 1022 | 62 |
| 255.255.255.224 | 11111111.11100000 | 2,046 | 30 |
| 255.255.255.240 | 11111111.11110000 | 4,094 | 14 |
| 255.255.255.248 | 11111111.11111000 | 8,190 | 6 |
| 255.255.255.252 | 11111111.11111100 | 16,382 | 2 |

#### How to calculate?
Well, take this example, 255.255.255.192:

1. 2-2=1022 subnets:
	
	(2<sup>n</sup>where N is the number of borrowed bits.)
	
2. 2-2=62 hosts per subnet:

	((Formula: 2<sup>(32 - n)</sup> - 2) where N is the number of subnet Masks.
	
3. 256-255=1.0, 2.0, 3.0, etc. for the third octet. 256-192=64, 128, 192 for the fourth octet. For every valid subnet in the third octet, we get four subnets in the fourth octet: 0, 64, 128, and 192.

4. Broadcast for the 1.0 subnet is 1.63, since the next subnet is 1.64. Broadcast for the 1.64 subnet is 1.127, since the next subnet is 1.128. Broadcast for the 1.128 subnet is 1.191, since the next subnet is 1.192. Broadcast for the 1.192 subnet is 1.255.

 ### What is a Private Network?
 A private network is a network that is not connected to the public internet, as we remember, the Internet is an <b>Inter</b>connected <b>net</b>work of networks.
 _What strange bold marks... It's as if I'm hinting something..._

By convention, a private network is given a subnet address from one of the reserved IP ranges that are designated for private networks and will ensure that a router does not convey traffic from the private network to a public network.

### How would a Private Network Communicate with a server on a public network?

Private networks can be connected to public networks through a Network Address Translating router or NAT Router.

_Aah, so that's what NAT stands for!_
_-Pointdexter...._

The NAT router maps the internal IP address of the computer to the public address of the router, using a mapping table, so that returning packets can be delivered to the correct computer. To support multiple computers on a private network, the NAT router will map the port number from the internal computer to an arbitrary port number on the public network, maintaining the tuple in the mapping table.

### What are the three main principles of network security?

#### Encryption, Authentication & Non-Repudiation

<sup>To **repudiate** means to deny or contest something. Therefore, non-repudiation must be the ability to ensure that someone cannot deny or contest that thing. This is usually seen in electronic communications where one party cannot be confirmed as the recipient or denies seeing or signing a contract or document. Non-repudiation means putting measures in place that will prevent one party from denying they received or agreed to a transaction.</sup>

### What are the main forms of attack that can be made on the security of computer systems?
The most common forms of attack on the security of computer systems include:
* Eaves-dropping
* Replay
* Denial of Server (Distributed Denial of Service) 

and so on. 

### What is Public Key and Symmetric Key Encryption and what are the main ways in which the two differ?

#### Public Key:
Uses two keys, the private key is kept secret by the owner, and the public key is known openly. Any plaintext can be encoded by either the public or private key, but the opposite is required to decode. Encoding is computation intensive. Therefore used to encode relatively short messages.

#### Symmetric Key:
Uses same key to encode and decode. It must be kept secret by sender and receiver. Encoding is much less computation intensive than public so used for large messages.

### What are Digital Certificates?

Digital certificates are used to prove the authenticity of the party presenting the certificate. They are in the form of a statement that is authenticated by a trusted party. The authentication is normally signed by the trusted party using  their private to encode the signing and is authenticated by decoding with the public key

### What are the most important features of the Transmission Control Protocol which provide a reliable service within networks:

A reliable transport will provide the following as features:

* Error detection
	* Error correction (retransmission or forward error correction)
* Flow control
	* Guaranteed order of delivery

TCP also provides traffic shaping through congestion algorithm and window protocol to maintain full transmission rate

### Consider the problems that might arise if an application sends data at a "Full Rate" over a network without taking into account prevailing conditions.

#### 1. What problems arise if computers send data at full rate?

The network will overload and packets will be lost when buffers overflow. This will result in retransmission adding further to congestion. Packets will arrive out of order and require buffering. This can impact applications.
Applications will not be able to accept and process data at the rate they are arriving. Data may be lost by the application.

#### 2. How is the Transmission Control Protocol designed to overcome these problems?

The congestion algorithm is used to shape traffic flow to match prevailing network conditions. Retransmission will overcome lost packets
Flow control prevents overload in the application

#### How would the throughput typically vary within a network
Suitable diagrams demonstrating TCP management typically showcase a slow start up followed by half drop when packet loss detected and then linear growth back to packet loss
![Image result for typical TCP packet transfer graph](https://www.cisco.com/c/dam/en_us/about/ac123/ac147/images/ipj/ipj_9-2/92_gig_fig_02_lg.jpg)

### Multi-Media applications are known for constant transfers of data, whether in the form of imagery or audio, what would be the the most preferred TRANSPORT LAYER protocol to support such applications within networks?

##### _Pssst, The Transport layer is the forth layer on the OSI reference model_ (Check previous notes)

UDP is used to transport packets in the network however, UDP has no retransmission; this is not required in this application as arrival time and order of packets is unpredictable and may arrive too late. RTP would be used to carry the multimedia packets as payload of the UDP packets in order to carry information on order, timing and sequence. Other protocols may be used in addition to support multi-media application such as H323, SIP and RSVP.

### What are the main physical topologies employed to implement networks.

* Bus
* Star
* Point to Point
* (wireless)

### Describe the CSMA/CD medium access protocol.

CSMA/CD or Carrier Sense, multiple access, collision detection, is the main protocol used for cable bus networks.

All nodes monitor the bus for silence before attempting to access the bus (carrier sense).

When silence is detected, all nodes waiting to transmit are allowed to attempt to transmit their data (multiple access).

Transmitting nodes monitor their transmission to detect if it is corrupted because 2 or more nodes are attempting to transmit at the same time (collision detection).

Transmission of data (minimum packet length) must be longer than maximum round trip time of the network to ensure corruption can be detected.

When collision detected, sending station exerts a jamming signal, then transmission terminates.

Transmitting stations must alter the period before attempting to resend in order to resolve contention. 

This is a random selection from a number of slots. If there are further collisions then the number is increased, by a factor of 2. This is termed binary exponential back off.

### How are network nodes enabled to deliver an IP packet to the specific physical node with that IP address within the subnet.

The network node needs to resolve the IP address to the physical MAC address in order to deliver to the specific physical node. This is normally achieved through the ARP. The sending node broadcasts an ARP request within the subnet, and the node with that IP address responds. The sending node can then resolve the IP address to MAC address and sends the packet. Normally nodes will cache the address resolution for a period of time.

# Even more Networking Notes:

### What are the characteristics expected of a reliable transport layer, such as the TCP of the TCP/IP protocol suite.

* Deliver data in same order as sent
* Retransmit lost or corrupted data
* Flow control to prevent loss by application

### What is the window protocol of the TCP and how does it overcomes the limitation of round trip time to achieve full rate transmission within an extended network.

Multiple packets are transmitted and are in flight before acknowledgement is received for the first transmitted packet. The window is made large enough so that packets are transmitted continually and there is no pause to wait for an acknowledgement, and so transmission is maintained at full speed. 

### How does TCP manage its rate of transmission to ensure that a network does not become congested and bandwidth is shared fairly between users.

TCP uses the congestion algorithm with slow start -up to match transmission rate to prevailing network conditions. Slow start up sends 1, 2, 4, 8 etc packets until loss, to ramp up to transmission speed, then uses linear growth. If there is further loss, then transmission rate is halved. Suitable diagram to be added. 

### When would UDP be the protocol of choice over TCP.

UDP is used for simple applications that have a single request and response which can each be placed in a single packet. This reduces significantly the number of packets (typically 2 in place of 9).
UDP is used for real time applications, such as multi-media, in order to deliver packets timely as there is no re-transmission which could cause freeze in play out if re-transmitted packet is not received in time.

### what is a subnet in a network system.

A subnet is a single address domain, where all network nodes are addressed with the same subnet address and differentiate by their node address. This normally corresponds to a single LAN domain.

### What are the advantages of segmenting networks using a combination of routers and switches within an organisation:
* Physical extension of network – subnets located in separate locations
* Increase capacity – physical limitation of limited number of node addresses on single subnet
* Reduce load – subnet can become overloaded so distribute to multiple subnets
* Security – isolate secure systems on separate subnet
* Resilience – isolate faults (e.g. virus)

### Why would you place a Web Server on an Isolated Subnet within a Network:

Isolated Subnets can be configured with controlled access from public network but remain isolated from internal networks to prevent spread of virus or unauthorized access to internal systems

###	How are network enabled to deliver an IP packet to the specific physical node with that IP address within a subnet.

ARP is used to resolve an IP address to its MAC address. ARP broadcasts a packet on the subnet requesting the node with a specified IP address to respond the requesting node.

### What is meant by the “public” network and a private network. How are these differentiated by the IP address of the network?

The public network refers to the interconnected network of organisations that supports inter communication between all connected organisations.
A private network is an isolated network that is not connected to the public network and will use an IP address that denies routing of packets to the public network.
Three private addresses are defined, one for each class:
* 10.0.0.0
* 172.16.0.0
* 192.168.0.0 

### How is a computer configured in a private network enabled to communicate with a server in the public network by use of a NAT router. How is the concept of the private network being exploited in current networks?

The NAT router performs a translation of the source IP address from the private source address of the private network to the public address of the NAT router, and appends a source port number to ensure that the address::port is unique. The NAT router maintains a mapping table so that a returning packet can have the incoming public destination address::port replaced by the appropriate private address::port.

There is a shortage of IP V4 addresses. The private network allows the connection of many computers that can share the single IP address of the NAT router and exploit the large range of unused port addresses, and so extend the lifetime of the current addresses.

### What is meant by an A, B and C class internet address. 

The intention was to create different classes in order that an organisation could be allocated a class that would include a number of addresses appropriate to its size. A class gave many (2^24), B class (65k) and C class (256).
The address range was split using simple binary rules (exact addresses are not expected to gain marks, only the principles)

| Class | Binary| Address | Subnet Mask |
|:----------:|:----------:|:----------:|:----------:|
| A Class | 00000000 | 0.0.0.0 | 127.255.255.255 |
| B Class | 10000000 | 128.0.0.0 | 191.255.255.255 |
| C Class | 11000000 | 192.0.0.0 | 223.255.255.255 |
| D Class | 11100000 | 224.0.0.0 |

###  Let us assume a organisation is provided with a C Class internet address of 202.18.6.0/24 and decides that it will create 4 identical subnets internally.

#### What will be the subnet mask for each of the internal subnets?
* 255.255.255.192   (or /26)

#### How many hosts can be placed on each of the internal subnets? Explain your answer. 

The C Class network has 256 addresses and this split into 4 giving 64 addresses per subnet; however 2 are lost to subnet address and broadcast address, so 62 hosts.

#### If the router is allocated the first IP address on each subnet, what is the IP address of the router on each of the subnets?

* 202.18.6.1, 
* 202.18.6.65
* 202.18.6.129
* 202.18.6.193

### How might the DHCP protocol be used by network administrators to manage the IP address and configuration of network nodes that are connected to a subnet. 

DHCP protocol is used by client to request information from the DHCP server on IP address, subnet mask, default gateway, DNS server. The client sends its MAC address, and so addresses can be reserved to ensure a client is given specific IP address each time. Each client is given a lease time for the IP address which must be renewed. If not renewed the IP address can be reallocated to a new client requesting an IP address. This allows limited pool of addresses to be used by larger number of clients.

#### How does the DNS protocol supports human users to use easily remembered names for web sites.	(5 marks)

DNS is a distributed database system that manages the mapping of names to IP addresses. The naming system is hierarchical; with top level domains managed by the root DNS servers that record the location of the local DNS servers that manage the sub-level names for the domain.

When a DNS request is made, the query is passed to the specified local DNS server to resolve. If it cannot resolve it passes to specified root server(s). These pass to local DNS server. The response is returned long the chain.

### Let us assume, A small company establishes its servers within a private network and connects these to the public network through a NAT router. The NAT router obtains its public IP address from the ISP using DHCP.

#### What are the issues that exist for the company in providing public access to its server and ways in which these may be overcome. 
The use of DHCP will result in a different IP address being allocated to the public port of the NAT router. DNS can be used to map the name of the server to the changing IP address. This is referred to as Dynamic DNS.
There are the issues of configuring the NAT router to map the external ports to the internal address::port of the server and the limitation that an external port can only be mapped once and so limiting the number of distinct servers that can be configured.


