# 🛡️ OASIS INFOBYTES – TASK 4  
## 📘 Research Report: Common Network Security Threats  

### 🎯 Subject: Analysis of DoS, MITM, and Spoofing Attacks

---

## 1️⃣ 📌 Introduction

🌐 Modern network security is a constant battle against rapidly evolving cyber threats.  
This report focuses on **three major attack vectors** that directly compromise the **CIA Triad**:

- 🔐 **Confidentiality**
- 🧾 **Integrity**
- ⚙️ **Availability**

The threats discussed are:
- 🚫 Denial of Service (DoS / DDoS)
- 🔄 Man-in-the-Middle (MITM)
- 🎭 Spoofing Attacks

---

## 2️⃣ 🚫 Denial of Service (DoS / DDoS) Attacks

### ⚙️ How It Works
A **DoS attack** attempts to shut down a machine or network, making it unavailable to legitimate users.  
A **DDoS attack** uses a **botnet 🤖** (infected “zombie” systems) to overwhelm the target.

**Types of DoS Attacks:**
- 🌊 **Layer 3/4 (Volumetric):** Flooding the network with UDP/TCP packets  
- 🕸️ **Layer 7 (Application):** Flooding web services with HTTP GET/POST requests  

### 💥 Impact
1. 💸 Total service outage and revenue loss  
2. 🏷️ Damage to brand reputation  
3. 🎭 Used as a distraction while data theft occurs  

### 🛡️ Mitigation & Prevention
- 🧹 **Traffic Scrubbing:** Cloudflare, Akamai  
- 🚦 **Rate Limiting:** Restrict excessive requests from a single IP  

### 🌍 Real-World Example
📅 **2024:** Cloudflare mitigated a **29.7 Tbps DDoS attack**, the largest ever recorded, highlighting the scale of modern botnets.

---

## 3️⃣ 🔄 Man-in-the-Middle (MITM) Attacks

### ⚙️ How It Works
An attacker secretly **intercepts and alters communication** between two parties who believe they are communicating directly.

**Common Techniques:**
- 📡 **Interception:** Rogue Wi-Fi hotspots  
- 🔓 **Decryption/Manipulation:** SSLstrip downgrading HTTPS to HTTP  

### 💥 Impact
1. 🔑 Theft of login credentials and session cookies  
2. 💳 Financial transaction manipulation  
3. 🗂️ Exposure of sensitive corporate data  

### 🛡️ Mitigation & Prevention
- 🔐 **Strong Encryption:** TLS 1.3  
- 🛜 **VPNs:** Encrypted communication tunnels  
- 🔑 **MFA:** Multi-Factor Authentication  

### 🌍 Real-World Example (2024–2025)
🕵️ **Salt Typhoon**, a state-linked group, conducted MITM-style intrusions on U.S. telecom providers (AT&T, Verizon), enabling call interception and location tracking.

---

## 4️⃣ 🎭 Spoofing Attacks

### ⚙️ How It Works
Spoofing occurs when attackers **impersonate trusted entities** to gain unauthorized access.

**Common Types:**
- 🧭 **IP Spoofing:** Fake source IP addresses  
- 🔁 **ARP Spoofing:** Mapping attacker MAC to gateway IP  
- 📧 **Email Spoofing:** Forged sender addresses for phishing  

### 💥 Impact
1. 🚪 Bypassing access control lists (ACLs)  
2. 🔄 Enabling MITM attacks  
3. 💣 Phishing leading to ransomware infections  

### 🛡️ Mitigation & Prevention
- 📦 **Packet Filtering:** Ingress & egress filtering  
- 🔍 **DAI:** Dynamic ARP Inspection on switches  
- 📬 **DMARC / SPF / DKIM:** Email sender verification  

### 🌍 Real-World Example (2025)
🎯 **RaccoonO365 phishing network** used advanced spoofing to steal **5,000+ Office 365 credentials** before being dismantled by Microsoft and Cloudflare.

---

## 5️⃣ ✅ Conclusion

🧠 Network protection requires a **Defense-in-Depth strategy**, not a single solution.

By combining:
- 🧰 **Technical controls:** Firewalls, encryption, IDS  
- 🏫 **Administrative controls:** Employee training, incident response  

Organizations can **significantly reduce risk** from DoS, MITM, and Spoofing attacks.

---

### 🏁 Task Status
✅ **OASIS INFOBYTES – Task 4 Completed**  
📂 **Beginner-Friendly & Industry-Oriented Report**
