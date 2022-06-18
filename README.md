# Info-Security-Tenets-Terms-and-Frameworks
Various Information Security Tenets, Frameworks, Terms and Articles discussing Info Security Processes 

## Information Security (InfoSec): The Complete Guide

https://www.exabeam.com/information-security/information-security/

**This article covers the following:**

What is Information Security?

Information Security vs Cybersecurity

Information Security Goals in Organizations

Types of Information Security: Application Security, Infrastructure Security, Cloud Security, Cryptography, Incident response, Vulnerability Management, Disaster recovery

What a CISO Does

Definition and Types of Security Operations Centers (SOC)

Common Information Security Risks: Social Engineering Attacks, Advanced Persistent Threats (APT), Insider Threats, Cryptojacking, Distributed Denial of Service (DDoS)
Ransomware, & Man-in-the-Middle (MitM) Attacks

Information security technologies: Firewalls, Security Incident and Event Management (SIEM), Data Loss Prevention (DLP), Intrusion Detection System (IDS),
User Behavioral Analytics (UBA), Blockchain Cybersecurity, Endpoint Detection and Response (EDR), Cloud Security Posture Management (CSPM)

Examples of Information Security in the Real World: DLP at Berkshire Bank, SOC at Grant Thornton, Incident Response at WSU, Information security certifications
Best Practices

# E-mail Protocols and Security Landscape

https://www.techtarget.com/searchsecurity/answer/What-are-the-most-important-email-security-protocols

**The following control how email is transmitted, formatted and retrieved:**

1. Simple Mail Transfer Protocol (SMTP) specifies how messages are transmitted.
2. The Internet Message Format, or Request For Comments 5322, and Multipurpose Internet Mail Extension (MIME) specifications determine how messages are formatted.
3. Internet Message Access Protocol 4 and Post Office Protocol 3 specify how email clients retrieve messages from SMTP servers.

E-mail Security Protocols and the Role They Play in Keeping E-mail Safe:

1. SL/TLS for HTTPS: Secure Sockets Layer (SSL) was introduced in 1995. After experiencing vulnerabilities, SSLv3 was succeeded by the Transport Layer Security (TLS) protocol in 1999 and eventually deprecated in 2015. Many still refer to TLS as its predecessor, SSL. 

While SSL/TLS does not play an inherent role in email security, it is used for HTTPS, which is used for almost all email exchanges between servers and users.

HTTPS uses TLS to encrypt streams of network traffic between clients and servers. It is not invoked directly in email, but is used for web traffic and thus is used to encrypt webmail messages.

2. SMTPS: SMTP Secure (SMTPS) works like HTTPS for SMTP. It uses TLS to encrypt message exchanges between clients and servers. Encrypted TLS traffic is decrypted at its destination, however, so cleartext messages may be accessible on email servers as messages are routed unless another encryption protocol, such as STARTTLS, is in use.
3. STARTTLS: STARTTLS is a service extension for SMTP that supports opportunistic encryption between mail servers and clients. When the STARTTLS extension is in use, communicating mail systems negotiate the use of encryption and authentication algorithms to protect exchanges. All message content and message metadata can be encrypted. Once the transmissions are received, the data will be decrypted.

4. SMTP MTA-STS: The SMTP Mail Transfer Agent Strict Transport Security (MTA-STS) protocol helps secure emails by enabling SMTP servers to add encryption via TLS. It also gives enterprises a mechanism to enable servers to refuse to connect with servers that do not offer TLS connections with a trusted certificate. By requiring a trusted certificate and rejecting connections from unauthenticated servers, email providers can prevent attackers from using fraudulent domains to send phishing or spam email.

5. SPF: Sender Policy Framework (SPF) provides a protocol that enables domain owners to identify which hosts are authorized to use their domain names when sending email and defines how that authorization can be verified. It provides a way for domain owners to announce which IP addresses are authorized to send email on behalf of the domain. It also reduces the likelihood that spam or phishing emails can be sent with that domain spoofed as the source of the messages, even though SPF is usually enabled with additional email security protocols that provide stronger assurances that email originated from the proper domain.

