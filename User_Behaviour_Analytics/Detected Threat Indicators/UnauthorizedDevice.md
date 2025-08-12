Unauthorized Device Documentation

An unauthorized device refers to hardware, such as USB drives or external devices, used to access or transfer sensitive data without permission. 

Identifying Unauthorized Device Activity

To identify unauthorized device activity in the logs, focus on usb_insert events with threat_indicator=Unauthorized_Device, indicating unauthorized hardware usage. 
A specific example from the log is a usb_insert event with file_path=Nexlify_Staff_Records.xlsx and threat_indicator=Unauthorized_Device.

Other Signs to Notice Unauthorized Device Attacks  
i)usb_insert events with high file_size or bytes_transferred, suggesting large data transfers.  
ii)Activity from network_zone=External or unusual ip_address values, indicating external device usage.


Scenarios to Check for Unauthorized Device Documentation

1. Check the users or user who performed the most unauthorized device actions and which file_path was most targeted
<img width="956" height="350" alt="UnauthorizedDevice1" src="https://github.com/user-attachments/assets/ab7eb3d8-cd41-43b9-b255-aca773ade538" />

2. List session_id, ip_address, and file_path for unauthorized device actions with file_size>5000:
<img width="959" height="482" alt="UnauthorizedDevice2" src="https://github.com/user-attachments/assets/bec1888c-03c9-4534-978d-e4ba8a25c994" />

3. Show user, file_path, and timestamp for unauthorized device activity
<img width="952" height="485" alt="UnauthorizedDevice3" src="https://github.com/user-attachments/assets/ccb06405-7bbc-4724-8354-8d6da7a8db4c" />

