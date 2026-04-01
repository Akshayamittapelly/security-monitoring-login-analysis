# Suspicious Login Detection

## Objective
To detect suspicious login activity using Windows Event Viewer.

## Tools
- Event Viewer
- Security Logs

## Process
- Generated failed login attempts
- Performed successful login
- Filtered logs using Event IDs 4624 and 4625
- Compared timestamps

## Observation
- Failed: 10:43:40  
- Success: 10:43:59  
- Time gap: 19 seconds  

## Conclusion
Short time gap between failed and successful login indicates possible brute force attack.

## Screenshots
Screenshots are added in the images folder.