6. DKIM: DomainKeys Identified Mail (DKIM) builds on SPF and enables the entity that owns the signing domain to link itself with a digital signature that authenticates that entity.

7. DMARC: Domain-based Message Authentication, Reporting and Conformance (DMARC) provides mechanisms for notification and mandating actions when messages fail authentication under SPF and DKIM. While SPF and DKIM can flag messages as being spoofed, DMARC enables domain owners to advertise what actions should be taken when spoofed addresses are detected and for recipients to determine the appropriate response action.

8.  S/MIME: Secure/MIME (S/MIME) is the standard that defines how to encrypt and authenticate MIME-formatted data. While S/MIME content can be encrypted, the email headers are not, so an attacker would be able to see who is sending the message and who the intended recipient is.

9.  OpenPGP: OpenPGP is a standard for encryption and authentication of data, including email messages, based on the Pretty Good Privacy (PGP) framework. OpenPGP is interoperable with S/MIME, and while data can be protected, the metadata around encrypted messages is not.

10. Digital Certificates: Digital certificates are electronic documents that prove public key ownership, verifying senders are who they claim to be. A digital certificate can also be used to sign and encrypt emails. While they are not protocols per se, there are protocols that define how digital certificates can be created and shared.

# COBIT vs. ITIL®: The Ultimate IT Governance Framework Comparison

https://www.simplilearn.com/cobit-vs-itil-article

1. IT Service Management Defined
2. What is COBIT?
3. What is ITIL?
4. What are the Differences Between ITIL and COBIT?
5. What are ITIL and COBIT’s Objectives?

What is COBIT?

First introduced in 1996, COBIT, short for Control Objectives for Information and Related Technologies, is a set of practices and guidelines to help management get the most out of IT resources. Also referred to as a framework or a methodology, COBIT bridges the gap between IT goals and business goals, providing resources to build, oversee, and improve its implementation, while reducing costs, maintaining privacy standards, and giving both structure and oversight to the IT functions within the organization.

COBIT’s Core Components Include:

1. Control objectives
2. Frameworks
3. Management guidelines
4. Maturity models
5. Process descriptions

COBIT’s framework embraces these principles:

1. Applying a single integrated framework to the organization
2. Enabling a holistic approach
3. End-to-end coverage of the enterprise
4. Meeting stakeholder needs
5. Separating governance from management

What is ITIL®?

ITIL® stands for Information Technology Infrastructure Library. It’s a framework designed to manage an organization’s IT services using a set of best practices, planning, and selection, across the entire lifecycle. ITIL® focuses on IT service management—handling issues from the perspective of the IT department. ITIL® helps businesses organize an IT team’s daily processes and routines.

ITIL® breaks down into the following five components:

1. Service strategy - Focusing on mirroring the entire IT Service Delivery model so that it perfectly matches and handles the organization’s structure and needs, while simultaneously establishing the processes necessary for monitoring and updating configuration items according to the organization’s needs and impact
2. Service Design - Designing and continuously assessing a set of IT processes and service processes that best fits the company’s needs
3. Service Transition - Defining and mitigating risk factors using proper planning and change management
4. Service Operation - Assuring daily operations by delivering recursive support tasks through resources such as a service desk or backups, to name a few
5. Continuous Service Improvement - Looking at established key performance indicators (KPIs) and their evolution, including any problems and bottlenecks, and performing the needed analysis to develop optimization proposals

# Comparing NIST & SANS Incident Response Frameworks

https://isacybersecurity.com/comparing-nist-sans-incident-frameworks/

NIST is the National Institute of Standards and Technology, a U.S. government agency that specializes in all kinds of tech. The NIST Cybersecurity Framework is one of the most popular methodologies for better understanding and managing cybersecurity risk. A component of their over-all framework is the NIST Incident Framework, which is one of the most widely-used incident response standards around the world.

The NIST Incident Framework involves four steps:

