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
