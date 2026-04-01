📌Project Title
Log Analysis for Kerberos Authentication Failure Detection.

📜description 
Analyzed Linux logs to detect repeated Kerberos authentication failures and identify potential brute force attack from suspicious IP.

🎯 Objective
The objective of this project is to analyze system log files and detect suspicious authentication activities such as repeated login failures and possible unauthorized access attempts.

🛠 Tools Used
Loghub Dataset (Linux Logs)
Notepad / VS Code

📂 Dataset
Linux log file from Loghub dataset was used for analysis.

🔍 Analysis Steps
Extracted the loghub dataset
Opened Linux log file
Searched for authentication-related events
Identified repeated Kerberos authentication failures
Analyzed IP address behavior
Observed session activity (open and close events)

🚨 Findings
Detected multiple Kerberos authentication failures
The IP address 163.27.187.39 attempted authentication repeatedly (~25 times)
This indicates a possible brute force attack or unauthorized access attempt
After several failed attempts, successful session activity was observed
Logs showed session opened and session closed events, indicating system access

⚠️ Security Interpretation
The repeated authentication failures followed by successful login activity may indicate:
Brute force attack attempt
Credential guessing
Possible account compromise risk

✏️ process diagram 
Attacker IP → Multiple Failed Logins → System Logs  
                      ↓  
               One Success Login  
                      ↓  
              Session Opened  
                      ↓  
              Session Closed 

              
📸 proof of project 
session closed and “connection established.png 
session opened- authentication failure.png 
authentication failed.png 

📊 Conclusion“
Log analysis plays an important role in identifying suspicious activities.
By analyzing authentication logs, potential attacks like brute force attempts can be detected early and prevented.
