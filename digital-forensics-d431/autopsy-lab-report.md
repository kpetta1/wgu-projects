# 🔍 Autopsy Lab Report – Insider Threat Investigation

**Author:** Kiarah Pettaway  
**Coursework-Based Project — WGU D431**  

> 📌 *This report is based on a fictional lab scenario developed as part of academic training through WGU's D431: Digital Forensics course. It was completed independently and is shared for educational and portfolio purposes only.*

---

## 🧠 Summary

This forensic lab involved analyzing a simulated disk image using Autopsy to investigate suspected insider activity involving the misuse of proprietary information. The objective was to recover artifacts, analyze user behavior, and determine whether confidential data was accessed or exfiltrated.

---

## 🔧 Tools & Environment

- Autopsy (Digital Forensics Suite)
- Provided disk image (.001)
- Windows 10 forensic analysis environment

---

## 🔍 Methodology

1. Created a new case in Autopsy and added the .001 disk image.
2. Enabled ingest modules for file metadata, keyword search, web activity, and recent documents.
3. Conducted keyword searches for terms like "confidential," "proprietary," and "trade secret."
4. Reviewed deleted files, installed applications, user documents, and browser history.
5. Noted time stamps, usernames, and file paths for correlation with suspicious behavior.
6. Exported relevant evidence for reporting.

---

## 🗂️ Key Findings

- **Keyword Search Hits:** Several instances of “confidential” and “proprietary” were found in documents recovered from the user profile.
- **Deleted File Recovery:** Multiple deleted documents related to sensitive topics were recovered and linked to the suspect’s activity.
- **Suspicious Artifacts:** The presence of cryptocurrency-related tools, anonymous browsing software, and file wiping utilities suggested an attempt to cover tracks.
- **Policy Violations:** Recovered artifacts included documents marked “internal use only” located in unauthorized folders, suggesting a breach of company policy and possibly a violation of the NDA.

---

## 🧾 Reporting & Recommendations

- Present findings to HR, Legal, and Compliance teams for further action.
- Recommend disabling access for the involved user(s) and auditing related systems.
- Suggest conducting a wider scope investigation to detect any potential data exfiltration vectors (e.g., USB, cloud syncing tools).

---

## ✅ Skills Demonstrated

- Disk image analysis with Autopsy
- Keyword and metadata search
- Deleted file recovery and correlation
- Reporting technical findings for non-technical stakeholders
- Identification of insider threat behaviors

---

**Contact:**  
Kiarah Pettaway   
[LinkedIn](https://www.linkedin.com/in/kiarah-pettaway/) • kiatan@duck.com
