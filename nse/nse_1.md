# Fortinet Network Security Expert(NSE) 1

## Module 1: Introduction
- Bad Actors = Attackers (Methods, Knowledge, Motive)
- Explorer, Hacktivist, Cyber Teririst, Cyber Criminals, Cyber Warrior
- White, grey, black, and blue hat

## Module 2: The Threat Landscape
- Bad Actors --> Threat vectors --> Vulnerability, Mechanisms, and Pathways
- Attack paths
- Cybersecurity Threats --> Unauthorised Access, Social Engineering, Malware, System Vulnerabilities
- Threat Intelligence --> Situation based evidences --> Relevant, Actionable, Contextual, Implication --> On existing and coming threats on organisational assets --> Public and Private
- CVSS --> Common Vulnerability Score System
- Common format for Threat Intelligence --> TAXII and STIX
- Understanding cyberthreats on organisation --> Gather public and private threat intelligence --> Process the information --> analyse IOCs --> Disseminate the information --> apply the strategies made on the basis of information
- Cyberattack framework --> Access the Situation -> find the problem -> analyse the impact -> develop and implement strategies --> Cyber Kill Chain by Lockheed Martin --> Reconnaissance -> Weaponisation -> Delivery -> Exploitation -> Installation -> Command and Control -> Exfiltration
- Outbreak Alert --> Keep current with vulnerabilities -> Consult online and offline cybersecurity consultant --> Includes Vulnerability, Technologies affected, timeline, solution, and research done on it.

## Module 3: Social Engineering
- Way an orchestrator will try to make other people do for his own good --> Consist Emotion of the human being in it
- Phishing --> Whale and Spear Phishing --> Smishing and Vishing
- Social Engineering in which people goes to attacker instead attack go to them --> Watering hole, Honey Pot Trap, Tailgating (In this person should need to know that he is helping you), and Scareware
- Quid pro quo, Pretexting, and Baiting
- Insider Threats --> Malicious -> Mole, Lone Wolf, Collaborator --> Negligent -> Pawn, Goof
- Cyber Fraud > Cyber Scams
- Copycat government sites, Holiday Fraud, Romance site Fraud, Mandate Fraud, and Pharming 
- Online Influence --> Campaign to promote something bad or bad rumours --> Creating a Fake ID -> Creating Content -> Posting Content -> Real people watching it and sharing it -> Media will take the story

## Module 4: Malware
- Malware --> Virus -> Triggered, Attached to application, and Spreads
- Virus --> Resident, Non-Resident, Multipartile, Direct Action, Browser Hijacking, Overwrite, Web Scripting Virus, Network virus, Boot Loader virus, File Infector
- Malware --> Worms, Rootkit, DLL Injection, Keylogger, PUB, Spyware, Adware, Dialler, Ransomeware, Adversel AI, Trojan Horse (Dropper, Downloader), Bootware, Cryptojacking
- Attack Surface --> Dropper, Downloader, Shellcode, Code Injection

## Module 5: Cryptography and the Public Key Infrastructure
- Digital Key: alphanumeric key used in cryptography
- Large key (1024 bit or larger) --> used to encrypt short messages
- Small key (128 or 256 bit) --> used to encrypt long messages
- Key Strength --> Complexity + Length
- Key Stretching --> Password -> hashing multiple times -> Add Salt -> hash one more time -> result
- Digital Signature --> Document -> hashed -> Asymmetric encryption -> Digital Signature attached to document --> Receiver end -> Document hashed -> new hash -> decrypt the digital signature then match the new hash with decrypted message(hash)
- Public Key Infrastructure(PKI) --> Policies, Procedures, Hardware, and Software --> needed to create, store, use, manage, and revoke --> Digital Certificate --> Consist of CA, RA, Directory Server, and End Entity
- CA(Certification Authority) --> Issues digital certificate to End Entity and provide Trust
- Hierarchical architecture and Lateral Architecture --> Above CA sign the digital certificate using their private key to build trust
- Sender either sends its digital certificate with message or receiver could download it from directory server directly.
- RA(Registration Authority) --> manual or automatic --> Receives Request for digital certificate from end entity and then authenticate it and send the request to CA
- End Entity manually or automatic generate key pairs for digital certificate to send to CA
- Quantum Computers --> Decrease their Strength --> Hash and Symmetric cryptography --> Both could be counter by increasing the size
- Quantum Cryptography --> Quantum key distribution --> using quantum principles along with quantum computers to create a cryptography which is unbreakable in theory.
- Post Quantum Cryptography --> Lattic-Based, Hash-Based, Code-based, and Multivariant-based
- Nist recognised cryptography to prevent quantum break --> ML-key distribution, FN-DSA, ML-DSA, SLH-DSA