**Step 1: Preparation**  
During the preparation phase, organizations aim to limit the risk of incidents by setting up controls and taking precautionary measures based on risk assessments. Depending on the nature of the work, this phase can include anything from hardware failure and power outages to extreme situations such as data leaks (accidental or  intentional) or state-sponsored cyberattacks.

Common controls implemented during this stage include a written policy about the organization’s rules, an established response plan with details about relevant 
personnel, a communication plan, and access control strategies for physical and digital spaces.

**Step 2: Detection and Analysis**  
This step is also quite similar for both NIST and SANS frameworks. During this phase, the cyber incident management experts will take a  closer look at deviations from the norm and analyze whether they fall into the incident category or not. Information from various sources such as error messages, log   files, firewalls, and detection intrusion systems is gathered.

Pro Tip: Training employees to report deviations immediately can help you respond faster to the situation.

**Step 3: Containment, Eradication and Recovery**  
NIST frameworks combine containment, eradication, and recovery in one step, which is a step that your cyber threat intelligence team can take. This can be the longest and most complex step in the process. On the other hand, the SANS framework for each of these steps needs to be distinct, even though the gist remains the same.

The first part of this step involves containing the incident and implementing damage control. The network of infected computers is quickly isolated by switching off routers, removing network cables, and powering down systems. This must be done in an orderly fashion to minimize damage and preserve forensic data for later analysis. Sometimes during this process, a backup or forensic image of the affected systems is captured so it can be reviewed later on.

Eradicating the problem requires the removal of the issue and eventual restoration. Malware is removed if possible, otherwise systems must be wiped completely before they can be re-used. At this point, any patches or improvements to the software should also be considered to prevent re-occurrence.

The recovery phase tests and validates all affected systems before they can go back online. Clear communication and timelines for testing and implementation can streamline the recovery process and ensure fully functional systems.

**Step 4: Post-Incident Activity**  
Lastly, both frameworks require you to analyze the aftereffects and what you know of the attack. Learning from the attack and moving forward with an improvement plan is key, which is what the framework requires from you. Best practice is to carry out the post-incident review as soon as possible following the incident to ensure memories are fresh, and findings can be implemented swiftly.


**SANS Incident Response 101**  
Sysadmin, Audit, Network, and Security (SANS) is a private organization that researches and educates industries in the four key cyber disciplines. The SANS framework primarily focuses on security as opposed to NIST, which has a wider domain of operation.

The SANS framework is similar to the NIST framework, except it splits out the containment, eradication, and recovery into discrete steps. The six phases of the SANS framework are as follow:

1. Preparation
2. Identification
3. Containment
4. Eradication
5. Recovery
6. Lessons Learned

# More Frameworks, Tenets, and Terms

## The Zero Trust Model 
The concept that there should be zero trust with anything or anyone that is attempting to access the company’s network until they’re verified. In other words, never trust always verify. It is valuable because it further secures one’s network against internal and external threats by verifying anything and everything that has access to it.

Examples of some of the main principles behind Zero Trust are: Implementing access controls (like VPN, which is an information access control), MFA or multi factor authentication (which requires 2 or more methods of authentication to verify a user, 2 factor is the most common), and Least Privilege (giving users the least amount of access they need to accomplish tasks within their specific role).

## The Service Organization Control Report (SOC 2) and the Payment Card Industry Data Security Standard (PCI DSS)  

https://reciprocity.com/resources/soc-2-vs-pci-compliance-whats-the-difference/

Neither standard is required by law, but non-compliance with either one has considerable consequences. For example, if your business isn’t PCI DSS-compliant, you run the risk of having your credit card processing privileges revoked. A company without an up-to-date SOC 2 report might lose business to rivals that can demonstrate that their customer data is safe, which a SOC 2 report helps to do.

**SOC 2** reports are comprehensive reviews of your organization’s data security controls, according to standards determined by the American Institute of Certified Public Accountants (AICPA). There are several kinds of SOC reports—most notably the SOC 3, which uses the same trust services criteria as the SOC 2. The SOC 2, however, contains more sensitive data and is meant to be confidential; SOC 3 reports are designed to be certified and shared.  

