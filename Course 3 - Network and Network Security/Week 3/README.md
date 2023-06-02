# Secure against network intrusions
Attacks can harm an organization by leaking valuable or confidential information. They can also be damaging to an organization's reputation and impact customer retention. Mitigating attacks may also cost the organization money and time.

Denial of Service Attack
A denial of service attack is an attack that targets a network or server and floods it with network traffic. The objective of a denial of service attack, or a DoS attack, is to disrupt normal business operations by overloading an organization's network. The goal of the attack is to send so much information to a network device that it crashes or is unable to respond to legitimate users. This means that the organization won't be able to conduct their normal business operations, which can cost them money and time. A network crash can also leave them vulnerable to other security threats and attacks.

A distributed denial of service attack, or DDoS, is a kind of DoS attack that uses multiple devices or servers in different locations to flood the target network with unwanted traffic. Use of numerous devices makes it more likely that the total amount of traffic sent will overwhelm the target server. Remember, DoS stands for denial of service.

The first is called a SYN flood attack. A SYN flood attack is a type of DoS attack that simulates the TCP connection and floods the server with SYN packets. 
Let's discuss two other common DoS attacks that use another protocol called ICMP. ICMP stands for Internet Control Message Protocol. ICMP is an internet protocol used by devices to tell each other about data transmission errors across the network. 
An ICMP flood attack is a type of DoS attack performed by an attacker repeatedly sending ICMP packets to a network server.

A ping of death attack is a type of DoS attack that is caused when a hacker pings a system by sending it an oversized ICMP packet that is bigger than 64 kilobytes, the maximum size for a correctly formed ICMP packet. Pinging a vulnerable network server with an oversized ICMP packet will overload the system and cause it to crash. 

Packet sniffing is the practice of using software tools to observe data as it moves across a network.

Packet sniffing can be passive or active. Passive packet sniffing is a type of attack where data packets are read in transit. Since all the traffic on a network is visible to any host on the hub, malicious actors can view all the information going in and out of the device they are targeting. Thinking back to the example of a letter being delivered, we can compare a passive packet sniffing attack to a postal delivery person maliciously reading somebody's mail. The postal worker, or packet sniffer, has the right to deliver the mail, but not the right to read the information inside. Active packet sniffing is a type of attack where data packets are manipulated in transit. This may include injecting internet protocols to redirect the packets to an unintended port or changing the information the packet contains. 

The good news is that malicious packet sniffing can be prevented. Let's look at a few ways the network security professional can prevent these attacks. One way to protect against malicious packet sniffing is to use a VPN to encrypt and protect data as it travels across the network. If you don't remember how VPNs work, you can revisit the video about this topic in the previous section of the program. When you use a VPN, hackers might interfere with your traffic, but they won't be able to decode it to read it and read your private information. Another way to add a layer of protection against packet sniffing is to make sure that websites you have use HTTPS at the beginning of the domain address.

IP spoofing is a network attack performed when an attacker changes the source IP of a data packet to impersonate an authorized system and gain access to a network. Some common IP spoofing attacks are on-path attacks, replay attacks, and smurf attacks.

An on-path attack is an attack where the malicious actor places themselves in the middle of an authorized connection and intercepts or alters the data in transit. On-path attackers gain access to the network and put themselves between two devices, like a web browser and a web server. Then they sniff the packet information to learn the IP and MAC addresses to devices that are communicating with each other. After they have this information, they can pretend to be either of these devices.

Another type of attack is a replay attack. A replay attack is a network attack performed when a malicious actor intercepts a data packet in transit and delays it or repeats it at another time. A delayed packet can cause connection issues between target computers, or a malicious actor may take a network transmission that was sent by an authorized user and repeat it at a later time to impersonate the authorized user.

A smurf attack is a combination of a DDoS attack and an IP spoofing attack. The attacker sniffs an authorized user's IP address and floods it with packets. This overwhelms the target computer and can bring down a server or the entire network.

# Glossary terms from week 3
Terms and definitions from Course 3, Week 3
Active packet sniffing: A type of attack where data packets are manipulated in transit

Botnet: A collection of computers infected by malware that are under the control of a single threat actor, known as the “bot-herder"

Denial of service (DoS) attack: An attack that targets a network or server and floods it with network traffic

Distributed denial of service (DDoS) attack: A type of denial or service attack that uses multiple devices or servers located in different locations to flood the target network with unwanted traffic

Internet Control Message Protocol (ICMP): An internet protocol used by devices to tell each other about data transmission errors across the network

Internet Control Message Protocol (ICMP) flood: A type of DoS attack performed by an attacker repeatedly sending ICMP request packets to a network server

IP spoofing: A network attack performed when an attacker changes the source IP of a data packet to impersonate an authorized system and gain access to a network

Network Interface Card (NIC): Hardware that connects computers to a network

On-path attack: An attack where a malicious actor places themselves in the middle of an authorized connection and intercepts or alters the data in transit

Packet sniffing: The practice of capturing and inspecting data packets across a network 

Passive packet sniffing: A type of attack where a malicious actor connects to a network hub and looks at all traffic on the network

Ping of death: A type of DoS attack caused when a hacker pings a system by sending it an oversized ICMP packet that is bigger than 64KB

Replay attack: A network attack performed when a malicious actor intercepts a data packet in transit and delays it or repeats it at another time

Smurf attack: A network attack performed when an attacker sniffs an authorized user’s IP address and floods it with ICMP packets

Synchronize (SYN) flood attack: A type of DoS attack that simulates a TCP/IP connection and floods a server with SYN packets