## Module 6: Secure Network (22 November 2026)
- Secure Perimeter --> Create Trust Boundary between trusted network and untrusted
- Data Link Layer --> using ACL(Access Control List), MAC(Media Access Control) issued by NIC to every device to filter the trusted devices.
- Transport Layer --> Stateless (5 tuple), Statefull(5 tuple and Continuous Connection) --> NAT (Network Address Translation) hides the internal devices from outside.
- Application Layer --> Proxy Filtering -> Creating two different session token to keep the internal devices hidden --> ALG (Application Layer Gateway) --> Scans the internal of traffics to filter and support protocols more properly
- Secure Perimeter Limitations --> BYOD, IoT, and cloud makes work of Security professionals harder to configure and manage
- Zero Trust Architecture --> Never Trust, Always Verify, Least Privilege, and Assume the breach is already happened
- Never Trust, Always Verifies --> Identification -> Geographical, Contextual, Security Procedure, Date and time
- Least Privilege --> PAM (Privileged Access Management) -> to manage high privilege resources --> Define the main assets and protect them --> Implement Kipling Method
- Assume Breach is Happened --> Be ready for worst case scenario and Micro segmentation
- Role-Based Access Control, End Agents, Network Access Control, Zero Trust Network Architecture
- Benefits of Zero Trust --> Least Privilege -> Micro Segmentation -> Never Trust
- Centralised Security System Management --> Collects all the information from other devices at one single point through API or SNMP (simple network management protocol) --> Data Fabric Architecture -> like a fabric knits each and every device wherever it is connected to a single server creating centralised environment
- Benefits --> Provide high level view and broader visibility -> Device Integration -> Reduce Manual/Repetitive Tasks -> Easier Maintenance -> Easier Audit Compliance
- Network Segmentation --> Creating Segmentation within the network in different different parts according to the needs --> Demilitarised zone -> Zone which is used to connect with the external network -> Consist Micro Segmentation in each component in it -> North-South Traffic is external to internal and vice versa -> East-West Traffic is within the demilitarised zone between other components
- Data Link Layer -- physical segmentation -> use of hardware to perform --> Logical Segmentation -> No need of extra hardware -> Virtual LAN connect small small components within the network creating segmentation of its own
- Software Defining - WAN --> Create a encrypted tunnel over an underlay physical network infrastructure to let them connect to the internet
- Jump Box --> Device help components or devices to talk or connect within the network -> High performance -> Low authorisation -> maintains logs
- Bastion Device --> Created to connect with external devices -> Made to withstand attacks
- Benefits of Network segmentation --> Reduction in network Congestion and broadcasting -> Protect Vulnerable Devices -> Reduce the implementation of Complines -> Easier Network management configuration -> Limiting the attacks within the segments
- Firewall --> Stateless Firewall --> Stateful Firewall --> Third Generation Firewall --> NGFW (Next Generation Firewall)
- Sateless Firewall --> Filter out 5 tuples -> Use configuration in which order matters -> At last their is either implicit or explicit ->  Need extra configuration for return traffic
- Statefull Firewall --> 5 tuples with Continuous Connection monitoring
- Third Generation Firewall --> use Application Layer Gateway to properly monitor inside of packets as well
- NGFW --> Security, Reliable, and Network Performance --> Packet Filter -> DPI (Deep Packet Inspection) -> Sandbox --> If malicious activity found then quarantined
- Can Control application by classification or user --> Adapts various Segmentation --> Moved Reactive to Proactive using AI
- Secure Switching --> CAM (Content Addressable Memory) store Port, VLAN, and MAC -> Dynamic Memory Allocation
- Common Threats --> Broadcast Frame, Unicast Frame(with no address found), Multicast Frame(with no address found) -> When no address is found on CAM table it broadcast the whole frame --> if attacker put this broadcast in loop then it will lead to collisions of packet or depleting resources --> Limiting the amount of packet per port by each MAC
- MAC Flooding Attack --> Spoof the MAC address and fill the CAM table with false data --> will lead to broadcast message every time as CAM table do not know where to send the data as it is filled with wrong data --> use static MAC or Sticky MAC
- Rate Limit of number of frames allowed from a port by a MAC in a period of time -> Implement Static and Sticky MAC -> Implement Port Authentication IEEE 802.1x -> Protect Switches physically -> Separate the Switches
- Secure Protocols --> MIME (Multipurpose Internet Mail Extension) -> Secure MIME (digital Signature) --> HTTP -> HTTPs (TLS) --> Telnet -> SSH --> L2PT -> IPsec
- SSH --> Client to server request to connect -> Server consist clients public key so server sends a string encrypted using client public key -> client decrypt the message and sends it -> Authentic
- Sandbox --> A virtual environment where everything works as original system but in locked room to test and execute malicious files -> use to detect zero days
- First Generation Sandbox --> Does not communicate much and harder to share information
- Second Generation Sandbox --> Start communication with each other -> Can connect other security tools -> directly sends the threat intelligence to cloud threat intelligence server
- third Generation Sandbox --> Stops and analyse AI driven Attacks
- Network Threat --> Spoofing -> Replay Attack -> DoS -> Transitive Attacks -> Hijacking
- DoS --> Flooding --> Smurf Attack (Spoofing victim address to send request to other servers to get tons of request at a same time), Fraggle Attack (UDP), SYN Attack (half TCP Connection), Christmas Tree Attack (TCP)
- Dos --> Ping of Dead -> Ping is used to measure and keeping connection between client and server -> if big data is fragmented which is larger than the memory size of protocol and sent then at the reassembly of receiver end it will put buffer overflow -> regular ping size < 100 bytes -> ping of death creates > 65,535 bytes
- Dos --> Teardrop Attack -> Sending fragmented packets overlapping with oversized payloads which will crash the target at reassembling end
- DoS --> Permanent DoS -> Use Vulnerability to make the system unavailable
- DoS --> Fork Attack -> system call -> UNIX System -> consumes the resources from baby to parents calls
- Close unnecessarily opened ports and patch vulnerabilities
- OT (Operational Technology) Security --> Hardware and software --> Monitor and Control --> Physical Devices, process and infrastructure
- Operational Systems --> Protected by Operational Security from Cyber Threats --> Ensure working of operational systems continuously and reliably
- IT works on information process, management and working -> OT manages running of devices, physical process, and infrastructure --> IT focus on confidentiality and integrity -> OT focus on reliability, Availability, Stability, and safety --> Business controls and communication -> require real time traffic
- OT Components --> Industrial Control Systems -> DSC, PLC, and SCADA --> Industrial IoT --> Human Machine Interface --> Remote Terminal Unit (works with SCADA)
- Common Threats to OT --> Malware --> Insider Threat --> Ransomeware --> APT --> Supply Chain Attacks --> Unauthorised Access
- OT Security unique --> Legacy Systems --> Zero Downtime --> Low Visibility --> Unencrypted Protocols --> Flat Network Architecture
- Benefits of OT Security --> Continuous operations --> Control of System --> Continuous Monitoring and visibility --> Regulatory Compliance --> Equipment and Personal Safety
- Best Practices -> Governance & Risk Management --> Monitoring and Detection --> Network and Access Control --> Incident Response and Recovery --> Workforce Preparedness

