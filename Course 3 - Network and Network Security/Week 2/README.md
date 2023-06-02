Week 2
# Network Operations

Network protocols are a set of rules used by two or more devices on a network to describe the order of delivery and the structure of the data.
TCP is an internet communications protocol that allows two devices to form a connection and stream data.

TCP also verifies both devices before allowing any further communications to take place. This is often referred to as a handshake. Once communication is established using a TCP handshake, a request is made to the network.

As data packets move across the network, they move between network devices such as routers. The Address Resolution Protocol, or ARP, is used to determine the MAC address of the next router or device on the path. This ensures that the data gets to the right place. Now the communication has been established and the destination device is known, it's time to access the Yummy Recipes For Me website.
Play video starting at :1:46 and follow transcript1:46
The Hypertext Transfer Protocol Secure, or HTTPS, is a network protocol that provides a secure method of communication between client and website servers. It allows your web browser to securely send a request for a webpage to the Yummy Recipes For Me server and receive a webpage as a response.
Play video starting at :2:5 and follow transcript2:05
Next comes a protocol called the Domain Name System, or DNS, which is a network protocol that translate internet domain names into IP addresses. The DNS protocol sends the domain name and the web address to a DNS server that retrieves the IP address of the website you were trying to access, in this case, Yummy Recipes For Me. The IP address is included as a destination address for the data packets traveling to the Yummy Recipes For Me web server. So just by visiting one website, the device on your networks are using for different protocols: TCP, ARP, HTTPS, and DNS.
Play video starting at :2:43 and follow transcript2:43
These are just some of the protocols used in network communications. To help you learn more about the different protocols, we'll discuss them further in an upcoming course material.
Play video starting at :2:51 and follow transcript2:51
But how do these protocols relate to security? Well, on the Yummy Recipes For Me website example, we used HTTPS, which is a secure protocol that requests a webpage from a web server. HTTPS encrypts data using the Secure Sockets Layer and Transport Layer Security, otherwise known as SSL/TLS. This helps keep the information secure from malicious actors who want to steal valuable information.

# Wireless Network
IEEE802.11, commonly known as Wi-Fi, is a set of standards that define communications for wireless LANs. IEEE stands for the Institute of Electrical and Electronics Engineers, which is an organization that maintains Wi-Fi standards, and 802.11 is a suite of protocols used in wireless communications.

Wi-Fi protocols have adapted over the years to become more secure and reliable to provide the same level of security as a wired connection. In 2004, a security protocol called the Wi-Fi Protected Access, or WPA, was introduced. WPA is a wireless security protocol for devices to connect to the internet. Since then, WPA has evolved into newer versions, like WPA2 and WPA3, which include further security improvements, like more advanced encryption. As a security analyst, you might be responsible for making sure that the wireless connections in your organization are secure. Let's learn more about security measures.

# System Identification
A firewall is a network security device that monitors traffic to and from your network. It either allows traffic or it blocks it based on a defined set of security rules. A firewall can use port filtering, which blocks or allows certain port numbers to limit unwanted communication. 

A hardware firewall is considered the most basic way to defend against threats to a network. A hardware firewall inspects each data packet before it's allowed to enter the network. A software firewall performs the same functions as a hardware firewall, but it's not a physical device. Instead, it's a software program installed on a computer or on a server. If the software firewall is installed on a computer, it will analyze all the traffic received by that computer.

Organizations may choose to use a cloud-based firewall. Cloud service providers offer firewalls as a service, or FaaS, for organizations. Cloud-based firewalls are software firewalls hosted by a cloud service provider. Organizations can configure the firewall rules on the cloud service provider's interface, and the firewall will perform security operations on all incoming traffic before it reaches the organization’s onsite network. Cloud-based firewalls also protect any assets or processes that an organization might be using in the cloud.

All the firewalls we have discussed can be either stateful or stateless. The terms "stateful" and "stateless" refer to how the firewall operates. Stateful refers to a class of firewall that keeps track of information passing through it and proactively filters out threats. A stateful firewall analyzes network traffic for characteristics and behavior that appear suspicious and stops them from entering the network. Stateless refers to a class of firewall that operates based on predefined rules and does not keep track of information from data packets. A stateless firewall only acts according to preconfigured rules set by the firewall administrator. The rules programmed by the firewall administrator tell the device what to accept and what to reject.

A next generation firewall, or NGFW, provides even more security than a stateful firewall. Not only does an NGFW provide stateful inspection of incoming and outgoing traffic, but it also performs more in-depth security functions like deep packet inspection and intrusion protection.

# Virtual private networks (VPNs)
When you connect to the internet, your internet service provider receives your network's requests and forwards it to the correct destination server. 
A virtual private network, also known as a VPN, is a network security service that changes your public IP address and hides your virtual location so that you can keep your data private when you're using a public network like the internet. VPNs also encrypt your data as it travels across the internet to preserve confidentiality. A VPN service performs encapsulation on your data in transit. Encapsulation is a process performed by a VPN service that protects your data by wrapping sensitive data in other data packets.

