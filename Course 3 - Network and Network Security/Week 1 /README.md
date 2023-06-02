
![image](https://github.com/benichi2022/googlecybersecurityprofessionalcertificate/assets/113864743/f07e6dc4-a323-4526-b6c6-7fc90cff29cb)
Week 1 

# Introduction to Networks
Networks : is a group of connected devices

Devices use IP address and Mac addresses to find each other.
They are unique addresses

Devices can communicate on LAN or WAN.
LAN is a network that spans a small area like an office building, a school or a home.

WAN - is a network that spans a large geographic area like a city, state or country.

# Network Tools

* Hub - a network device that broadcasts info to every device on the network.
* Switch - a device that makes connections between specific devices on a network by sending and recieving data between them.
* Router - a device that connects multiple networks together.
* Modem - a device that connects your router to the internet and brings internet access to the LAN.
* Virtualization tools : pieces of software that perform network ops


Network components, devices, and diagrams
In this section of the course, you will learn about network architecture. 

Once you have a foundational understanding of network architecture, sometimes referred to as network design, you will learn about security vulnerabilities inherent in all networks and how malicious actors attempt to exploit them. In this reading, you will review network devices and connections and investigate a simple network diagram similar to those used every day by network security professionals. Essential tasks of a security analyst include setting up the tools, devices, and protocols used to observe and secure network traffic. 

# Devices on a network 
Network devices are the devices that maintain information and services for users of a network. These devices connect over wired and wireless connections. After establishing a connection to the network, the devices send data packets. The data packets provide information about the source and the destination of the data.

![image](https://github.com/benichi2022/googlecybersecurityprofessionalcertificate/assets/113864743/472eb147-f684-4fc7-b26c-157d726730e5)

A network diagram displaying how different devices are connected to an internal network
Devices and desktop computers 
Most internet users are familiar with everyday devices, such as personal computers, laptops, mobile phones, and tablets. Each device and desktop computer has a unique MAC address and IP address, which identify it on the network, and a network interface that sends and receives data packets. These devices can connect to the network via a hard wire or a wireless connection.

Firewalls
A firewall is a network security device that monitors traffic to or from your network. Firewalls can also restrict specific incoming and outgoing network traffic. The organization configures the security rules. Firewalls often reside between the secured and controlled internal network and the untrusted network resources outside the organization, such as the internet.

Servers 
Servers provide a service for other devices on the network. The devices that connect to a server are called clients. The following graphic outlines this model, which is called the client-server model. In this model, clients send requests to the server for information and services. The server performs the requests for the clients. Common examples include DNS servers that perform domain name lookups for internet sites, file servers that store and retrieve files from a database, and corporate mail servers that organize mail for a company. 

![image](https://github.com/benichi2022/googlecybersecurityprofessionalcertificate/assets/113864743/b86fb5d3-227c-46a3-955b-aaa018d8cc1b)

A client server model showing three client devices sending requests and receiving responses from a database server.
Hubs and switches
Hubs and switches both direct traffic on a local network. A hub is a device that provides a common point of connection for all devices directly connected to it. Hubs additionally repeat all information out to all ports. From a security perspective, this makes hubs vulnerable to eavesdropping. For this reason, hubs are not used as often on modern networks; most organizations use switches instead. 

A switch forwards packets between devices directly connected to it. It maintains a MAC address table that matches MAC addresses of devices on the network to port numbers on the switch and forwards incoming data packets according to the destination MAC address. Switches are a part of the data link layer in the TCP/IP model.

Routers
Routers sit between networks and direct traffic, based on the IP address of the destination network. In the TCP/IP model, routers are a part of the network layer. The IP address of the destination network is contained in the IP header. The router reads the header information and forwards the packet to the next router on the path to the destination. This continues until the packet reaches the destination network. Routers can also include a firewall feature that allows or blocks incoming traffic based on information in the transmission. This stops malicious traffic from entering the private network and damaging the local area network. 

Modems and wireless access points
Modems

Modems usually interface with an internet service provider (ISP). ISPs provide internet connectivity via telephone lines or coaxial cables. Modems receive transmissions from the internet and translate them into digital signals that can be understood by the devices on the network. Usually, modems connect to a router that takes the decoded transmissions and sends them on to the local network. 

Note: Enterprise networks used by large organizations to connect their users and devices often use other broadband technologies to handle high-volume traffic, instead of using a modem. 

A modem converting data from the internet, connecting to a Wi-Fi router
Wireless access point

A wireless access point sends and receives digital signals over radio waves creating a wireless network. Devices with wireless adapters connect to the access point using Wi-Fi. Wi-Fi refers to a set of standards that are used by network devices to communicate wirelessly. Wireless access points and the devices connected to them use Wi-Fi protocols to send data through radio waves where they are sent to routers and switches and directed along the path to their final destination.

A wireless access point connected to wired and wireless devices on a network
Using network diagrams as a security analyst
Network diagrams allow network administrators and security personnel to imagine the architecture and design of their organization’s private network.

Network diagrams are topographical maps that show the devices on the network and how they connect. Network diagrams use small representative graphics to portray each network device and dotted lines to show how each device connects to the other. Security analysts use network diagrams to learn about network architecture and how to design networks. 

A router connecting to two firewalls and creating two separate security zones
Key takeaways
In the client-server model, the client requests information and services from the server, and the server performs the requests for the clients. Network devices include routers, workstations, servers, hubs, switches, and modems. Security analysts use network diagrams to visualize network architecture.

![image](https://github.com/benichi2022/googlecybersecurityprofessionalcertificate/assets/113864743/7218d80f-f07f-4005-acec-033156fd17c8)

# Introduction to network communication
A data packet is a basic unit of information that travels from one device to another within a network.
A data packet is very similar to a physical letter. It contains a header that includes the internet protocol address, the IP address, and the media access control, or MAC, address of the destination device. It also includes a protocol number that tells the receiving device what to do with the information in the packet. Then there's the body of the packet, which contains the message that needs to be transmitted to the receiving device. Finally, at the end of the packet, there's a footer, similar to a signature on a letter, the footer signals to the receiving device that the packet is finished.

Bandwidth refers to the amount of data a device receives every second. You can calculate bandwidth by dividing the quantity of data by the time in seconds
Speed refers to the rate at which data packets are received or downloaded. Security personnel are interested in network bandwidth and speed because if either are irregular, it could be an indication of an attack. Packet sniffing is the practice of capturing and inspecting data packets across the network.

The TCP/IP model
First, TCP, or Transmission Control Protocol, is an internet communication protocol that allows two devices to form a connection and stream data. The protocol includes a set of instructions to organize data, so it can be sent across a network.
The IP in TCP/IP stands for Internet Protocol. IP has a set of standards used for routing and addressing data packets as they travel between devices on a network. Included in the Internet Protocol (IP) is the IP address that functions as an address for each private network.

 A port is a software-based location that organizes the sending and receiving of data between devices on a network.
Port numbers allow computers to split the network traffic and prioritize the operations they will perform with the data. Some common port numbers are: port 25, which is used for e-mail, port 443, which is used for secure internet communication, and port 20, for large file transfers.

The TCP/IP model is a framework that is used to visualize how data is organized and transmitted across the network. The TCP/IP model has four layers. The four layers are: the network access layer, the internet layer, the transport layer, and the application layer.

![image](https://github.com/benichi2022/googlecybersecurityprofessionalcertificate/assets/113864743/20d91453-3b62-4935-b2e8-1c49d35bdaeb)

# TCP/IP Model vs OSI Model
![image](https://github.com/benichi2022/googlecybersecurityprofessionalcertificate/assets/113864743/f0f4dac9-4840-413a-9ff7-a0518370ca54)

# IP Address
An internet protocol address, or IP address, is a unique string of characters that identifies a location of a device on the internet. Each device on the internet has a unique IP address, just like every house on a street has its own mailing address.
There are two types of IP addresses: IP version 4, or IPv4, and IP version 6, or IPv6. Let's look at examples of an IPv4 address.
Play video starting at ::37 and follow transcript0:37
IPv4 addresses are written as four, 1, 2, or 3-digit numbers separated by a decimal point. In the early days of the internet, IP addresses were all IPV4. But as the use of the internet grew, all the IPv4 addresses started to get used up, so IPv6 was developed.

Another kind of address used in network communications is called a MAC address. A MAC address is a unique alphanumeric identifier that is assigned to each physical device on a network. 

# Glossary terms from week 1
Terms and definitions from Course 3, Week 1
Bandwidth: The maximum data transmission capacity over a network, measured by bits per second

Cloud computing: The practice of using remote servers, application, and network services that are hosted on the internet instead of on local physical devices

Cloud network: A collection of servers or computers that stores resources and data in remote data centers that can be accessed via the internet

Data packet: A basic unit of information that travels from one device to another within a network

Hub: A network device that broadcasts information to every device on the network

Internet Protocol (IP): A set of standards used for routing and addressing data packets as they travel between devices on a network

Internet Protocol (IP) address: A unique string of characters that identifies the location of a device on the internet

Local Area Network (LAN): A network that spans small areas like an office building, a school, or a home

Media Access Control (MAC) address: A unique alphanumeric identifier that is assigned to each physical device on a network

Modem: A device that connects your router to the internet and brings internet access to the LAN

Network: A group of connected devices

Open systems interconnection (OSI) model: A standardized concept that describes the seven layers computers use to communicate and send data over the network

Packet sniffing: The practice of capturing and inspecting data packets across a network

Port: A software-based location that organizes the sending and receiving of data between devices on a network

Router: A network device that connects multiple networks together

Speed: The rate at which a device sends and receives data, measured by bits per second

Subnetting: The subdivision of a network into logical groups called subnets

Switch: A device that makes connections between specific devices on a network by sending and receiving data between them

TCP/IP model: A framework used to visualize how data is organized and transmitted across a network

Transmission Control Protocol (TCP): An internet communication protocol that allows two devices to form a connection and stream data

User Datagram Protocol (UDP): A connectionless protocol that does not establish a connection between devices before transmissions

Wide Area Network (WAN): A network that spans a large geographic area like a city, state, or country