**The trust services criteria of the SOC 2 are derived from five key principles:**  
**Security:** All procedures and security controls included in an organization’s defense against data breaches should be effective and tested regularly.  
**Availability:** Systems and information should be accessible to staff and clients in accordance with the company’s purpose and goals.  
**Processing Integrity:** System processing must meet the objectives of the company and user entities while remaining both accurate and efficient.  
**Confidentiality:** Any information deemed confidential should be appropriately shielded from access by unauthorized parties.  
**Privacy:** Any information that is connected to an individual’s identity should be both stored and disposed of securely. 

**What Is the PCI DSS?**  
The PCI DSS was developed by the major credit card providers to ensure that cardholder data is protected by companies that process credit card information. There are 12 primary PCI compliance requirements. Those primary requirements are further divided into 281 sub-requirements, which may or may not apply to an organization based on the volume of transactions it performs annually and how those transactions are processed. Companies must validate their compliance with PCI DSS to process transactions, and any part of their network which is found not to be PCI compliant in the event of a breach could lead to heavy monetary penalties.

The primary difference between PCI DSS and SOC 2 is that the former only applies to businesses that process payment card data; the latter applies to any company that processes or stores personal consumer information of any kind. So some overlap does exist between the two standards, but SOC 2 applies to a far larger number of organizations than PCI DSS.

Another difference is the kind of professional who is allowed to conduct each audit. SOC 2 examinations can only be conducted by CPA firms, while PCI DSS compliance is proven by either an audit from a qualified security assessor (QSA) or a self-assessment questionnaire (SAQ). PCI DSS assessments must also be accompanied by an attestation from the bank that performs the company’s financial transactions. 

Finally, SOC 2 allows much more flexibility in adhering to its trust service principles. A company striving to meet SOC 2 compliance standards can tailor its business and security strategies to meet its specific needs—for example, by choosing which of the five trust service principles to include in a SOC 2 audit. 

In contrast, the PCI DSS standard is far more prescriptive about what a business must do to secure payment card transactions. Future PCI DSS updates might offer some new flexibility, but nowhere near what the SOC 2 standard allows.

## IEC 27001 & 27002 
Essentially an overview of everything a company must do to achieve compliance.

## ISO 27001
ISO 27001 is the central framework of the ISO 27000 series which is the Standard that contains the implementation requirements for an ISMS (Information Security Management System, a series of documents relating to various parts of information security management).

## ISO 27002
ISO 27002 is a supplementary standard that focuses on the information security controls that organizations might choose to implement.

## When you should use each standard
ISO 27001 and ISO 27002 have different objectives and will be helpful in different circumstances.

If you’re starting out with the Standard or are planning your ISMS implementation framework, then ISO 27001 is ideal. 

You should refer to ISO 27002 once you’ve identified the controls that you’ll be implementing to learn more about how each one works.

## What is the General Data Protection Regulation & Consumer Privacy Act?
The California Consumer Privacy Act (CCPA) and the General Data Protection Regulation (GDPR) are laws that emerged to give individuals greater power over their personal information. 

Both regulate organizations that collect and use data in a variety of ways.

The GDPR does have implications for businesses in the United States, despite originating in Europe. 

## A brief summary of the CCPA
1. Gives California residents increased transparency and control over how businesses collect and use their data.
2. Generally applies to organizations doing business in California, and to those that handle or share the personal information of California residents

## A brief summary of the GDPR
1. To give European Union (E.U.) residents increased transparency and control over how businesses collect and use their data.
2. GDPR applies to organizations in and out of the E.U. that process the personal data of E.U. residents.

## Security Controls that need to be put in place so that General Data Protection Regulation can work for your business
The fundamental practices needed for compliance around a security and data privacy program are:

1. Identity and Access Management (IDAM or IAM), whose two key principles are, separation of duties and least privilege. They help ensure that employees have access  only to information or systems applicable to their job function.

