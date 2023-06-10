# Week 2
# Protect Organizational Assets

# Safeguard Information

In today's world, information is scattered across various platforms, putting organizations under immense pressure to establish robust security controls to safeguard everyone's data from theft or exposure. Security controls encompass a wide range of measures designed to mitigate specific security risks, and they can be categorized into three types: technical, operational, and managerial.

Technical controls involve the use of technologies like encryption and authentication systems to protect assets. Operational controls focus on day-to-day security maintenance, such as awareness training and incident response. Managerial controls revolve around risk reduction and include policies, standards, and procedures.

Security policies serve as guidelines for organizations, outlining the necessary controls to achieve their security goals. Information privacy plays a crucial role in these decisions, as it concerns protecting data from unauthorized access and distribution. Individuals and organizations should have the right to determine when, how, and to what extent their private information is shared.

To illustrate the importance of security controls in maintaining information privacy, consider booking a flight through a travel app. While you expect the airline company to access your personal information for reservation purposes, it's unnecessary for everyone within the company to have access to your credit card details. The principle of least privilege dictates that security controls should limit access based on the user and situation, ensuring privacy.

Furthermore, security controls should align with the principle of least privilege by differentiating between data owners and data custodians. Data owners have the authority to decide who can access, edit, use, or destroy their information, while data custodians are responsible for securely handling and storing the data, including organizations and their systems.

Implementing security controls also involves considering proper classification and handling of data, recognizing it as a valuable asset. Just like any other asset, information privacy necessitates appropriate treatment and protection.

