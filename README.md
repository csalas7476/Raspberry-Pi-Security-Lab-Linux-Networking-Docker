# Raspberry-Pi-Security-Lab-Linux-Networking-Docker
*Raspberry Pi security lab for Linux, networking, and Docker experimentation SOC-focused Raspberry Pi lab: network monitoring, Linux hardening, and Docker security Hands-on Raspberry Pi lab for cybersecurity learning and SOC skills

1. Set up the testing environment  
   - Installed Docker on Kali Linux  
   - Verified Docker was running properly  

2. Deployed OWASP Juice Shop container  
   - Pulled the Juice Shop image from Docker Hub  
   - Ran the container locally on a specified port (3000:3000)  

3. Configured Burp Suite  
   - Launched Burp Suite Community Edition  
   - Set up the proxy listener (127.0.0.1:8080)  
   - Enabled intercept mode  

4. Connected browser to Burp Suite  
   - Configured browser proxy settings to route traffic through Burp  
   - Installed Burp’s CA certificate to avoid HTTPS errors  

5. Accessed the Juice Shop application  
   - Opened the app in the browser via localhost  
   - Confirmed traffic was being captured in Burp Suite  

6. Monitored login activity  
   - Navigated to the login page of Juice Shop  
   - Entered test credentials  
   - Observed intercepted HTTP/HTTPS requests in Burp  

7. Analyzed requests and responses  
   - Examined login request payloads (POST data)  
   - Reviewed headers, cookies, and parameters  
   - Identified how authentication data is transmitted  

8. Tested multiple login attempts  
   - Sent repeated login requests  
   - Observed differences in server responses  
   - Checked for potential vulnerabilities (e.g., lack of rate limiting)  

9. Documented findings  
   - Recorded screenshots of intercepted traffic  
   - Noted key observations about authentication behavior  
