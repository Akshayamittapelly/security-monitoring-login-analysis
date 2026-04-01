# Security Monitoring Practical – Suspicious Login Detection

## 📌 Objective
To detect and analyze suspicious login activity by monitoring Windows security logs using Event Viewer.

---

## 🛠️ Tools Used
- Windows Event Viewer  
- Security Logs (Event IDs 4624 & 4625)

---

## 📂 Project Description
This project demonstrates how to identify suspicious login behavior by analyzing system-generated security logs. Failed and successful login attempts are correlated using timestamps to detect potential brute force attacks.

---

## 🔍 Procedure
1. Generated multiple failed login attempts by entering incorrect passwords.  
2. Performed a successful login using the correct password.  
3. Opened Event Viewer and navigated to **Windows Logs → Security**.  
4. Applied filter using Event IDs:
   - **4625** → Failed login  
   - **4624** → Successful login  
5. Analyzed logs based on timestamp and user activity.  

---

## 📊 Observation
- Failed Login (Event ID 4625): **10:43:40**  
- Successful Login (Event ID 4624): **10:43:59**  
- Time Difference: **19 seconds**

---

## 🧠 Analysis
- Multiple failed login attempts were observed.  
- A successful login occurred shortly after the failed attempts.  
- The time gap between events is very small (19 seconds).  
- This pattern indicates suspicious behavior.

---

## ⚠️ Conclusion
The observed activity suggests a possible **brute force attack**, where repeated login attempts are made until the correct credentials are found.

---

## 📸 Screenshots
Screenshots of Event Viewer logs are included in the `screenshots` folder for reference.

---

## 🚀 Future Improvements
- Integration with SIEM tools (Splunk / ELK)  
- Automated alert generation  
- Detection of advanced attack patterns  

---

## 📚 Key Learnings
- Understanding Windows Event Logs  
- Identifying suspicious login patterns  
- Event correlation using timestamps  
- Basic security monitoring techniques  

---