## Module 7: Authentication and Access Control (23 November 2026)
- Authentication --> Identification and Verification
- Knowledge, Possession, Inherence, Behaviour
- SSO (Single Sign On) --> Sign in only one time then that authentication token will be distributed to every other application connected to it
- Same Sign On --> Every application will consist same credentials which is saved on a directory server --> every application will validate the same credential from the server --> Still need to sign in at each application
- User -> go to Service Provider -> Identity Provider -> authenticate user with session token -> SP
- SSO Benefits --> Only need to manage one database of credentials --> User only need to remember one credentials --> Reduction of Compliance
- SSO Limitation --> If the credential got compromised then everything could be compromised
- SSO work with Service Provider and Identity Provider as talked above
- SSO Protocols --> OAuth --> SAML (Security Assertion Markup Language) -> use different kinds of Assertion to provide the authentication and other things -> Authentication assertion, authorisation assertion, attribute assertion
- Authentication Framework --> It provides a schema for the user to verify themselves --> Factors -> Forms -> Protocols/Methods -> Tools
- RADIUS (Remote Authentication Dial-In Service) --> It is an Protocol but it also has an framework which works on Radius protocol --> Ensure AAA protocol --> User sends the request for login to a application or device -> device sends the request to Radius authentication server -> Server will decide the authentication, authorisation, and accounting
- Radius use data packet format to exchange data --> 0 - 7 is Code -> 7 - 15 is Identifier -> 15 - 31 is Length -> bellow all this from 0 - 31 is authenticator -> bellow this 0 - 31 is Attribute
- Radius client (like firewall, or any other application in the network) --> sends the user credential -> Radius authentication Server use LDAP(Lightweight Directory Access Protocol) to retrieve credentials of the user from its own directory server or the server provided by the organisation -> match the credentials -> either send a reject response -> accept response -> or accept - challenge response for second factor authentication
- LDAP (Lightweight Directory Access Protocol) --> Could be used for basic authentication also --> its whole use is to retrieve credentials from the server --> send user credential through it -> LDAP will retrieve the credentials from server and match it then return with match or no match
- TACACS+ --> RADIUS ≈ TACACS+ --> RADIUS use UDP -> TACACS+ use TCP --> RADIUS encrypts only Authentication in AAA -> TACACS+ encrypts all AAA
- Other methods of Authentications --> Password Authentication Protocol (PAP) -> 2 way handshake -> you went to a club and you are infant of guard for your authentication -> you speak your credentials to guard -> guard checks your credentials and decide yes or no -> sends back response in yes -> In this anyone who is hiding in the bush (hacker or bad actors) can listen to your credentials --> Challenge Handshake Authentication Protocol -> 3 way handshake -> this time you go to guard and said hi -> guard sent you a random string -> you combine that string with your credentials and then create a hash of it and send it back to guard -> guard do the same thing in his server and check is your credentials are correct or not -> as random number changes every time attacker could not determine the credentials based on guesses and clues.
- IEEE 802.1x port-based authentication framework --> Supplicant(user) sends the request with credentials using digital signature or EAP to Intermediary(authenticator) -> Intermediary receives  it and then sends the credentials to RADIUS authentication server using Radius protocol -> Radius authentication server retrieves the credentials of the user from directory server using LDAP -> RADIUS then matches the credentials and then take actions according to the results
- EAP (Extensible Authentication Protocols) --> EAP is a framework which is like menu from which you could decide the different EAP methods to authenticate --> EAP-FAST -> EAP-Flexible Authentication via Secure Tunnelling -> first time user signs it the authentication server provides the user with PAC(Protected Access Credentials) as it is issued by the authorised authority you can use it every time you login instead of whole sign in process --> Protected EAP (PEAP) -> Encapsulates the user credentials going through TLS tunnel to server -> It authenticate Wi-Fi LAN clients only from server side certificate --> Lightweight EAP (LEAP) -> Encrypts data transmission by dynamically generated WEP keys -> allows authentication from both sides -> no longer in use due as modern tools could break the hash
- Access Control Methods --> Mandatory Access Control -> Absolute law created by administration authority could not be bypassed in any case --> Discretionary Access Control (DAC) -> Owner could change the permission of the resource according to the need --> Lattice Based Access Control -> In this permission works according to the security clearance each and every person in the network get --> Rule-set Access Control -> create a list of rules in which order matter and at the end implicit or explicit works --> Role-Based Access Control -> Instead of providing each and every permission and configuration individually just put users according to their common group and configure them --> Attribute Based Access Control -> You can adjust according to what attribute you need to provide the permissions or access to different types of resources
- Access Control Management Life Cycle --> Provisioning -> Authentication -> Authorisation -> self-Service -> Deprovisioning -> throughout this life cycle Governance remain important part
- Limitations --> Configuring access control --> user experience --> auditing --> Consistency
- User vs Group --> instead of configuring and allowing and revoking permission of single user at time divide all of them in common groups then do it in one go
- Reduce Human Error --> Clear Security Policies --> User Education --> Robust Password creation --> Self-Service Tools --> IT will never Call
- Files and Folders Access Control --> Do not let the anonymous guest to wander around the applications and work with any files or folders it is too risky --> Inheritance lock -> if the folder is locked then each and everything inside should be Locked
- Benefits of Access Controls --> Keep Zero Trust Architecture in mind
- Best Practices --> Work on Administration and Governance --> Determine the Duty Separation --> user Education --> Access Control Policy Creation and Recreation --> Escalation and Disaster Recovery Plan
- (24 November 2026)
- Network Access Control (NAC) --> Appliance or a Virtual Machine -> used to control access to the network -> It has full visibility of Network profile of all the participants along with automatic categorisation of their function
- NAC evaluates security compliance on the basis of User, Device, Location, OS, and other factors
- NAC began as a network authentication and authorisation tool which uses IEEE 802.1x standards
- Captive Portal --> a pop up portal you see whenever trying to connect with public wifi in which you have to accept terms and conditions or enter some credentials etc. --> if it is given through NAC then it could be said as self service portal
- Challenges in NAC --> Guest, BYOD, and IoT pose a serious challenges to NAC -> These devices are personally owned and could not be controlled by NAC -> NAC can't control what applications could run or not in those devices --> most IoTs consist low level authentications, they connect to many different networks from remote locations -> IoTs also connects back to their vendors for user experience data and lot more -> This increase the attack surface area -> But organisations tolerate this due to simplicity, cheap, and easiness
- When MIS introduce NAC to the network -> NAC scans the network and create network profiles of each and every device and other entity in the network along with their categorisation on the basis of their function -> If an entity request for the network resources beyond their function needs then NAC declines the request -> It also includes Guest, Collaborators, and contractors in the network
- NAC can integrate with other security tools and products to enhance the experience and security
- Benefits of NAC --> Improved Security --> Cost Savings --> Enhanced IT Experience --> Ease of Control --> Automation

