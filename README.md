# 📧 The Planet's Prestige – Email Phishing Investigation

## 📌 Findings

| **Field** | **Finding** |
|-----------|-------------|
| **Email Date & Time** | January 26, 2021 – 1:41:18 AM EST |
| **Subject** | *A Hope to CoCanDa* |
| **Sender** | billjobs@microapple[.]com |
| **Reply-To** | negeja3921@pashter[.]com |
| **Recipient** | themajoronearth@gmail.com |
| **Sending Host** | emkei.cz |
| **Source IP** | 93.99.104.210 |
| **SPF Authentication** | Failed |
| **Attachment** | PuzzleToCoCanDa.pdf |
| **Actual File Type** | ZIP Archive |
| **Document Author Metadata** | Pestero Negeja *(Metadata alone cannot verify identity)* |
| **Recovered Location** | The Martian Colony, Beside Interplanetary Spaceport |

---

# 📝 Investigation Summary

A phishing email titled **"A Hope to CoCanDa"** targeted **themajoronearth@gmail.com**, using a fabricated ransom scenario to manipulate the recipient into opening a disguised attachment.

Email header analysis identified multiple indicators of compromise, including failed SPF authentication, mismatched Sender and Reply-To domains, and suspicious email routing. File signature verification confirmed that the attached **PuzzleToCoCanDa.pdf** was actually a ZIP archive containing hidden evidence.

Further forensic analysis uncovered concealed files and Base64-encoded information that ultimately revealed the location:

> **The Martian Colony, Beside Interplanetary Spaceport**

This investigation demonstrates how phishing campaigns leverage spoofed identities, encoded content, misleading file extensions, hidden files, and metadata manipulation to evade detection and complicate forensic investigations.

---

# 📌 Who, What, When, Where, Why & How

| **Category** | **Summary** |
|--------------|-------------|
| **Who** | The phishing campaign targeted **themajoronearth@gmail.com** using a spoofed sender (**billjobs@microapple[.]com**) and a different Reply-To address to disguise the attacker's identity. |
| **What** | A phishing email delivered a disguised ZIP archive masquerading as a PDF, containing hidden files and encoded information. |
| **When** | January 26, 2021, at **1:41:18 AM EST**. No additional malicious activity was identified after delivery. |
| **Where** | The email originated from **emkei.cz (93.99.104.210)** and the hidden evidence referenced **The Martian Colony, Beside Interplanetary Spaceport**. |
| **Why** | The attacker used a fake ransom narrative to mislead the recipient while concealing the true objective through multiple layers of obfuscation. |
| **How** | The attack combined failed SPF authentication, sender spoofing, Base64 encoding, disguised file extensions, hidden spreadsheet data, and manipulated document metadata to evade detection. |

---

### 🔍 Additional Findings

| **Analysis** | **Observation** |
|--------------|-----------------|
| **Email Authentication** | SPF validation failed, indicating the sending server was unauthorized to send email on behalf of the claimed domain. |
| **Sender Analysis** | Sender and Reply-To addresses originated from different domains, suggesting possible spoofing. |
| **Origin** | Email was traced to **emkei.cz** (**93.99.104.210**). |
| **Encoding** | Both the email body and attachment were Base64 encoded to conceal their contents. |
| **Attachment Analysis** | The attachment appeared to be a PDF but was identified as a ZIP archive through file signature verification (`50 4B 03 04`). |
| **Recovered Files** | `DaughtersCrown` (JPEG), `GoodJobMajor` (PDF), and a hidden spreadsheet `Money.xlsx`. |
| **Hidden Evidence** | The concealed spreadsheet contained Base64-encoded data revealing the final location. |


# 🛡️ Recommendations

| **Recommendation** | **Purpose** |
|--------------------|-------------|
| Search for similar emails using the identified Indicators of Compromise (IOCs). | Identify additional affected users. |
| Quarantine or delete matching phishing emails. | Prevent further user exposure. |
| Block malicious email addresses, domains, hosts, and source IPs. | Reduce the likelihood of repeat attacks. |
| Review the recipient's endpoint for evidence of execution or compromise. | Determine potential impact. |
| Enforce SPF, DKIM, and DMARC validation. | Strengthen email authentication. |
| Verify attachment file signatures before opening. | Detect disguised or malicious files. |
| Use sandboxing to inspect suspicious attachments safely. | Prevent malware execution. |
| Preserve emails and extracted artifacts as forensic evidence. | Support future investigations and incident response. |
| Conduct regular phishing awareness training. | Improve user detection and reporting of phishing attempts. |

---

## 🧰 Skills Demonstrated

- Email Security Investigation
- Phishing Analysis
- Digital Forensics
- Email Header Analysis
- File Signature Verification
- Base64 Decoding
- Metadata Analysis
- IOC Identification
- Incident Documentation
- Threat Investigation
- Evidence Collection
- Security Operations (SOC)

---

**Status:** ✅ Completed  
**Category:** Phishing Investigation • Email Security • Digital Forensics • Incident Response
