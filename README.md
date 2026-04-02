🔐 Log Analysis: Kerberos Authentication Failure Detection

📌 Project Overview

This project focuses on analyzing system log data to detect authentication failures related to the Kerberos protocol. The analysis helps identify suspicious login attempts and potential security threats in a system environment.

---

🎯 Objective

- To analyze log data and identify Kerberos authentication failure events
- To detect repeated access attempts from suspicious IP addresses
- To understand how authentication logs help in identifying attacks

---

🛠️ Tools Used

- LogHub Dataset
- Notepad / VS Code
- Manual log analysis

---

📂 Dataset

- Source: LogHub
- Log Type: System authentication logs

---

🔍 Log Example

163.27.187.39kerberos authentication failed

Explanation:

- 163.27.187.39 → Source IP address
- Kerberos → Authentication protocol
- authentication failed → Login attempt unsuccessful

---

🚨 Analysis Performed

1. Authentication Failure Detection

- Identified multiple "kerberos authentication failed" events
- Indicates unsuccessful login attempts

2. Suspicious IP Behavior

- Same IP address appeared repeatedly
- Indicates repeated access attempts

3. Threat Identification

- Pattern suggests:
  - Possible brute force attack
  - Unauthorized access attempt
  - Suspicious authentication activity

---

📊 Analysis Flow

User → Authentication Request → Kerberos → Log Generated → Analysis → Threat Detection

---

🧠 Key Findings

- Repeated Kerberos authentication failures detected
- Same IP involved in multiple attempts
- Indicates suspicious or malicious behavior

---

⚠️ Security Impact

- Continuous authentication failures may lead to:
  - Credential-based attacks
  - Unauthorized access
  - System compromise

---
🔐 What is Kerberos? 

It is an authentication protocol
Uses tickets instead of passwords
Works in Windows domain environment
----
🎨 Kerberos diagram 
User → AS (Authentication Server) → TGT Ticket
      → TGS (Ticket Granting Server) → Service Ticket
      → Server → Access
----
✅ Conclusion

This project demonstrates how log analysis can be used to detect authentication-related threats. By analyzing Kerberos failure events, suspicious activity can be identified early and necessary security measures can be taken.

---

🚀 Future Scope

- Use SIEM tools like Splunk for automated detection
- Create alerts for repeated authentication failures
- Correlate logs with other security events

---

💬 Interview Explanation

"I analyzed system logs to detect Kerberos authentication failures. I identified repeated failed authentication attempts from a specific IP address, indicating possible brute force or unauthorized access attempts. This helped me understand real-world SOC analysis and threat detection."

---
