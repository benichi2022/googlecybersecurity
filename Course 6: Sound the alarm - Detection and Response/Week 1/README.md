# Week 1
# Incident Response LifeCycle


Incident lifecycle frameworks are designed to provide structure and support for incident response operations. These frameworks help organizations establish a standardized approach to handling incidents, ensuring effective and consistent management. Various types of frameworks exist, which can be adopted and customized to suit specific organizational needs.

One such framework is the NIST CSF (National Institute of Standards and Technology Cybersecurity Framework), which comprises five core functions: identify, protect, detect, respond, and recover. This course focuses on the last three steps of the NIST CSF, namely detect, respond, and recover, which are crucial stages in incident response. As an analyst, you'll be responsible for detecting and responding to incidents, as well as implementing recovery actions.

The NIST incident response lifecycle, another framework provided by NIST, consists of several substeps dedicated to incident response. It begins with preparation, followed by detection and analysis, containment, eradication and recovery, and finally, post-incident activity. It's important to note that the incident lifecycle is not a linear process but rather a cycle, allowing steps to overlap as new discoveries are made.

Before diving into incident detection and response, it is necessary to understand what constitutes an incident. According to NIST, an incident is an occurrence that jeopardizes the confidentiality, integrity, or availability of information or information systems without lawful authority. It can also involve violations or imminent threats to security policies, procedures, or acceptable use policies.

All security incidents are events, but not all events are security incidents. Events are observable occurrences on a network, system, or device. For example, a user attempting to log into their email account but forgetting their password is an observable event. However, if a malicious actor successfully initiates a password change request and gains unauthorized access to an account, it becomes both an event and a security incident.

During incident investigations, security analysts handle and document evidence and findings, similar to detectives working a case. They gather information on the who, what, when, where, and why of the incident, which is crucial for understanding and resolving the situation. Keeping track of this information is vital for incident investigations and when writing the final report.

To facilitate documentation and easy access to incident information, analysts can utilize an incident handler's journal, which serves as a form of documentation specifically designed for incident response.

# Incident Response Operations

Successful teams, whether in sports, workplaces, or schools, leverage the diverse strengths of their members to achieve a common goal. Incident response teams are no exception. Responding effectively to security incidents requires a collaborative effort from both security and non-security professionals, each with defined roles.

Computer security incident response teams (CSIRTs) are specialized groups of security professionals trained in incident management and response. The objectives of CSIRTs include efficiently managing incidents, providing resources for response and recovery, and preventing future incidents.

CSIRTs recognize that security is a shared responsibility, necessitating cross-functional collaboration with other departments. For example, if an incident involves the breach of sensitive data, the legal team should be consulted. Regulatory compliance measures may require public disclosure of security incidents within specific timeframes, necessitating coordination with the organization's public relations team.

Within a CSIRT, there are various roles. Security analysts investigate security alerts to determine if an incident has occurred and assign criticality ratings. Less critical incidents can be remediated by analysts, while highly critical ones are escalated to the technical lead, who provides technical leadership throughout the incident's lifecycle. The incident coordinator oversees and manages the CSIRT's activities, ensuring adherence to incident response processes and regular updates to involved teams.

CSIRTs can be known by different names, such as Incident Handling Teams (IHT) or Security Incident Response Teams (SIRT), depending on the organization's preference. Some teams may have specialized focuses or be integrated with a Security Operations Center (SOC). Regardless of their titles or areas of focus, all incident response teams share the common goal of incident management and response.

When an incident occurs, it is crucial for incident response teams to be prepared to respond swiftly and effectively. Incidents such as data breaches, DDoS attacks, or ransomware can cause significant harm to organizations. Compliance regulations may also mandate timely incident reporting, making it essential for organizations to have a formal incident response plan in place.

An incident response plan is a document that outlines the procedures to be followed at each stage of incident response. These plans are tailored to meet an organization's unique requirements, considering factors such as mission, size, culture, industry, and structure. While some organizations may include their incident response plan within their broader security plan, others may maintain separate documents.

Although incident response plans can vary, they share common elements. These include incident response procedures, which provide step-by-step instructions for responding to incidents, as well as system information like network diagrams, data flow diagrams, logging, and asset inventory details. Contact lists, forms, and templates are also included in incident plans.

It is important to recognize that incident response plans are not perfect and should be subject to regular review and testing. Exercises such as tabletops or simulations help familiarize team members with the response plan and identify any gaps or areas for improvement. Furthermore, specific types of exercises may be required for regulatory compliance purposes.
