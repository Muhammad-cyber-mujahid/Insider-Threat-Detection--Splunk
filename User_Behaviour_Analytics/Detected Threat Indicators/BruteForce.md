Brute Force Documentation

Brute force is a malicious technique where attackers repeatedly attempt to guess login credentials by submitting multiple username and password combinations. 

Identifying Brute Force Attack

To identify brute force attempts in the logs, focus on login_failure events with threat_indicator=Brute_Force, indicating multiple failed login attempts. A specific example from the log is a login_failure event with login_attempts>5 and network_zone=External.

Other Signs to Notice Brute Force Attacks  

i) High login_attempts values (e.g., >5) in a single event, suggesting rapid credential guessing.  
ii)Repeated login_failure events from the same ip_address or user within a short time window.

Scenarios to Check for Brute Force

1. Check the users or user who has committed the most brute force attempts and which ip_address was most used
<img width="955" height="299" alt="BruteForce1" src="https://github.com/user-attachments/assets/3fda01b8-62d3-46c8-a84d-d3adcc7b051d" />

2. Which user_role and department combination initiated brute force attempts from network_zone=External with login_attempts>19, and what are the associated client_browser and timestamp values?
<img width="953" height="493" alt="BruteForce2" src="https://github.com/user-attachments/assets/f37fbb00-00ec-4c08-af57-9b246a9cf2da" />


3. Which user and device initiated brute force attempts with action_category=Authentication, and what are the status_code and network_zone values?  
<img width="948" height="490" alt="BruteForce3" src="https://github.com/user-attachments/assets/7958652e-1ca3-4d49-8485-1c63aa6c9b90" />
