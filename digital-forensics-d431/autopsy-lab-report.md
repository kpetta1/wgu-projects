# 🔬 Digital Forensics Lab Report – Autopsy Analysis (Task 2)

**Author:** Kiarah Pettaway  
**Coursework-Based Project — WGU D431**  

> 📌 *This report documents the results of a simulated forensic investigation performed using Autopsy. All findings are from fictional academic scenarios.*

---

## Objective

To perform forensic analysis on a suspect image using Autopsy, identify potential policy violations, and extract supporting evidence including deleted files and keyword hits.

---

## Case Setup

- **Tool Used:** Autopsy 4.19.1
- **Case Name:** JohnSmith_Investigation
- **Evidence File:** `JSmith_Q1.001`
- **Case Location:** `C:\Users\LabUser\Desktop\Evidence Files`
- **Examiner Name:** 376284567  

![Autopsy Launch Screen](./images/1.png)
![New Case Info](./images/2.png)
![Optional Case Info](./images/3.png)

---

## Adding Data Source

- **Source Path:** `C:\Users\LabUser\Desktop\Evidence Files\JSmith_Q1.001`
- **Ingest Modules Used:**
  - Recent Activity
  - Hash Lookup
  - File Type ID
  - Encryption Detection
  - Picture Analyzer
  - Email Parser

![Add Data Source](./images/4.png)
![Select Source Type](./images/5.png)
![Path Input](./images/6.png)
![Ingest Modules](./images/7.png)

---

## Analysis Results

### 📂 Deleted Files Discovered

Autopsy detected multiple deleted files. Notably:

- `Business_Strategy.pdf`
- `Drilling Methodology.pdf`
- `Oil Company data strategy.pdf`

![Deleted Files Found](./images/9.png)

### 🔍 Metadata for "Business_Strategy.pdf"

- **Owner:** Mike Morris  
- **Created/Modified:** 08/11/2021  
- **Path:** `/img_JSmith_Q1.001/Business_Strategy.pdf`

![PDF Metadata](./images/12.png)

---

## Keyword Searches

Keywords used: `confidential`, `restricted`, `proprietary`, `classified`

Each returned documents with business-sensitive content, suggesting possible insider threat activity:

![Keyword Hits - Confidential](./images/13.png)
![Keyword Hits - Restricted](./images/14.png)
![Keyword Hits - Proprietary](./images/15.png)
![Keyword Hits - Classified](./images/16.png)

---

## File Artifacts: Sensitive Business Documents

Recovered files show unauthorized possession of:
- Energy R&D strategies
- Confidential drilling techniques
- Data suggesting export of documents

![Business Strategy Preview](./images/20.png)
![Oil Strategy Confidential Preview](./images/19.png)

---

## Additional Findings

Two suspicious browser artifacts:
- "How to buy and pay with bitcoin anonymously"
- "The best way to hide something is in plain sight: Crypto laundering"

Indicating a possible attempt to evade tracking or monetize stolen data.

![Bitcoin Anon](./images/21.png)
![Crypto Laundering](./images/23.png)

---

## Conclusion

Autopsy analysis uncovered clear signs of:
- Confidential document access and deletion
- Keywords suggesting sensitive internal data
- Evidence of interest in anonymizing and laundering information

🔐 **Recommendation:** Escalate to security and legal teams for further review and disciplinary action.

---

**Contact:**  
Kiarah Pettaway  
[LinkedIn](https://www.linkedin.com/in/kiarah-pettaway) • kiatan@duck.com
