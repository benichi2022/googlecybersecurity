# Week 3
# Vulnerabilites in Systems
# Flaws in Systems

The process of vulnerability management is crucial for protecting assets. Every asset has numerous vulnerabilities that need to be identified and addressed proactively to ensure its safety. A vulnerability refers to a weakness that can be exploited by a threat. Recognizing that vulnerabilities can be exploited is essential in understanding the significance of this process.

To illustrate the concept, imagine being given an important document to keep safe. Locking it up in a secure location is a common protection measure, considering that documents are vulnerable to theft due to their portability. Additionally, other vulnerabilities such as susceptibility to fire or water damage may prompt the implementation of further safeguards.

Similarly, security teams aim to protect assets by assessing their vulnerabilities and potential exploits. Exploits are methods used to take advantage of vulnerabilities. By preemptively considering vulnerabilities and corresponding exploits, security teams can plan and implement appropriate defenses. For instance, an alarm system can deter burglars from exploiting the vulnerability of windows to break-ins.

Vulnerability management is a four-step process: identifying vulnerabilities, considering potential exploits, preparing defenses, and evaluating the effectiveness of these defenses. It is an ongoing cycle because new vulnerabilities constantly emerge. This is why a diverse range of perspectives within security teams is valuable, as it enhances their ability to discover exploits. However, even with large and diverse teams, it is impossible to track every vulnerability.

One particular concern is the discovery of zero-day exploits, which are previously unknown vulnerabilities. Zero-day exploits occur in real-time without any time for preparation or fixing. They pose a significant threat because they haven't been planned for in advance. These unexpected exploits can render assets even more vulnerable than before, making their identification and mitigation vital.

In summary, vulnerability management involves finding vulnerabilities and addressing their corresponding exploits. It is a regular and vital process performed by organizations to safeguard assets. The initial step of identifying vulnerabilities holds particular importance in this process.


Defense in depth is a security model that employs a layered approach to vulnerability management, significantly reducing the risk of attacks. This concept is often referred to as the castle approach due to its resemblance to the layered defenses of medieval castles.

In the Middle Ages, castles were difficult to penetrate because they featured different defenses. For instance, moats prevented large groups of attackers from reaching the castle walls, while stone walls posed a challenge for those who managed to bypass the moat. Watchtowers were yet another layer of defense, deterring attackers attempting to climb the walls. Each layer minimized the risk of attacks by identifying vulnerabilities and implementing security controls.

The defense in depth concept applies a similar principle to protect assets, especially in cybersecurity. It utilizes a five-layer design to safeguard information as it travels in and out of the model.

The first layer is the perimeter layer, which involves user authentication to filter external access. The network layer focuses on authorization and utilizes technologies such as network firewalls. The endpoint layer protects devices with technologies like anti-virus software. The application layer encompasses interfaces and employs security measures like multi-factor authentication. Finally, the data layer safeguards critical data, including personally identifiable information, with asset classification as a crucial security control.

By implementing multiple layers of defense, defense in depth ensures that even if one layer fails, others are in place to prevent or mitigate an attack. This layered approach significantly enhances security and reduces the likelihood of successful breaches.


Online public libraries exist for vulnerabilities and exposures, allowing individuals and organizations to share and document common weaknesses and mistakes that can be exploited by threats. While vulnerabilities refer to system weaknesses, exposures are mistakes that can be taken advantage of by attackers.

One prominent resource for vulnerabilities and exposures is the Common Vulnerabilities and Exposures (CVE) list. Established by MITRE Corporation in 1999, the CVE list serves as an openly accessible dictionary of known vulnerabilities and exposures. It provides a standardized way of identifying and categorizing such issues. The CVE list relies on reports from independent researchers, technology vendors, ethical hackers, and anyone who identifies a vulnerability. These reports undergo a rigorous review process by a CVE Numbering Authority (CNA) before being assigned a CVE ID.

CNAs are organizations that volunteer to analyze and distribute information on eligible CVEs. They conduct thorough testing to ensure the reported vulnerabilities meet specific criteria. These criteria include the vulnerability being independent of other issues, recognized as a security risk, supported by evidence, and only affecting one codebase.

Vulnerabilities added to the CVE list are often reviewed by other online vulnerability databases, such as the NIST National Vulnerabilities Database. These databases subject the vulnerabilities to additional tests, including the Common Vulnerability Scoring System (CVSS). CVSS assigns severity scores to vulnerabilities, helping security teams calculate their potential impact and determine the urgency of patching.

The NIST National Vulnerabilities Database provides base scores for CVEs on a scale of 0-10, indicating their severity at the time of evaluation. Scores below 4.0 are considered low risk, while scores above 9.0 are deemed critical risks requiring immediate attention.

Security teams utilize resources like the CVE list and CVSS scores as part of their vulnerability management strategy. These references aid in prioritizing security fixes and determining the urgency of addressing vulnerabilities. Libraries like the CVE list help organizations assess the level of danger a vulnerability poses to their business and decide how promptly they should address it.

# Identify System Vulnerabilities


Vulnerability assessments play a crucial role in the vulnerability management process. These assessments are internal reviews conducted by an organization's security team to identify weaknesses and flaws in their security systems. The goal is to prevent attacks, ensure regulatory compliance, and protect assets.

The vulnerability assessment process typically involves four steps. The first step is identification, where scanning tools and manual testing are employed to discover vulnerabilities. This step provides a snapshot of the current state of the security system.

After identification, the vulnerabilities are subjected to vulnerability analysis, the second step. This involves testing each vulnerability to determine its source and understand the problem at hand.

The third step is risk assessment, where vulnerabilities are assigned scores based on the potential impact if they were exploited and the likelihood of exploitation. This step helps prioritize resources for addressing vulnerabilities based on their severity score.

The fourth and final step is remediation. During this step, vulnerabilities deemed impactful to the organization are addressed. Remediation involves collaboration between the security staff and IT teams to devise the best approach, which may include implementing new security procedures, updating operating systems, or applying system patches.

Vulnerability assessments are conducted regularly due to the multitude of assets organizations need to protect. These assessments not only assist in identifying weaknesses but also aid security teams in evaluating the effectiveness of their security controls and meeting regulatory standards.



# Cyber Attacker Mindset

To effectively allocate resources and stay ahead of threats, companies need to understand their attack surface, which encompasses the potential vulnerabilities that threat actors could exploit. Analyzing the attack surface is a crucial initial step for security teams.

Both physical and digital attack surfaces need consideration in modern organizations. The physical attack surface involves people and their devices, which can be targeted from both internal and external sources. For instance, an unattended laptop in a public space can be vulnerable to external threats recording sensitive company information or internal threats posed by disgruntled employees. Security hardening is the process of reducing vulnerabilities and minimizing the attack surface through measures like obstacle implementation and access controls.

On the other hand, the digital attack surface is more challenging to harden. With the prevalence of cloud computing, information is accessed from anywhere, expanding the attack surface. Data is no longer confined to on-site servers within an organization's network but is now accessible globally. This expansion increases the pressure on organizations of all sizes to defend against threats from multiple entry points.

Understanding the attack surface helps companies prioritize their security efforts, identify potential vulnerabilities, and implement appropriate defenses. By comprehending the environment surrounding their operations and taking proactive measures to minimize the attack surface, organizations can enhance their security posture and mitigate risks.


To effectively defend against cyber attacks, organizations must not only understand the evolving digital landscape but also familiarize themselves with the types of attacks they may face. Cloud computing has expanded the digital attack surface, leading to an increase in attack vectors, which are pathways attackers use to breach security defenses.

Attack vectors can range from social media platforms to removable media like USB drives. It is a misconception that only cybercriminals exploit these vectors; even employees can unintentionally or intentionally become vectors of attack, compromising sensitive company information. Thus, attack vectors pose critical risks to asset security and require diligent effort from security professionals to counter them.

Security teams adopt an attacker mindset to tackle attack vectors effectively. They identify a target, determine how it can be accessed, evaluate exploitable attack vectors, and explore the tools and methods attackers might employ. This mindset provides valuable insights into implementing the appropriate security controls and monitoring vulnerabilities.

Educating users about security vulnerabilities, applying the principle of least privilege, employing the right security controls and tools, and building a diverse security team are common rules for defending attack vectors. User education raises awareness of new threats, least privilege limits access rights to minimize security holes, and the right security tools reduce risks associated with human error. Additionally, a diverse security team helps mitigate attack vectors and prevents future attacks.

By understanding attack vectors, organizations can develop comprehensive defense strategies, educate their users, implement effective security controls, and foster a strong security team. These efforts contribute to a robust defense against the various forms of attacks they may encounter.

# Glossary terms from week 3
Terms and definitions from Course 5, Week 3
Advanced persistent threat (APT): An instance when a threat actor maintains unauthorized access to a system for an extended period of time 

Attack surface: All the potential vulnerabilities that a threat actor could exploit

Attack tree: A diagram that maps threats to assets

Attack vector: The pathways attackers use to penetrate security defenses 

Bug bounty: Programs that encourage freelance hackers to find and report vulnerabilities

Common Vulnerabilities and Exposures (CVE®) list: An openly accessible dictionary of known vulnerabilities and exposures

Common Vulnerability Scoring System (CVSS): A measurement system that scores the severity of a vulnerability

CVE Numbering Authority (CNA): An organization that volunteers to analyze and distribute information on eligible CVEs

Defense in depth: A layered approach to vulnerability management that reduces risk

Exploit: A way of taking advantage of a vulnerability

Exposure: A mistake that can be exploited by a threat

Hacker: Any person who uses computers to gain access to computer systems, networks, or data

MITRE: A collection of non-profit research and development centers

Security hardening: The process of strengthening a system to reduce its vulnerability and attack surface

Threat actor: Any person or group who presents a security risk

Vulnerability: A weakness that can be exploited by a threat

Vulnerability assessment: The internal review process of a company’s security systems

Vulnerability management: The process of finding and patching vulnerabilities

Vulnerability scanner: Software that automatically compares existing common vulnerabilities and exposures against the technologies on the network

Zero-day: An exploit that was previously unknown
