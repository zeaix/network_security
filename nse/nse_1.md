##Fortinet Network Security Expert(NSE) 1

#Module 1: Introduction
- Bad Actors = Attackers (Methods, Knowledge, Motive)
- Explorer, Hacktivist, Cyber Teririst, Cyber Criminals, Cyber Warrior
- White, grey, black, and blue hat

#Module 2: The Threat Landscape
- Bad Actors --> Threat vectors --> Vulnerability, Mechanisms, and Pathways
- Attack paths
- Cybersecurity Threats --> Unauthorised Access, Social Engineering, Malware, System Vulnerabilities
- Threat Intelligence --> Situation based evidences --> Relevant, Actionable, Contextual, Implication --> On existing and coming threats on organisational assets --> Public and Private
- CVSS --> Common Vulnerability Score System
- Common format for Threat Intelligence --> TAXII and STIX
- Understanding cyberthreats on organisation --> Gather public and private threat intelligence --> Process the information --> analyse IOCs --> Disseminate the information --> apply the strategies made on the basis of information
- Cyberattack framework --> Access the Situation -> find the problem -> analyse the impact -> develop and implement strategies --> Cyber Kill Chain by Lockheed Martin --> Reconnaissance -> Weaponisation -> Delivery -> Exploitation -> Installation -> Command and Control -> Exfiltration
- Outbreak Alert --> Keep current with vulnerabilities -> Consult online and offline cybersecurity consultant --> Includes Vulnerability, Technologies affected, timeline, solution, and research done on it.

#Module 3: Social Engineering
- Way an orchestrator will try to make other people do for his own good --> Consist Emotion of the human being in it
- Phishing --> Whale and Spear Phishing --> Smishing and Vishing
- Social Engineering in which people goes to attacker instead attack go to them --> Watering hole, Honey Pot Trap, Tailgating (In this person should need to know that he is helping you), and Scareware
- Quid pro quo, Pretexting, and Baiting
- Insider Threats --> Malicious -> Mole, Lone Wolf, Collaborator --> Negligent -> Pawn, Goof
- Cyber Fraud > Cyber Scams
- Copycat government sites, Holiday Fraud, Romance site Fraud, Mandate Fraud, and Pharming 
- Online Influence --> Campaign to promote something bad or bad rumours --> Creating a Fake ID -> Creating Content -> Posting Content -> Real people watching it and sharing it -> Media will take the story

#Module 4: Malware
- Malware --> Virus -> Triggered, Attached to application, and Spreads
- Virus --> Resident, Non-Resident, Multipartile, Direct Action, Browser Hijacking, Overwrite, Web Scripting Virus, Network virus, Boot Loader virus, File Infector
- Malware --> Worms, Rootkit, DLL Injection, Keylogger, PUB, Spyware, Adware, Dialler, Ransomeware, Adversel AI, Trojan Horse (Dropper, Downloader), Bootware, Cryptojacking
- Attack Surface --> Dropper, Downloader, Shellcode, Code Injection

#Module 5: Cryptography and the Public Key Infrastructure
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

#Module 6: Secure Network (22 November 2026)
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
