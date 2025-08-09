FUTURE_CS_02
This repository documents a cybersecurity intern-led SOC analysis using Elastic Stack (Kibana, Elasticsearch, Logstash) and Kali Linux. It includes monitoring security alerts, potential threats analysis, and incident response.

Tools Used
Elastic Stack (Kibana, Elasticsearch)
Kali Linux
Sample Log Files
MS Word (for reporting)
Key Features
Real-time log analysis via Kibana Discover
Detection of malware (Trojan, Rootkit)
Login failure tracking and brute-force detection
Connection attempt monitoring
Alert severity classification
Incident Timeline
Timestamp	User	IP Address	Action	Threat	Severity
08:30:14	bob	10.0.0.5	malware detected	Trojan Detected	High
05:30:14	alice	198.51.100.42	malware detected	Rootkit Signature	High
07:18:14	bob	172.16.0.3	login failed	-	Medium
05:27:14	charlie	198.51.100.42	login failed	-	Medium
08:31:14	david	10.0.0.5	connection attempt	-	Low
Recommendations
Isolate infected hosts
Trigger endpoint malware scans
Audit user credentials
Monitor flagged IP ranges
Notification Plan
Alert SOC Lead
Share report with IT Security Manager
Prepare containment instructions
Dashboard Screenshots
Include screenshot of:

Filtered Threats and actions
Alert visualizations
Severity breakdowns
🧠 Developer
Bhaskar Pagadala
📍Hyderabad India
