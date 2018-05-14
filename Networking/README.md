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

**Layer**|**Name**|**OSI Protocol**|**TCP/IP Protocols**
:-----:|:-----:|:-----:|:-----:
7|Application|FTAM, X.400, X.500, DAP, ROSE, RTSE, ACSE, CMIP| 
6|Presentation|ISO / IEC 8823, x.226, ISO / IEC 9576-1, X.236|MIME, SSL, TLS, XDR
5|Session|ISO / IEC 8327, X.225, ISO / IEC 9548-1, X.234|SOCKETS ( Session establishment in TCP, RPT, PPTP)
4|Transport|ISO / IEC 8037, TP0, TP1, TP2, TP3, TP4 (X.224), ISO / IEC 8602, X.234|TCP, UDP, SCTP, DCCP
3|Network|ISO / IEC 8208, X.25 (PLP), ISO / IEC 8878, X.223, ISO / IEC 8473-1, CLNP X.233, ISO / IEC 10589, IS-IS|IP, Ipsec, ICMP, IGMP, OSPF, RIP
2|Data link|ISO / IEC 7666, X.25 (LAPB), Token Bus, X.222, ISO / IEC 8802-2, LLC (Type 1 & 2)|PPP, SBTV, SLIP
1|Physical|X.25 (X.21bis, EIA / TIA-232, EIA / TIA-449, EIA-530, G.703)| 
