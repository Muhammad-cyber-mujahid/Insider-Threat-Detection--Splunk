<img width="959" height="487" alt="XSSAttempt1" src="https://github.com/user-attachments/assets/11085d6a-c765-4cc2-8401-e2e85e751d5e" />Cross-Site Scripting (XSS) Documentation

Cross-site scripting (XSS) is a malicious technique where attackers inject harmful scripts, typically JavaScript, into web applications to execute in a user’s browser, compromising their interaction with the site. 

Identifying XSS attack

To identify XSS attempts in the logs, focus on web_access events with threat_indicator=XSS, indicating malicious scripts in url_path. 
A specific url_path example from the log is https://nexlify.com/search?q=<script>alert('xss')</script>.

Other Signs to Notice XSS Attacks  

i) url_path containing JavaScript keywords like <script>, alert, prompt, or onerror.  
ii) Unusual HTTP responses, such as status_code=200 with malicious payloads, indicating successful script execution.


Scenarios to Check for XSS attack

1. List ip_address, status_code, and url_path for XSS attempts:
<img width="959" height="487" alt="XSSAttempt1" src="https://github.com/user-attachments/assets/28d0a8a5-6b32-40ed-b197-d5d51dde5492" />

2. Display session_id, user_role, and client_browser for XSS attempts:
<img width="958" height="440" alt="XSSAttempt2" src="https://github.com/user-attachments/assets/0e2d9d24-4a4d-4e11-bad7-4c5e694ff597" />

3. Show event_id, destination_ip, and timestamp for XSS attempts:
<img width="956" height="482" alt="XSSAttempt3" src="https://github.com/user-attachments/assets/05ac1ca8-923e-4fd7-babd-0207cd2962c4" />