![image](https://github.com/benichi2022/googlecybersecurityprofessionalcertificate/assets/113864743/37523057-b3bc-4ec0-b5f3-2f2f237f6660)

# Encryption Methods


The internet is a vast and open system that handles a massive amount of data. While we use it to send and store information, there are certain pieces of data that we consider private. This kind of information is referred to as personally identifiable information (PII), which includes details that can be used to identify an individual, such as their name, medical and financial records, photos, emails, or fingerprints.

Protecting the privacy of PII online is challenging, requiring appropriate security measures. One crucial security control used for safeguarding information is cryptography. Cryptography involves transforming data into an unintelligible form that unauthorized individuals cannot comprehend. It achieves this through encryption, which conceals the information, and decryption, which restores it to its original readable state.

Cryptography has a long history predating computers, and one of the earliest methods is known as Caesar's cipher. Named after Julius Caesar, a Roman general, this simple algorithm involved shifting letters in the Roman alphabet forward by a fixed number of spaces. For instance, using a shift of 3, "hello" would become "khoor." Decrypting the message requires knowing the key, which indicates the number of shifts used in the encryption process.

However, Caesar's cipher has significant flaws that limit its usage today. Firstly, it relies solely on the characters of the Roman alphabet, making it susceptible to brute force attacks, where an attacker systematically tries all possible combinations. Additionally, the cipher's vulnerability lies in its dependence on a single key, risking unauthorized access if the key is lost or stolen. Therefore, modern cryptography employs more advanced algorithms to ensure online information security.


Computers rely on various encryption algorithms to protect information online, but the security of these algorithms depends on safeguarding their keys. Public key infrastructure (PKI) is an encryption framework that ensures secure information exchange online, offering a fast, easy, and secure system.

PKI operates through a two-step process that involves encrypted information exchange using either asymmetric encryption, symmetric encryption, or a combination of both. Asymmetric encryption uses a public and private key pair. The public key allows others to send encrypted information that can only be decrypted by the recipient's private key. This two-key system enhances security but can slow down the process. On the other hand, symmetric encryption employs a single secret key for information exchange, making it faster but less secure.

PKI utilizes both asymmetric and symmetric encryption based on the priorities of speed and security. For example, mobile chat applications use asymmetric encryption initially for establishing a secure connection, and then switch to symmetric encryption for faster communication. Both encryption methods rely on trust between the sender and receiver, which is addressed in the second step of PKI using digital certificates.

Digital certificates verify the identity of a public key holder and establish trust between computers and networks. They are created by trusted certificate authorities (CAs) that verify the identity of organizations or individuals. The CA encrypts the verified data, creates a digital certificate containing the encrypted information, and adds its digital signature as proof of authenticity. Digital certificates act as online ID badges, controlling access to information.

By combining asymmetric and symmetric encryption with digital certificates, PKI provides a reliable security control for exchanging secure information between trusted sources, mitigating the trust issues associated with sharing keys.


Security professionals continually consider vulnerabilities to stay ahead of threats. In addition to encryption, another security control that addresses weaknesses in key sharing is the use of hash functions. Hash functions are one-way algorithms that produce unique hash values or digests that cannot be decrypted or reversed.

A hash value serves as an identifier for the integrity of files and applications. If even a single line of code is modified, the resulting hash value will be different from the original. This allows for the identification of tampering or unauthorized changes. Hash functions enable data integrity and non-repudiation, ensuring the accuracy and consistency of information without the ability to deny its authenticity.

Security analysts frequently use hash functions to verify file integrity. By comparing hash values of files against known malicious ones, analysts can detect potential threats. Tools like VirusTotal provide databases of hash values for online viruses, aiding in the analysis of suspicious files, domains, IPs, and URLs.

Hash functions are designed to quickly and easily compare input and output values, making them valuable for validating data integrity and non-repudiation. Their one-way nature ensures that the original data cannot be derived from the hash value, adding an extra layer of security to information systems.

# Authentication, Authorization and Accounting


Protecting data is crucial for security, and two powerful tools for achieving this are hashing and encryption. However, ensuring the safety of information goes beyond these tools. Access controls play a vital role in managing access, authorization, and accountability of data. Well-implemented access controls maintain data confidentiality, integrity, and availability, while also providing quick access to authorized users.

Access controls can be categorized into three functions: authentication, authorization, and accounting. This video focuses on the basics of authentication. Authentication systems serve the purpose of determining "who you are" when accessing information. Different organizations employ various methods to collect this information based on their security policies. Authentication can be based on three factors:

Knowledge: This factor involves something the user knows, such as a password or a security question answer.
Ownership: This factor refers to something the user possesses, like a one-time passcode (OTP) sent via text or email.
Characteristic: This factor relates to something the user is, such as biometrics like fingerprint or facial scans.
For authentication to be successful, the provided information must match the stored data. Access is granted when the credentials match, and denied when they don't.

To enhance convenience, single sign-on (SSO) technology combines multiple logins into one, eliminating the need for repetitive authentication. However, relying solely on SSO poses vulnerabilities. Therefore, organizations often use SSO in combination with multi-factor authentication (MFA). MFA requires users to verify their identity using two or more independent credentials, such as knowledge and ownership. By employing SSO and MFA together, organizations achieve convenient and secure access to company resources.


Access controls encompass both authentication and authorization, and authorization is a crucial function in determining user privileges within systems and processes. This video explores the mechanisms of authorization and its relationship with authentication.

Authorization works hand in hand with authentication technologies, as authentication validates user identity while authorization determines their allowed actions. The principle of least privilege and the separation of duties influence authorization systems. The principle of least privilege ensures that access to information is granted only for the necessary duration. The separation of duties aims to prevent misuse of the system by granting appropriate levels of authorization to users, reducing the risk of system failures and improper behavior.

Authorization applies not only to individuals but also to systems, networks, databases, and other organizational aspects. Roles play a significant role in authorization, determining the privileges granted to users or systems. Two commonly used access controls for securing data over a network are HTTP basic auth and OAuth.

HTTP basic auth is a technology used to establish a user's request to access a server by sending an identifier with each communication. However, it is vulnerable to attacks as it transmits usernames and passwords openly. Nowadays, HTTPS is preferred for secure communication over the network.

OAuth is an open-standard authorization protocol that enables designated access sharing between applications. It uses API tokens to verify access, allowing users to authorize third-party websites or services without transmitting sensitive credentials. API tokens contain encrypted information about the user's identity and permissions.

Both HTTP basic auth and OAuth align with the principles of least privilege and separation of duties. They enhance security by limiting risks associated with unauthorized access. Additionally, monitoring access is essential along with controlling it.


Accounting, in the context of access controls, refers to the practice of monitoring access logs in a system. Access logs contain valuable information such as user activity, timestamps of access, and the resources utilized.

Security analysts heavily rely on access logs to identify patterns and trends, including failed login attempts and potential security breaches by hackers. Access logs are crucial in investigating security events, often being the first step in the process. These logs compile information about user sessions, which encompass a sequence of network requests and responses associated with a specific user's access to a system.

At the start of a session, two actions occur. First, a unique session ID is created to identify the user and their device during system access. Second, session cookies are exchanged between the server and the user's device. These cookies validate the session and determine its duration, enhancing security and efficiency.

While session cookies prevent the sharing of sensitive information and protect against certain attacks, they can be vulnerable to session hijacking. Attackers can impersonate users and potentially gain unauthorized access to systems, leading to data theft or financial harm. Monitoring access logs and accounting for unusual activity is vital in detecting such incidents and ensuring the safety of information.

Accounting provides valuable insights that enhance the security of information by identifying unauthorized access and potential breaches.

# Glossary terms from week 2
Terms and definitions from Course 5, Week 2
Access controls: Security controls that manage access, authorization, and accountability of information

Algorithm: A set of rules used to solve a problem

Application programming interface (API) token: A small block of encrypted code that contains information about a user

Asymmetric encryption: The use of a public and private key pair for encryption and decryption of data   

Basic auth: The technology used to establish a user’s request to access a server

Bit: The smallest unit of data measurement on a computer

Brute force attack: The trial and error process of discovering private information

Cipher: An algorithm that encrypts information

Cryptographic key: A mechanism that decrypts ciphertext

Cryptography: The process of transforming information into a form that unintended readers can’t understand

Data custodian: Anyone or anything that’s responsible for the safe handling, transport, and storage of information

Data owner: The person that decides who can access, edit, use, or destroy their information

Digital certificate: A file that verifies the identity of a public key holder

Encryption: The process of converting data from a readable format to an encoded format

Hash collision: An instance when different inputs produce the same hash value

Hash function: An algorithm that produces a code that can’t be decrypted

Hash table: A data structure that's used to store and reference hash values

Identity and access management (IAM): A collection of processes and technologies that helps organizations manage digital identities in their environment 

Information privacy: The protection of unauthorized access and distribution of data

Loader: Malicious code that launches after a user initiates a dropper program

Multi-factor authentication (MFA): A security measure that requires a user to verify their identity in two or more ways to access a system or network

Non-repudiation: The concept that the authenticity of information can’t be denied

OAuth: An open-standard authorization protocol that shares designated access between applications

Payment Card Industry Data Security Standards (PCI DSS): Any cardholder data that an organization accepts, transmits, or stores

Personally identifiable information (PII): Any information used to infer an individual's identity

Principle of least privilege: The concept of granting only the minimal access and authorization required to complete a task or function

Protected health information (PHI): Information that relates to the past, present, or future physical or mental health or condition of an individual

Public key infrastructure (PKI): An encryption framework that secures the exchange of online information

Rainbow table: A file of pre-generated hash values and their associated plaintext

Salting: An additional safeguard that’s used to strengthen hash functions

Security assessment: A check to determine how resilient current security implementations against threats

Security audit: A review of an organization's security controls, policies, and procedures against a set of expectations

Security controls: Safeguards designed to reduce specific security risks 

Separation of duties: The principle that users should not be given levels of authorization that would allow them to misuse a system

Session: A sequence of network HTTP basic auth requests and responses associated with the same user

Session cookie: A token that websites use to validate a session and determine how long that session should last

Session hijacking: An event when attackers obtain a legitimate user’s session ID

Session ID: A unique token that identifies a user and their device while accessing a system 

Single Sign-On (SSO): A technology that combines several different logins into one

Symmetric encryption: The use of a single secret key to exchange information

User provisioning: The process of creating and maintaining a user's digital identity