2. A DLP (Data Loss Prevention) tool helps prevent the loss of personal data, which is critical in preventing a breach. DLP controls add a layer of protection by restricting the transmission of personal data outside the network.

3. Pseudonymization helps the organization meet its data protection obligations, particularly the principles of data minimization and storage limitation, and processing for research purposes for which ‘appropriate safeguards’ are required. It is defined within GDPR as the processing of personal data in such a way that the data can no longer be attributed to a specific data subject without the use of additional information, as long as such additional information is kept separately and subject to technical and organizational measures to ensure non-attribution to an identified or identifiable individual.

4. A mature Incident Response Plan (IRP) addresses phases such as preparation, identification, containment, eradication, recovery, and lessons learned. Under GDPR, in the event of a potential data breach that involves personal information, your organization would need to notify the Data Protection Authority without undue delay, within 72 hours if feasible, after becoming aware of the breach; and Communicate high-risk breaches to affected data subjects without undue delay.

5. Third-Party Risk Management, if an organization entrusts the processing of personal data to a processor or sub-processor, and a breach occurs, all are liable. GDPR data compliance also obligates processors to have an active role in the protection of personal data. Regardless of instructions fromthe controller, the processor of  personal data must follow GDPR and can be liable for any incidents associated with loss or unauthorized access to personal data. Sub-processors also will need to
comply with the GDPR based on each contractual relationship established between a processor and sub-processor.
 
6. Review Policies and Procedures and measure their effectiveness and maturity. (i.e., they may be outdated or just not work for your current posture and if not, draft new/revise current policies) Revision would be best, as if everyone isn’t on board because the change is too broad, and they don’t implement the processes as needed, a breach can occur. For best practices, organizational policy acknowledgment and training ensures policies are properly communicated and understood.

7. Create a plan that provides in-depth analysis of gaps in order to assess your company’s level of compliance of the information security management.

## NERC/ NERC CIP
The NERC is the federal entity responsible for the oversight of the Bulk Electric System (BES) for North America. Its jurisdiction applies to all owners, users, producers, and suppliers of the Bulk Electric Supply in eight provinces of Canada, one state in Mexico and all of the continental United States. NERC Standards carry the force of regulation and as such are mandatory for all entities to whom it applies, and they cover a wide range of categories. 

NERC Critical Infrastructure Protection (CIP) Standards are those which apply specifically to the cybersecurity aspects of the Bulk Electric System and its efficient and reliable supply. 

CIP deals with the prior planning and preparation within organizations and government agencies to deal with threats to the effective and timely functioning of national and regional critical infrastructure. 

## HIPAA - The Health Insurance Portability and Accountability Act of 1996
HIPAA is United States legislation that provides data privacy and security provisions for safeguarding medical information. The law has emerged into greater prominence in recent years with the many health data breaches caused by cyber attacks and ransomware attacks on health insurers and providers. The federal law was signed by President Bill Clinton on Aug. 21, 1996. HIPAA overrides state laws regarding the safety of medical information, unless the state law is considered more stringent than HIPAA.

It's two main purposes are: 
1. To provide continuous health insurance coverage for workers who lose or change their job and to ultimately reduce the cost of healthcare by standardizing the electronic transmission of administrative and financial transactions. 
2. Other goals include combating abuse, fraud and waste in health insurance and healthcare delivery, and improving access to long-term care services and health insurance.

## HIPAA Privacy Rule 
Officially known as the Standards for Privacy of Individually Identifiable Health Information, this rule establishes national standards to protect patient health information.

## HIPAA Security Rule
The Security Standards for the Protection of Electronic Protected Health Information (ePHI) sets standards for patient data security.

## HIPAA Enforcement Rule 
This rule establishes guidelines for investigations into HIPAA compliance violations.

## What should a risk profile include?
A risk profile should include:

1. The nature and level of the threats faced by an organization.
2. The likelihood of adverse effects occurring.
3. The level of disruption and costs associated with each type of risk.
4. The effectiveness of the controls in place to manage those risks.
