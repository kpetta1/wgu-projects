# 📱 Task 2 – WLAN & Mobile Device Security Plan

**Course:** Emerging Technologies in Cybersecurity – C844  
**Author:** Kiarah Pettaway  

> 📌 *This report is based on a fictional academic scenario for educational and portfolio use only.*

---

## 🧠 Objective

Design a wireless LAN (WLAN) and mobile device security plan for a small-to-medium business. Identify risks, apply security best practices, and recommend appropriate controls aligned with industry standards.

---

## 🏢 Scenario Overview

The organization allows employees to access internal resources from both corporate and personal mobile devices. WLAN access is provided across multiple office locations, including remote work capabilities.

---

## ⚠️ Risks & Threats

### WLAN Threats:
- Weak or shared Wi-Fi passwords
- Rogue access points (APs)
- Eavesdropping and MITM attacks
- Lack of segmentation

### Mobile Threats:
- BYOD policy gaps
- Lost or stolen devices
- Outdated mobile OS
- Malware via unsecured apps

---

## 🔐 Recommended Controls

### 🔑 WLAN Security
- Implement **WPA3-Enterprise** with 802.1X authentication
- Segment guest and employee networks via VLANs
- Disable WPS and UPnP
- Use MAC filtering and SSID broadcast control

### 📱 Mobile Device Security
- Enforce **MDM** (Mobile Device Management) for corporate and BYOD devices
- Require device encryption and biometric screen locks
- Use remote wipe and device tracking
- Restrict app permissions; allow only trusted app stores

---

## 🛠️ Tools & Frameworks
- **NIST SP 800-153** – WLAN Security
- **NIST SP 800-124r2** – Mobile Device Security
- **NIST SP 800-46r2** – Telework and Remote Access
- Microsoft Intune / JAMF (MDM)
- WPA3 with AES encryption

---

## ✅ Implementation Strategy

1. Draft and enforce **Acceptable Use Policy (AUP)** for mobile devices
2. Configure WLAN with strong encryption and network segmentation
3. Deploy MDM solution with auto-enrollment
4. Train users on secure device usage and phishing awareness
5. Audit logs and perform regular vulnerability scans

---

## 📚 References
- NIST SP 800 Series: [https://csrc.nist.gov/publications/sp800](https://csrc.nist.gov/publications/sp800)
- CISA Mobile Device Best Practices
- WPA3 Overview: Wi-Fi Alliance
- Microsoft Defender for Endpoint (Mobile)

---

**Contact:**  
Kiarah Pettaway  
[LinkedIn](https://www.linkedin.com/in/kiarah-pettaway) • kiatan@duck.com
