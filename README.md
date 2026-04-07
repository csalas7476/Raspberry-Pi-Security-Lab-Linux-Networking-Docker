# Raspberry-Pi-Security-Lab-Linux-Networking-Docker
*Raspberry Pi security lab for Linux, networking, and Docker experimentation SOC-focused Raspberry Pi lab: network monitoring, Linux hardening, and Docker security Hands-on Raspberry Pi lab for cybersecurity learning and SOC skills

1. Set up the testing environment  
   - Installed Docker on Kali Linux  
   - Verified Docker was running properly 

2. Deployed OWASP Juice Shop container  
   - Pulled the Juice Shop image from Docker Hub  
   - Ran the container locally on a specified port (3000:3000)
  
   - <img width="1920" height="1045" alt="Screenshot_2026-03-25_13-53-56" src="https://github.com/user-attachments/assets/1103d3af-f634-407a-bb5e-e8e853be33ee" />


3. Configured Burp Suite  
   - Launched Burp Suite Community Edition  
   - Set up the proxy listener (127.0.0.1:8080)  
   - Enabled intercept mode
  
   - <img width="1172" height="700" alt="Screenshot_2026-03-25_13-56-26" src="https://github.com/user-attachments/assets/b029c92e-1510-4353-9c23-da53655f0bfc" />


4. Connected browser to Burp Suite  
   - Configured browser proxy settings to route traffic through Burp  
   - Installed Burp’s CA certificate to avoid HTTPS errors
  
   - 

5. Accessed the Juice Shop application  
   - Opened the app in the browser via localhost  
   - Confirmed traffic was being captured in Burp Suite
  
   - <img width="1920" height="1045" alt="Screenshot_2026-03-25_13-59-07" src="https://github.com/user-attachments/assets/e4ae739c-6c4c-4d78-817d-4f29ac635db4" />


6. Monitored login activity  
   - Navigated to the login page of Juice Shop  
   - Entered test credentials  
   - Observed intercepted HTTP/HTTPS requests in Burp
  
   -  <img width="1920" height="1045" alt="Screenshot_2026-03-25_13-59-48" src="https://github.com/user-attachments/assets/7daa7ef0-35f6-47ec-9d58-f9c1bb35b2ce" />


7. Analyzed requests and responses  
   - Examined login request payloads (POST data)  
   - Reviewed headers, cookies, and parameters  
   - Identified how authentication data is transmitted
  
   - <img width="1920" height="1045" alt="Screenshot_2026-03-25_13-59-48" src="https://github.com/user-attachments/assets/21c335a0-b52d-4e52-b7d1-e903e701476f" />


8. Tested multiple login attempts  
   - Sent repeated login requests  
   - Observed differences in server responses  
   - Checked for potential vulnerabilities (e.g., lack of rate limiting)
  
   - <img width="1920" height="1045" alt="Screenshot_2026-03-25_19-54-03" src="https://github.com/user-attachments/assets/bd158709-fca2-42e2-8d44-3d13b73048db" />


9. Documented findings  
   - Recorded screenshots of intercepted traffic  
   - Noted key observations about authentication behavior  
