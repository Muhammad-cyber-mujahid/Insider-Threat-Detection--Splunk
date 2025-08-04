Phishing Documentation

Phishing is a malicious technique where attackers send fraudulent emails or messages to trick users into revealing sensitive information or interacting with harmful links.

Identifying Phishing attack

To identify phishing attempts in the logs, focus on email_sent events with threat_indicator=Phishing_URL, which indicate malicious URLs in url_path. A specific url_path example from the log is https://mail.nexlify.com/compose?to=http://fake-login.com.

Other Signs to Notice Phishing Attacks  

i) url_path containing suspicious domains or URLs that mimic legitimate sites (e.g. fake-login.com).  



Scenarios to Check for Phishing:

1. Check the users or user who has committed the most SQL injection attempts and which webpath was most targeted





2. Which ip_address initiated the most SQL injection attempts with status=failure, and what is the total count of such attempts per ip_address?

3. List session_id, ip_address, and status_code for SQL injection attempts with status=failure:










