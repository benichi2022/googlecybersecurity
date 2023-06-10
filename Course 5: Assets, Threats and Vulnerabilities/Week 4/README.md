# Week 4
# Threats to Asset Security
# Social Engineering

When we hear the word "cybercriminal," the image of a hacker in a dark room often comes to mind. However, cybercriminals encompass more than just these stereotypical hackers. They employ various methods, including manipulation, to commit online crimes. Social engineering is one such technique that exploits human error to gain access to private information or valuables.

Social engineering attacks can occur both online and offline, utilizing different tactics to deceive individuals. These attacks can range from quick impersonations, such as someone posing as tech support to obtain passwords, to more elaborate schemes that span months. Attackers often target individuals with limited knowledge of security procedures, taking advantage of their vulnerabilities.

Recognizing the signs of an attack is crucial in mitigating its impact. Social engineering attacks typically follow several stages: preparation, establishing trust, persuasion, and finally, disconnection from the target. Attackers gather information about their targets, create a false sense of trust, manipulate their targets into divulging information, and then disappear to cover their tracks.

To defend against social engineering attacks, implementing managerial controls like policies, standards, and procedures is essential. Staying informed about emerging trends is also crucial, and sharing knowledge with others can be an effective defense strategy. By teaching people to recognize the signs of an attack, the spread of threats can be curtailed.

Ultimately, social engineering poses a significant threat to both individuals and organizations, and cybercriminals employ various tactics to exploit and deceive their targets. Preventive measures, awareness, and sharing knowledge are key in combating these malicious attacks.


Cybercriminals often seek to maximize damage with minimal effort, and one prevalent form of social engineering that fits this description is phishing. Phishing involves using digital communications, primarily email, to deceive individuals into revealing sensitive data or deploying malicious software. It not only impacts individuals but also poses a significant threat to organizations, as a single employee falling for a phishing attack can grant attackers access to valuable systems and sensitive information.

Phishing kits, which comprise various software tools, are commonly used by attackers to launch their campaigns. These kits contain resources designed to evade detection. The three main tools found in phishing kits are malicious attachments, fake-data collection forms, and fraudulent web links. Malicious attachments are infected files that can harm an organization's systems, while fake-data collection forms resemble legitimate surveys but ask for sensitive information not typically requested in emails. Fraudulent web links lead to malicious websites disguised as trusted brands, aimed at stealing login credentials and other personal information.

Phishing attacks are commonly conducted through malicious emails, but cybercriminals also employ other communication methods such as smishing (via text messages) and vishing (via voice calls). Preventive measures employed by organizations include anti-phishing policies, employee training, securing email inboxes with filters and blocklists, and utilizing intrusion prevention systems to detect and quarantine suspicious emails.

Phishing campaigns are widespread and pose significant risks to organizations, as a single compromised password can lead to costly data breaches. Understanding the tools and techniques used by attackers empowers individuals and organizations to recognize phishing attempts and take appropriate preventive measures.

# Malware

Both humans and computers share a vulnerability to infections, although in different ways. While humans can contract viruses causing illnesses, computers can be infected by malware, short for malicious software. Malware can spread through various means, such as infected USB drives or online transmission between computers.

Devices connected to the internet are particularly susceptible to malware infections. Once infected, malware disrupts normal device operations, enabling attackers to gain control without the user's knowledge or consent. Over time, attackers have developed different strains of malware, with five of the most common types being viruses, worms, trojans, ransomware, and spyware.

Viruses are code designed to interfere with computer operations and damage data and software. They often hide within trusted applications and require user activation to initiate infection. Worms, on the other hand, can independently duplicate and spread across systems, scanning networks for vulnerable devices without user-triggered actions.

Phishing emails and other methods serve as delivery mechanisms for viruses and worms. Being cautious about clicking links only from trusted sources helps mitigate these infections. However, trojans, named after the Greek legend of the Trojan horse, masquerade as legitimate files or programs to deceive users into installing them.

Trojans are commonly employed by attackers to gain access and install ransomware, which encrypts an organization's data and demands payment for its restoration. Ransomware attacks often make themselves known to their targets to extort money, but there's no guarantee that payment will prevent future demands.

Lastly, spyware is used to gather and sell information without consent, unlike legitimate organizations that provide opt-out options. Cybercriminals utilize spyware to steal sensitive information, such as login credentials and account details, for personal gain.

While viruses, worms, trojans, ransomware, and spyware represent prominent forms of malware, many other types exist, with new ones constantly emerging.


Malware has existed since the early days of computers, initially used for digital vandalism but now serving as a profitable tool for financial gain. Ransomware is a type of malware that attackers employ to steal money, while cryptojacking is a more recent form of malware that illegally installs software to mine cryptocurrencies.

Crypto mining is the process of obtaining new coins using computers to process encrypted code. Criminals realized the potential and began using cryptojacking malware in 2017 to gain control of personal computers for mining purposes. Over time, cryptojacking techniques have become more sophisticated, with criminals targeting vulnerable servers to spread their mining software and infect connected devices.

Detecting cryptojacking software is challenging, but security professionals have tools like intrusion detection systems (IDS) to monitor system activity and alert potential intrusions. Signs of infection include slowdown, increased CPU usage, system crashes, fast-draining batteries, and higher electricity costs.

Preventive measures against malware attacks like cryptojacking include using browser extensions to block malware, ad blockers, disabling JavaScript, and staying informed about the latest trends. Security analysts can also educate others in their organizations about malware attacks.

While cryptojacking is a growing threat, it is just one example of evolving malware. Analyzing and combating new forms of malware requires years of experience and continuous vigilance.

# Web Exploits

Malicious software, or malware, can be delivered to a target through various means, including phishing and social engineering techniques. Web-based exploits are another class of threats used to spread malware. Cybercriminals target web applications to exploit coding flaws and gain access to sensitive personal information. One common type of web-based exploit is injection attacks, where malicious code is inserted into a vulnerable application, often remaining undetected as it runs in the background.

Injection attacks take advantage of how applications handle user inputs. Web applications interact with multiple users and have various interactive objects, making it challenging for developers to sanitize all inputs effectively. Cross-site scripting (XSS) is a dangerous type of injection attack that targets websites or web applications. XSS attacks exploit languages like HTML and JavaScript to gain access to sensitive data loaded on the infected web page, including cookies, geolocation, webcams, and microphones.

There are three main types of XSS attacks: reflected, stored, and DOM-based. Reflected XSS attacks involve sending a malicious script to the server, which is then reflected back to the user's browser, executing the script and allowing the attacker to retrieve information. Stored XSS attacks involve injecting the malicious script directly on the server, targeting elements served to users, and activating the code when they visit the site. DOM-based XSS attacks occur when the malicious script is present in the web page itself, without needing server interaction, and can be seen in the URL or hidden in HTML tags.

These cross-site scripting methods are employed by hackers to steal sensitive information. Security analysts should be familiar with injection attacks, including XSS, to better understand and mitigate the risks associated with web-based exploits.


Injection attacks are a common type of web-based exploit that can target websites by manipulating the way they access information from databases. SQL (Structured Query Language) is a programming language widely used by web applications to interact with databases. Websites use menus, images, and buttons to display information to users in a user-friendly manner, triggering SQL queries in the background.

However, injection attacks, such as SQL injection, can occur when user input is not properly sanitized. For example, a login form may accept user credentials and insert them into a backend SQL statement without proper validation. Attackers can exploit this vulnerability by inserting additional SQL code, causing unexpected and potentially harmful queries to be executed on the database. This can lead to unauthorized access, data modification, and even administrative control over the database.

To defend against SQL injection, developers can implement code that sanitizes user input, searching for specific SQL characters and ensuring the input is as expected. Prepared statements are a recommended coding technique that executes SQL statements before passing them to the database, allowing for validation of the code before query execution.

Preventing SQL injection requires well-written code and collaboration between security teams and developers to identify and mitigate vulnerabilities. Injection attacks are just one example of the various web-based exploits that security teams need to address.

# Threat Modeling

Preparing for attacks is a collective responsibility of the security team, as different targets require different approaches and defenses. To anticipate and prepare for attacks, security teams employ threat modeling, a process that involves identifying assets, vulnerabilities, and exposure to threats.

Threat modeling encompasses various aspects, including entire systems, applications, and business processes, and is conducted by experienced individuals with expertise in the field. While it is considered an advanced skill, team members can still be involved in the process.

There are different threat modeling frameworks available, each suited to specific areas such as network security, information security, or application development. The general process of threat modeling consists of six steps:

Defining the scope of the model by identifying and classifying assets.
Identifying potential threat actors, both internal (such as employees) and external (like malicious hackers or competitors).
Constructing an attack tree, which maps threats to assets in a detailed manner.
Characterizing the environment by considering customer and employee interactions, as well as external partners and vendors.
Analyzing threats, evaluating existing protections, identifying gaps, and assigning risk scores.
Developing a plan to mitigate risks, including options to avoid, transfer, reduce, or accept risks.
The final step involves evaluating the findings, documenting the exercise, implementing fixes, highlighting successes, and capturing lessons learned for future threat modeling endeavors.

In the context of a fitness company preparing to launch a mobile app, the security team utilizes the PASTA (Process for Attack Simulation and Threat Analysis) threat modeling framework to ensure the protection of customer data. PASTA consists of seven stages that guide the threat modeling process.

Stage one involves defining the business and security objectives, with a focus on protecting customer data in this scenario. The team asks pertinent questions to evaluate the impact of potential threats on personally identifiable information.

Stage two entails defining the technical scope, identifying the application components that need evaluation, including network protocols, security controls, and data interactions.

Stage three involves decomposing the application by working with developers to create a data flow diagram that outlines how data flows from the user's device to the company's database and the existing controls in place.

Stage four focuses on conducting a threat analysis, where the team researches and stays updated on the latest attack techniques and vectors specific to mobile apps.

Stage five encompasses a vulnerability analysis, delving deeper into potential vulnerabilities and identifying their root causes.

Stage six involves attack modeling, where the team simulates attacks using techniques such as creating attack trees. Attack vectors like SQL injection may be identified and tested to validate threats.

Stage seven is dedicated to analyzing risk and impact, synthesizing all the gathered information to make informed risk management recommendations aligned with the business stakeholders' goals.

By following the PASTA framework, the security team can systematically evaluate threats, vulnerabilities, and risks associated with the fitness company's mobile app, thereby enabling effective protection of customer data.

![image](https://github.com/benichi2022/googlecybersecurityprofessionalcertificate/assets/113864743/8e21276d-627d-455f-8ace-112f31c544ed)

# Glossary terms from week 4
Terms and definitions from Course 5, Week 4
Angler phishing: A technique where attackers impersonate customer service representatives on social media 

Advanced persistent threat (APT): Instances when a threat actor maintains unauthorized access to a system for an extended period of time 

Adware: A type of legitimate software that is sometimes used to display digital advertisements in applications

Attack tree: A diagram that maps threats to assets

Baiting: A social engineering tactic that tempts people into compromising their security

Botnet: A collection of computers infected by malware that are under the control of a single threat actor, known as the “bot-herder"

Cross-site scripting (XSS): An injection attack that inserts code into a vulnerable website or web application

Cryptojacking: A form of malware that installs software to illegally mine cryptocurrencies 

DOM-based XSS attack: An instance when malicious script exists in the webpage a browser loads

Dropper: A program or a file used to install a rootkit on a target computer

Fileless malware: Malware that does not need to be installed by the user because it uses legitimate programs that are already installed to infect a computer

Hacker: Any person or group who uses computers to gain unauthorized access to data

Identity and access management (IAM): A collection of processes and technologies that helps organizations manage digital identities in their environment 

Injection attack: Malicious code inserted into a vulnerable application

Input validation: Programming that validates inputs from users and other programs

Intrusion detection system (IDS): An application that monitors system activity and alerts on possible intrusions

Malware: Software designed to harm devices or networks

Process of Attack Simulation and Threat Analysis (PASTA): A popular threat modeling framework that’s used across many industries

Phishing: The use of digital communications to trick people into revealing sensitive data or deploying malicious software

Phishing kit: A collection of software tools needed to launch a phishing campaign

Prepared statement: A coding technique that executes SQL statements before passing them onto the database 

Potentially unwanted application (PUA): A type of unwanted software that is bundled in with legitimate programs which might display ads, cause device slowdown, or install other software

Quid pro quo: A type of baiting used to trick someone into believing that they’ll be rewarded in return for sharing access, information, or money

Ransomware: Type of malicious attack where attackers encrypt an organization’s data and demand payment to restore access

Reflected XSS attack: An instance when malicious script is sent to a server and activated during the server’s response 

Rootkit: Malware that provides remote, administrative access to a computer

Scareware: Malware that employs tactics to frighten users into infecting their device

Smishing: The use of text messages to trick users to obtain sensitive information or to impersonate a known source

Social engineering: A manipulation technique that exploits human error to gain private information, access, or valuables

Spear phishing: A malicious email attack targeting a specific user or group of users, appearing to originate from a trusted source.

Spyware: Malware that’s used to gather and sell information without consent

SQL (Structured Query Language): A programming language used to create, interact with, and request information from a database

SQL injection: An attack that executes unexpected queries on a database

Stored XSS attack: An instance when a malicious script is injected directly on the server

Tailgating: A social engineering tactic in which unauthorized people follow an authorized person into a restricted area

Threat: Any circumstance or event that can negatively impact assets

Threat actor: Any person or group who presents a security risk

Threat modeling: The process of identifying assets, their vulnerabilities, and how each is exposed to threats

Trojan horse: Malware that looks like a legitimate file or program

Vishing: The exploitation of electronic voice communication to obtain sensitive information or to impersonate a known source

Watering hole attack: A type of attack when a threat actor compromises a website frequently visited by a specific group of users

Whaling: A category of spear phishing attempts that are aimed at high-ranking executives in an organization

Web-based exploits: Malicious code or behavior that’s used to take advantage of coding flaws in a web application

Worm: Malware that can duplicate and spread itself across systems on its own

