# Security Hardening
Security hardening is the process of strengthening a system to reduce its vulnerability and attack surface.  All the potential vulnerabilities that a threat actor could exploit are referred to as a system's attack surface. Security hardening can be conducted on any device or system that can be compromised, such as hardware, operating systems, applications, computer networks, and databases. Physical security is also a part of security hardening.
Some common types of hardening procedures include software updates, also called patches, and device application configuration changes.
Another important strategy for security hardening is to conduct regular penetration testing. A penetration test, also called a pen test, is a simulated attack that helps identify vulnerabilities in a system, network, website, application, and process. 

# OS Hardening
The operating system is the interface between computer hardware and the user. The OS is the first program loaded when a computer turns on. The OS acts as an intermediary between software applications and the computer hardware. 
Some OS hardening tasks are performed at regular intervals, like updates, backups, and keeping an up-to-date list of devices and authorized users. Other tasks are performed only once as part of preliminary safety measures. 
A patch update is a software and operating system, or OS, update that addresses security vulnerabilities within a program or product. Now we'll discuss patch updates provided to the company by the OS software vendor. With patch updates, the OS should be upgraded to its latest software version.
The newly updated OS should be added to the baseline configuration, also called the baseline image. A baseline configuration is a documented set of specifications within a system that is used as a basis for future builds, releases, and updates. 
Another hardening task performed regularly is hardware and software disposal. This ensures that all old hardware is properly wiped and disposed of. It's also a good idea to delete any unused software applications since some popular programming languages have known vulnerabilities. 
The final OS hardening technique that we'll discuss is implementing a strong password policy. Strong password policies require that passwords follow specific rules. 
Some systems also require multi-factor authentication, or MFA. MFA is a security measure which requires a user to verify their identity in two or more ways to access a system or network. 

# Network Hardening
Network hardening focuses on network-related security hardening, like port filtering, network access privileges, and encryption over networks. Some tasks that are regularly performed are firewall rules maintenance, network log analysis, patch updates, and server backups. Network log analysis is the process of examining network logs to identify events of interest. Security teams use a log analyzer tool or a security information and event management tool, also known as a SIEM, to conduct network log analysis. A SIEM tool is an application that collects and analyzes log data to monitor critical activities in an organization. It gathers security data from a network and presents that data on a single dashboard. The dashboard interface is sometimes called a single pane of glass. A SIEM helps analysts to inspect, analyze, and react to security events across the network based on their priority. Now that we've covered tasks that are performed regularly, let's examine tasks that are performed once. These tasks include port filtering on firewalls, network access privileges, and encryption for communication, among many things. Let's start with port filtering. Port filtering can be formed over the network. Port filtering is a firewall function that blocks or allows certain port numbers to limit unwanted communication. A basic principle is that the only ports that are needed are the ones that are allowed. Any port that isn't being used by the normal network operations should be disallowed. This protects against port vulnerabilities.

Security analysts also use network segmentation to create isolated subnets for different departments in an organization. For example, they might make one for the marketing department and one for the finance department. This is done so the issues in each subnet don't spread across the whole company and only specified users are given access to the part of the network that they require for their role. Network segmentation may also be used to separate different security zones. Any restricted zone on a network containing highly classified or confidential data should be separate from the rest of the network.
Encryption standards are rules or methods used to conceal outgoing data and uncover or decrypt incoming data. Data in restricted zones should have much higher encryption standards, which makes them more difficult to access.

# Cloud Hardening
a cloud network is a collection of servers or computers that stores resources and data in a remote data center that can be accessed via the internet. One distinction between cloud network hardening and traditional network hardening is the use of a server baseline image for all server instances stored in the cloud. This allows you to compare data in the cloud servers to the baseline image to make sure there haven't been any unverified changes. Similar to OS hardening, data and applications on a cloud network are kept separate depending on their service category. For example, older applications should be kept separate from newer applications, and software that deals with internal functions should be kept separate from front-end applications seen by users.

# Glossary terms from week 4
Terms and definitions from Course 3, Week 4
Baseline configuration (baseline image): A documented set of specifications within a system that is used as a basis for future builds, releases, and updates

Hardware: The physical components of a computer

Multi-factor authentication (MFA): A security measure which requires a user to verify their identity in two or more ways to access a system or network

Network log analysis: The process of examining network logs to identify events of interest 

Operating system (OS): The interface between computer hardware and the user

Patch update: A software and operating system update that addresses security vulnerabilities within a program or product

Penetration testing (pen test): A simulated attack that helps identify vulnerabilities in systems, networks, websites, applications, and processes 

Principle of least privilege: Access and authorization to information only last long enough to complete a task

Security hardening: The process of strengthening a system to reduce its vulnerabilities and attack surface

Security information and event management (SIEM): An application that collects and analyzes log data to monitors critical activities for an organization

World-writable file: A file that can be altered by anyone in the world
