## Module 8: Endpoint Security
- IoT --> Its a network of Physical objects connected to the internet through sensors, bluetooth, and other technologies
- Different Categorisation of IoT --> Industrial Devices -> Residential Location -> Personal Devices
- Personal Devices --> its very hard to manage data from the personal IoT used in persons daily life as that data is sensitive and could cause a huge harm to a person if compromised
- Residential Location --> Smart Homes -> Secure your Passwords -> implement restriction to data transfer -> Updating patches regularly --> Smart Cities -> Securing and Validating Endpoint connections at enterprise level
- Industrial Devices --> with the union of Operational Technology and Information Technology the use of IoT has been increase as it provides better efficiency, automation and data collection
- Industrial IoT benefits --> Manager get the broader view of the work due to realtime tracking --> ICS can monitor and adjust the parameters on the assembly lines according to the need --> Realtime tracking and sensors increase the safety and maintenance
- Endpoint Security Challenges --> As well the increase in the development of Endpoint is increase the corresponding security of endpoint is not --> It increases the Attack Surface --> When compromised they could be used as Bots
- Precautions to take when introducing new and unknown endpoints --> Identify devices -> collect the information of devices -> add them to an isolated network instead of your main network to check and find out about any risks -> If everything is good to go then add them in main network.
- Best Practices in Endpoint Security --> Identify and learn everything about IoT before connecting it --> Group them according to their security and connection needs --> Separate the traffics of devices according to their functions to prevent infrastructure attack
- Endpoint Hardening Techniques --> Administrative Control --> Local Endpoint Protection --> Endpoint Maintenance --> Endpoint Monitoring
- Administrative Controls --> Secure Passwords --> PoLP --> Restrictions
- Local Endpoint Protection --> Secure Operating Systems and Startups -> Secure the endpoints physically -> keep track of the firmware used in the endpoints used by the organisation -> Keep them updated -> always keep a list of Operating systems types and version only need to be used by the organisation endpoints and sometimes endpoints use boot loader instead of BIOS and UEFI-> UEFI is newer and implement better security then BIOS -> UEFI checks the hardware is valid or not before booting the system -> Locking Down the BIOS is also very good security measure --> Disk Security and Encryption -> Encrypt the disks to prevent any data theft -> FDE (Full Disk Encryption) it is a software based encryption tool which encrypts the disk which is done by OS and key is stored at TPM(Trusted Platform Module) -> Self Encryption Drive --> Data Loss Prevention -> Detect the copying and transferring of large files over the network -> Limit the attachable devices functions -> Could be network based also
- Endpoint Maintenance --> Auto-Update/Patches -> updating patches of OS, firmwares, software and all the devices greatly reduce the overall security risks -> It also helps to slow down any attacker after the breach -> if an attack may able to enter the infrastructure using Zero day then their might be a chance that they would not be able to go further due to other vulnerability patches --> Keep regular Backups of the systems to prevent greater loss
- Endpoint Monitoring --> Endpoint Solutions -> System created by organisation to keep track of endpoint security
- Endpoint Solutions --> Endpoint Protection Platform (EEP) -> Scans the endpoint for malware and other vulnerabilities issues -> keep them updated -> if any risk arise can work swiftly on it --> Endpoint Detection and Response (EDR) -> Can detect malicious movements and suspicious activities on endpoint and take quick actions against them -> Use AI for better security -> Can transmit data to other endpoints regarding the compromised endpoint to block it from their perspective -> It tools provide data on new threats and could quarantine systems that are suspected of compromise --> Through both EEP and EDR, security professions have broader view from top to down on the conditions of the endpoints
- On Unknown Endpoints which you have to provide connection to some of your resources --> create a unique network consisting only the resources which they need -> separated from the original network of enterprise -> implement PoLP
- Asking each and every connection point to decline the unauthenticated devices to connect -> This forces them register to the network for authentication to connect
