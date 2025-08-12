Insider Threat Detection with Splunk

Overview
This project uses Splunk to detect insider threats in a fictional company, Nexlify Solutions, by analyzing user activity logs. The dataset, user_activity_nexlify.json, has 7000–8000 events, including 2100–3200 malicious ones like brute force, phishing, SQL injection, and unauthorized device use. It’s designed to help SOC analysts practice spotting threats and documenting findings.

Goals
- Identify insider threats like data leaks or unauthorized access using Splunk queries.
- Practice writing queries to find patterns in logs (e.g., suspicious IPs or user actions).
- Document key threats (e.g., brute force, XSS) with clear explanations and visuals.
- Simulate a real-world scenario to build threat-hunting skills.

Real-World Scenario
Nexlify Solutions noticed sensitive data leaks and odd login attempts, suspecting insider threats from employees or hacked accounts. For example, an employee made repeated login attempts from outside the company network. This project uses Splunk to analyze logs, catch these threats, and help the company secure its data.

Steps
1. Generate logs using a Python script (user_behaviour_nexlify_logs.py) to create user_activity_nexlify.json
2. Upload the JSON file to Splunk Cloud with "_json" source type into "user_activity_index"
3. Check data in Splunk with index=user_activity_index | stats count (7000–8000 events)
4. Run queries to find malicious activities 
5. Create dashboards to visualize threats 
6. Document findings for each threat type in with queries and screenshots
7. Save results and visuals in screenshots/ and update GitHub repo.
8. Compile a final report with insights and recommendations.

Requirements
- Splunk Cloud (free trial works) for log analysis.
- Python 3.13 to run the log generation script.
- VS Code for editing/running the script.
- user_activity_nexlify.json (7–10 MB) with fields like user, action, ip_address.
- GitHub repo for storing scripts, docs, and screenshots.

