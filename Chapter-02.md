# Chapter 02

[toc]

## 2.01: Networks

### Client Server Model

- Client Computer will access services provided over network by a server

  - Files Server

    - All software and files stored on server

  - Domain Control Server

    - Manages User ID's and Accounts

  - Email Server

    - Used for the sending, recieving, and storage of emails

  - Print Server

    - Manages print jobs from client network

  - Database Server

    - Manages a Database system like SQL

  - Web Server

    - Manages web-pages

      

- Client computer makes a request to appropriate server

- Processing of request is carried out on server

- Server packages results to be displayed by software on client

  

### The Internet

- Internet is an Open Stack
- Access is provided by an ISP
- TCP / IP protocol used where devices are identified via an IP Address



### The World Wide Web

- Concists of Webpages made available from web-servers
- Invented in 1989 by Tim Berners-Lee
- Utilises HTML, URI, and HTTP / HTTPS



### Hardware: Networks

- A LAN is a group of computers that can communicate accross a network
- Network users use the Internet to access the World-Wide-Web



### Hardware: Routers

- Used on a Packet-Switched Network
- Data is organised into packets for sending betweend devices
- TCP / IP Protocol 
- Route determined by packet's destination address



### Hardware: Gateways

- Hardware that allows two networks to communicate
- Can be a hardware device or software solution
- Gateway may have Firewall capabilities



### Communication Systems: PSTN

- Public Switched Telephone Network
- Creates direct line between two end points



### Communication Systems: Dedicated Lines

- Used by companies
- Links corporate offices over the Internet
- Consistent data transfer rates
- High + Consistent Bandwidth
- Can carry phone calls and videos transmission without degredation



### Communication Systems: Cell Phone Networks

- Land mass divided into cells
- Each cell served by transceiver or base station
- Cells are Hexagonal in shape and uses a unique frequency
- Common useage is Mobile Phone calls
- Uses Radio waves



### Communication Media: Copper Cable

- Twisted Pair
  - Twisted to cancel out EM interference 
  - Cat-5E - Maximum distance of 500 meters
  - Suffers from signal loss over distance
- Coaxial Cable
  - Single strand of insulated wire 
  - Available in a number of specifications
  - Most widely used Bus Networking standard for the physical layer is Ethernet  
  - Uses include
    - Connecting TV or Radio to antenna
    - Computer Network Connections
    - Cable TV Connections



### Communication Media: Fiber-optic Cable

- Up to 24 glass strands in single cable
- Signal is pulses of light
- Data is free of interference and less susceptible to unathorised access
- Advantages over copper
  - Signal free from interference
  - Signal is not affected by cable length
  - Cable does not suffer from corrosion
- Uses Include
  - Telephone communications
  - Internet Communications
  - Networking



### Telecommunications & EM Spectrum: Radio Waves

- Largest Wavelength
- Includes AM and FM Radio
- Used for
  - Domestic antennae recieving TV signal from broadcaster mast
  - Sending and recieving mobile phone communications



### Telecommunications & EM Spectrum: Microwaves

- Wavelengths measured in centimeters
- Can penetrate light rain, snow, clouds, and smoke
- Used by satellites



### Telecommunications & EM Spectrum: Satellite Communication

- Applications include

  - Radio and TV broadcasting

  - Photography of the earth

  - Satellite based internet

  - Satellite Phones

  - Military Communications

    

### Telecommunications & EM Spectrum: Wireless

- IEEE.802.11
- Uses include
  - LAN communication
  - Smartphone and other devices



### Bit Streaming: Real Time Bit Streaming

- Example
  - Allows users to stream films from BBC IPlayer over 4G



### Bit Streaming: On Demand Bit Streaming

- Catch Up services like BBC IPlayer or Sky On-Demand



### Bit Streaming: Issues 

- Lagging due to lack of free buffer space
- Issues caused by lack of bandwidth
- Issues caused by client-side software processing



## 2.02: IP Addressing

- Most internet traffic uses IPv4

- Networks are joined into  a network of networks using TCP/IP

- IPv4 uses 32 bits for and IP Address, expressed as four numbers between 0-255, separated by commas

- Original Addressing

  - Used first byte for Networking ID
  - Proved inadequate and so a system of classes was defined
    - A B C D E
    - Each use different bit lengths for network identification
    - Class C may not use 0 or 255 as host numbers

- Internet traffic has no dedicated path

- Individual data packets may take different routes over separate networks to reach final destination

- Data is placed into packets with a destination and source address

- An IP address is usually written in Denary - 192.168.0.1

  - This is called dotted decimal notation
  - Can also be written as dotted hexadecimal or dotted binary

  

### IPV6

- In 2011 IPv4 was fully allocated

- New standard IPv6 - created in 2006 - increases address length to 128 bits

  

### Dynamic Name Service

- Known as URI
- Looks up IP Address from URL
- Once IP Address is known **routers** send packets to receiving device
- Root Servers store complete database of internet domain 
  - 13 Root Servers named A-M
- Lower level DNS Servers are owned by companies like Google or ISP's
- Usage
  - Client web browser requests resource
  - DNS Resolver contacts DNS Server to determine server's IP
  - If DNS Server cannot contain the mapping it forwards request to DNS Server higher in the hierarchy
  - This continues until request is resolved
- Three ranges of Private IP
  - 10.0.0.0/8
  - 172.16.0.0/16   to 172.31.0.0/16
  - 192.168.0.0/24 to 192.168.255.0/24



## 2.03: Client Side & Server Side Scripting

- Server used HTTP / HTTPS 
  - Recieve requests from client computers
  - Deal with each request
  - Send response to client



### Requesting Data from DB Server

- Client creates Query
- Client requests SQL Query
- Query is processed by DBMS Software
- Query Results are sent back to client



### Requesting Web Pages from Web Server

- Client browser requests page via URI
- DNS directs request to appropriate Domain
- Server retrieves Page
- Server send page content to Client
- Client browser renders and displays Page



### Client Side Scripting

- Dynamic content is processed when web page is received by client's browser.
- Popular languages include JavaScript and VBScript
- Server assumes Client Side Browser is configured to support this
- All Programming Languages are compiled or interpreted
- JavaScript
  - Interacting with User
  - Accepting User's Data input
  - Validating Data Input
  - Manipulating Images



### Server Side Scripting

- Browser requests Page
- Web Server aware that Page contains code
- Web Server processes code
- Web Server renders page content
- Web Server delivers page as HTML + Text
- Client displays image







