SQL Injection Documentation 

SQL injection is a malicious technique where attackers insert or inject harmful SQL code into input fields or URLs to manipulate a system’s database.


Identifying SQL Injections

To identify SQL injection attempts in the logs, focus on web_access events with threat_indicator=SQL_Injection, which indicate malicious payloads in url_path. A specific url_path example from the log is https://nexlify.com/contact_us?input=1' OR '1'='1. 

Other signs to notice SQL injection attacks include:
i) Url path containing SQL keywords like OR, UNION, SELECT, or --.
ii) Abnormal user input behavior, such as entering complex strings or special characters in forms.



Scenarios to Check for SQL Injection:

1. Check the users or user who has committed the most SQL injection attempts and which webpath was most targeted

![Dashboard Screenshot](Images/sqli/SQL1.png)



2. Which ip_address initiated the most SQL injection attempts with status=failure, and what is the total count of such attempts per ip_address?

3. List session_id, ip_address, and status_code for SQL injection attempts with status=failure:







