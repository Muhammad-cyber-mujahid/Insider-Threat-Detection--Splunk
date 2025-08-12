Known Bad IP Address Documentation

A known bad IP address is an IP address identified as a source of malicious activity, such as malware distribution, phishing, brute force attacks, or other cyber threats. 

Identifying Known Bad IP Addresses

To identify known bad IP addresses in the logs, focus on events with threat_indicator=Known_Bad_IP, indicating IPs linked to malicious behavior. 
A specific example from the log is an ip_address like 185.156.73.54 associated with a web_access event targeting a sensitive endpoint.

Other Signs to Notice Known Bad IP Address Activity  
i)Repeated events from the same ip_address across multiple action types, suggesting coordinated attacks.  
ii)Events from network_zone=External with high bytes_transferred or unusual user_agent values, indicating potential bot activity.

Scenarios to Check for Known Bad IP Addresses

1. Check the users or user who interacted with the most known bad IP addresses and which action was most associated
<img width="959" height="352" alt="KnownBadIP1" src="https://github.com/user-attachments/assets/c27bb2ab-bb0c-4a31-a1b5-dd126fa60371" />

2. Show event_id, ip_address, and client_browser for known bad IP activity
<img width="959" height="479" alt="KnownBadIP2" src="https://github.com/user-attachments/assets/738124de-f5bb-4fbd-bf0b-c67a14b1df3c" />

3. Display session_id, user_role, and network_zone for known bad IP activity
<img width="953" height="490" alt="KnownBadIP3" src="https://github.com/user-attachments/assets/57ce25e4-2895-4622-885d-056b798fd72f" />


