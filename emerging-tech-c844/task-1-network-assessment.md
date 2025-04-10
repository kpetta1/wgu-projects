# 🔎 Task 1 – Network Vulnerability Assessment

**Course:** Emerging Technologies in Cybersecurity – C844  
**Author:** Kiarah Pettaway  

> 📌 *This project is based on a fictional academic scenario for educational purposes only.*

---

## 🧠 Objective
Conduct a network vulnerability assessment using Nmap and Wireshark. Identify insecure protocols, outdated systems, and suspicious traffic, and provide recommendations for mitigation.

---

## 🌐 A. Network Topology
- Nmap scan of the `10.168.27.0/24` subnet revealed a **star topology**.
- All devices were connected through a central node (likely a switch or hub).
- Advantage: easy to scale and isolate failures.
- Risk: single point of failure at the central hub.

![Figure 1: Nmap Star Topology](./images/figure1.png)

---

## ⚠️ B. Identified Vulnerabilities

### 1. FTP on Port 21
- Found on host `10.168.27.15`
- **Plaintext protocol**, no encryption
- ⚠️ Susceptible to sniffing (usernames, passwords)

![Figure 2: FTP Service on Port 21](./images/figure2.png)

✅ **Recommendation**: Replace with **SFTP or FTPS**, disable anonymous FTP, enforce TLS/SSL.

---

### 2. LDAP on Port 389
- Found on host `10.168.27.10`
- **Unencrypted LDAP communication**
- ⚠️ Risk of credential interception

![Figure 3: LDAP Detection](./images/figure3.png)

✅ **Recommendation**: Use **LDAPS (port 636)** with TLS encryption.

---

### 3. Windows Server 2012 R2
- Detected OS on `10.168.27.10`
- ⚠️ End-of-support OS — no patches available

![Figure 4: Windows Server 2012 R2 Identified](./images/figure4.png)

✅ **Recommendation**: Upgrade to **Windows Server 2019+**, enable patch management and hardening.

---

## 🔍 C. Additional Network Findings (Wireshark)

### 1. ICMP – Destination Unreachable
- Host `10.168.27.10` pinged `8.8.4.4`
- Received ICMP error: **"port unreachable"**

![Figure 5: ICMP Destination Unreachable](./images/figure5.png)

✅ **Insight**: Indicates blocked ICMP traffic; may impact troubleshooting and latency.

---

### 2. HTTP in Cleartext
- Host downloaded a file via HTTP (not HTTPS)
- ⚠️ Sensitive content exposed to sniffing

![Figure 6: HTTP GET Request in Cleartext](./images/figure6.png)

✅ **Recommendation**: Enforce **HTTPS** across all endpoints and update web servers.

---

### 3. TCP Anomaly – ACKed Unseen Segment
- Possible **TCP sequence prediction attack**
- ⚠️ Suggests session hijack or injection attempt

![Figure 7: TCP ACK Anomaly Detected](./images/figure7.png)

✅ **Recommendation**: Enable TCP sequence randomization; monitor with IDS/IPS.

---

## 🔐 D. Mitigation Summary

| Vulnerability | Solution |
|--------------|----------|
| FTP | Replace with SFTP/FTPS, enforce TLS |
| LDAP | Use LDAPS, secure authentication |
| Outdated OS | Upgrade to supported version |
| ICMP Issues | Refine firewall/IDS policies |
| HTTP Traffic | Enforce HTTPS everywhere |
| TCP Anomaly | Enable randomization, monitor sessions |

---

## 📚 References
- CVE List – [https://cve.mitre.org](https://cve.mitre.org)
- NIST SP 800-115 – Security Testing and Assessment
- Microsoft Lifecycle Docs – Windows Server EOL
- OWASP Secure Headers Project
- CISA Guidance on TCP Vulnerabilities

---

**Contact:**  
Kiarah Pettaway  
[LinkedIn](https://www.linkedin.com/in/kiarah-pettaway) • kiatan@duck.com
