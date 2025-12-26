OASIS INFOBYTES : TASK – 4
Research Report : Common Network Security Threats

Subject: Analysis of DoS, MITM, and Spoofing Attacks.

1. Introduction
Modern network security is a constant battle against evolving threats. This report focuses on three primary attack vectors that compromise the CIA Triad (Confidentiality, Integrity, and Availability): Denial of Service (DoS), Man-in-the-Middle (MITM), and Spoofing.  

2. Denial of Service (DoS/DDoS) Attacks
How it Works
A DoS attack aims to shut down a machine or network, making it inaccessible to its intended users. DDoS (Distributed Denial of Service) is the more common modern version, where the attacker uses a "botnet" (a network of infected "zombie" computers) to flood a target with overwhelming traffic.  
•	Layer 3/4 (Volumetric): Flooding the network pipe with UDP/TCP packets.
•	Layer 7 (Application): Flooding a specific web service with complex requests (e.g., HTTP GET/POST).
Impact
1.	Total service outage and loss of revenue.  
2.	Damage to brand reputation.  
3.	Often used as a "smoke screen" to distract IT teams while another attack (like data theft) occurs.  
Mitigation & Prevention
•	Traffic Scrubbing: Using services like Cloudflare or Akamai to filter malicious traffic before it reaches your server.
•	Rate Limiting: Restricting the number of requests a single IP can make.
Real-World Example:
In late 2024, a massive 29.7 Tbps DDoS attack—the largest ever recorded—was mitigated by Cloudflare, demonstrating the sheer scale of modern botnets.  

3. Man-in-the-Middle (MITM) Attacks
How it Works
The attacker secretly relays and possibly alters the communication between two parties who believe they are directly communicating with each other. This often involves:  
•	Interception: Catching the data (e.g., via a Rogue Wi-Fi Hotspot).  
•	Decryption/Manipulation: Using tools like SSLstrip to downgrade HTTPS to HTTP to read credentials.  
Impact
1.	Theft of login credentials and session cookies.  
2.	Manipulation of financial transactions.  
3.	Compromise of sensitive corporate data.  
Mitigation & Prevention 
•	Encryption: Using strong end-to-end encryption (TLS 1.3).  
•	VPNs: Tunneling traffic through an encrypted "pipe" so an interceptor only sees gibberish.
•	MFA: Multi-Factor Authentication ensures that even if a password is stolen, the attacker cannot log in. 
Real-World Example (2024–2025):
The state-linked group Salt Typhoon executed deep MITM-style intrusions into U.S. telecom providers (AT&T, Verizon), enabling them to intercept voice calls and track locations. 

4. Spoofing Attacks
How it Works
Spoofing occurs when an attacker masquerades as a trusted entity to gain access to a system or steal data.
•	IP Spoofing: Altering the source IP address in a packet to bypass firewalls.  
•	ARP Spoofing: Associating an attacker's MAC address with the IP address of a legitimate gateway.  
•	Email Spoofing: Sending emails with a forged "From" address to trick employees into phishing trap.  
Impact
1.	Bypassing access control lists (ACLs).
2.	Enabling MITM attacks (via ARP spoofing).  
3.	Successful phishing campaigns leading to ransomware.
Mitigation & Prevention
•	Packet Filtering: Implementing ingress and egress filtering to ensure incoming packets are from where they claim to be.  
•	DAI (Dynamic ARP Inspection): A security feature in switches that validates ARP packets in a network.
•	DMARC/SPF/DKIM: Email authentication protocols that verify the sender's identity.
Real-World Example (2025): 
The RaccoonO365 phishing network used advanced spoofing techniques to steal over 5,000 Office 365 credentials before being taken down by Microsoft and Cloudflare in September 2025.

5. Conclusion
Protecting a network is not about a single tool, but a Defense-in-Depth strategy. By combining technical controls (firewalls, encryption) with administrative controls (employee training, incident response plans), organizations can significantly reduce their risk profile against these common threats.