VPN services encrypt your data packets and encapsulate them in other data packets that the routers can read. This allows your network requests to reach their destination, but still encrypts your personal data so it's unreadable while in transit. A VPN also uses an encrypted tunnel between your device and the VPN server. The encryption is unhackable without a cryptographic key, so no one can access your data.

# Security zones
Security zones are a segment of a network that protects the internal network from the internet. They are a part of a security technique called network segmentation that divides the network into segments. Each network segment has its own access permissions and security rules. Security zones control who can access different segments of a network. Security zones act as a barrier to internal networks, maintain privacy within corporate groups, and prevent issues from spreading to the whole network. Additionally, an organization's network can be divided into subnetworks, or subnets, to maintain privacy for each department in a organization.
An organization's network is classified into two types of security zones. First, there's the uncontrolled zone, which is any network outside of the organization's control, like the internet. Then, there's the controlled zone, which is a subnet that protects the internal network from the uncontrolled zone. There are several types of networks within the controlled zone. On the outer layer is the demilitarized zone, or DMZ, which contains public-facing services that can access the internet. This includes web servers, proxy servers that host websites for the public, and DNS servers that provide IP addresses for internet users. It also includes email and file servers that handle external communications. The DMZ acts as a network perimeter to the internal network.

Inside the internal network is another zone called the restricted zone. The restricted zone protects highly confidential information that is only accessible to employees with certain privileges.
# Proxy servers
Proxy servers are another system that helps secure networks. The definition of a proxy server is a server that fulfills the request of a client by forwarding them on to other servers. The proxy server is a dedicated server that sits between the internet and the rest of the network. When a request to connect to the network comes in from the internet, the proxy server will determine if the connection request is safe. The proxy server is a public IP address that is different from the rest of the private network. This hides the private network's IP address from malicious actors on the internet and adds a layer of security.
A proxy server uses temporary memory to store data that's regularly requested by external servers. This way, it doesn't have to fetch data from an organization's internal servers every time. This enhances security by reducing contact with the internal server.
A forward proxy server regulates and restricts a person with access to the internet. The goal is to hide a user's IP address and approve all outgoing requests. In the context of an organization, a forward proxy server receives outgoing traffic from an employee, approves it, and then forwards it on to the destination on the internet. A reverse proxy server regulates and restricts the internet access to an internal server. The goal is to accept traffic from external parties, approve it, and forward it to the internal servers.

# Glossary terms from week 2
Terms and definitions from Course 3, Week 2
Address Resolution Protocol (ARP): A network protocol used to determine the MAC address of the next router or device on the path

Cloud-based firewalls: Software firewalls that are hosted by the cloud service provider

Controlled zone: A subnet that protects the internal network from the uncontrolled zone

Domain Name System (DNS): A networking protocol that translates internet domain names into IP addresses

Encapsulation: A process performed by a VPN service that protects your data by wrapping sensitive data in other data packets

Firewall: A network security device that monitors traffic to or from your network

Forward proxy server: A server that regulates and restricts a person’s access to the internet

Hypertext Transfer Protocol (HTTP): An application layer protocol that provides a method of communication between clients and website servers

Hypertext Transfer Protocol Secure (HTTPS): A network protocol that provides a secure method of communication between clients and servers

IEEE 802.11 (Wi-Fi): A set of standards that define communication for wireless LANs

Network protocols: A set of rules used by two or more devices on a network to describe the order of delivery of data and the structure of data

Network segmentation: A security technique that divides the network into segments

Port filtering: A firewall function that blocks or allows certain port numbers to limit unwanted communication

Proxy server: A server that fulfills the requests of its clients by forwarding them to other servers

Reverse proxy server: A server that regulates and restricts the internet's access to an internal server

Secure File Transfer Protocol (SFTP): A secure protocol used to transfer files from one device to another over a network

Secure shell (SSH): A security protocol used to create a shell with a remote system 

Security zone: A segment of a company’s network that protects the internal network from the internet

Simple Network Management Protocol (SNMP): A network protocol used for monitoring and managing devices on a network

Stateful: A class of firewall that keeps track of information passing through it and proactively filters out threats 

Stateless: A class of firewall that operates based on predefined rules and does not keep track of information from data packets

Transmission Control Protocol (TCP): An internet communication protocol that allows two devices to form a connection and stream data

Uncontrolled zone: The portion of the network outside the organization

Virtual private network (VPN): A network security service that changes your public IP address and masks your virtual location so that you can keep your data private when you are using a public network like the internet

Wi-Fi Protected Access (WPA): A wireless security protocol for devices to connect to the internet









































