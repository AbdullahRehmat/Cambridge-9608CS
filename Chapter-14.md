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

