Objective: Monitor simulated logs, identify 3–5 suspicious alerts, classify severity, and produce an incident report with dashboard evidence.

Tools: Splunk Enterprise (Free/Trial), provided sample logs.

Method:

Ingested SOC_Task2_Sample_Logs.txt via Add Data > Upload.

Searched for failed logins, malware events, success-after-fail sequences.

Built dashboard panels (failed logins over time, top source IPs, malware by host).

Key Findings (examples—replace with your actuals):

High: Brute-force pattern (EventCode 4625) from <IP> targeting <user>.

High: Malware detection “<signature>” on <host>.

Medium: Successful login after multiple failures for <user> from <IP>.

Deliverables:

Incident_Response_Report_Task2.pdf (timeline, analysis, remediation)

screenshots/ (dashboard + searches)

searches.md (SPL used)

alert_log.md (classification table)

Example SPL (see searches.md for full):

failed OR "failed login" OR failure | stats count by src_ip, user | sort - count

… (bursts over time, success-after-fail correlation, malware terms)
