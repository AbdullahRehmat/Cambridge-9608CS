# Communication & Internet Technologies

[toc]

## 14.01 Protocols

### Communication between Computers

- Protocol = A set of rules about the form of messages exchanged between computers



### TCP/IP Stack

![https://www.technologyuk.net/computing/computer-networks/internet/images/tcp_ip_layers.gif](https://www.technologyuk.net/computing/computer-networks/internet/images/tcp_ip_layers.gif)

- Nature of communications across the internet required the the two end-points or hosts use the TCP Protocol

- Each layer of the stack has its own role in ensuring successful communication

  

- **Application Layer**

  - Packages Core Data to be transmitted
  - Each application will have its own "application package" protocol

- **Transport Layer**
  - TCP Layer
  - Responsible for setting up bi-directional communication between hosts and maintaining connection
  - Responsible for detecting errors, unsent packages, and instigating their re-transmission
  - Responsible for organising data packets into correct format for recipient
  - Each process is associated with a Port Number
- **IP Address**
  - Client & Server are identified via their IP Addresses
  - IP Address + Port = Socket
- **Network Layer**
  - IP Packet consists of a Header & Data Section
  - Header Contains
    - Version - If IPv4 used version will be 4
    - Source IP Address
    - Destination IP Address
    - Time to Live value
    - Checksum
    - Total Packet Length - Data Section
- **Link Layer**
  - Receives packets from network layer & adds hardware address for a LAN using a MAC Address
  - Using Ethernet, final packaging of packet for sending across an Ethernet cable  is called an Ethernet Frame



### BitTorrent Protocol

- Peer to Peer Network Communications Protocol
- Used by 50% of all internet traffic
- Allows user to join swarm of hosts
- Seed = User who has torrent file open in client
- Tracker Computer = Assists in communication between peers
- Swarm = Group of Hosts



### Other Protocols

- POP3 - Email Receiving
- SMTP - Email Sending
- FTP - File Transfer
- HTTP - Web Browser

- All use Client-Server Model
- Client application must know of existence of server address
- Server continuously listening for requests
- Client + Server establish communication vs Sockets



- HTTP Protocol
  - Application Level Protocol
  - Uses GET/POST Requests
  - Sequence
    - URL Entered into Address Bar
    - Socket opened on Client and connection made to Server on Port 80
    -  Text String sent to Server: GET/POST
    - Server responds with Text-Stream which is displayed and rendered by brower
- FTP
  - File Transfer Protocol
  - Allows for the updating of sites and downloading of files
- POP3 + SMTP
  - Post Office Version 3
  - Simple Mail Transfer Protocol



## 14.02 Circuit & Packet Switching + Routers

### Circuit Switching

- Dedicated circuit established between two network nodes to allow communications
- Earliest example is Telephone network switching



### Packet Switching

- Data divided in blocks called packets or data-grams
- Packets/Data-grams are transported through network independently of each other
- May take different routes



### Routers

- Hardware device 
- Receives packets from switched-network and routes each packet to destination address
- Key component of DNS and WWW
- Can be used to monitor and route LAN Packets



## 14.03 Local Area Network

- Topology = Physical layout of cabling & connection of nodes
- Bus Topology = Single cable segment with several connected nodes
- Star Topology = Separate communications link from each computer to a centralised computer



### Bus Topology

![What is Bus Topology?](https://www.computerhope.com/jargon/b/bustopol.gif)



### Network Interface Card

- NIC



### Ethernet

- Most widely used Bus Topology networking standard for the physical layer
- Electrical signal broadcast along cable and received by destination device



### CSMA/CD Policy

- Ethernet media access control policy to avoid collisions

  ![CSMA/CD | What is CSMA with collision detection? - IONOS](https://www.ionos.co.uk/digitalguide/fileadmin/DigitalGuide/Screenshots_2018/EN-CSMA-CD-schema.png)



### Collisions

- Detected by voltage change at node



### Hubs

- Shares bandwidth amongst all transmitting nodes



### Switched Ethernet 

- Full Duplex Connection 
- Eliminates issue of collisions
- Frames are forwarded based on MAC Addresses



### IP Addresses & Networks

- TCP/IP Protocol
- All IPv4 Addresses are stored as 32 bits
- Classes A B C | Reserved for Private Network use



### Public & Private IP Addresses

- Groups starting with `10.`,  `172.`  &  `192.68.` reserved for private use
- These groups are ignored by all public routers
- Several devices communicating across a LAN using private IP's will communicate accross internet via single public address via NAT



### Subnet Masks

<img src="https://i.ytimg.com/vi/sCvQL7Ds8F4/maxresdefault.jpg" alt="Subnetting #1 - Subnet Masking - YouTube" style="zoom: 50%;" />



### Star Network Topology

![Star network - Wikipedia](https://upload.wikimedia.org/wikipedia/commons/thumb/8/84/Star_Topology.png/220px-Star_Topology.png)

- Separate communications link for every node to centralised node
- If one link fails then all other nodes are still able to communicate



### Wireless Network

- IEEE 802.11
- WiFi Networks
- 3G, 4G 
- Wireless Access Points
  - Use WEP or WPA for security
  - Radio link between devices



### Routers

- Used to split networks into segments
- Maintains routing table showing which MAC addresses belong to which cable segment



### Server

- File Server
- Domain Control Authentication Server
- Multiple Servers can be run on same hardware









































