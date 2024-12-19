<h1>SIEM Lab</h1>
<h2>Introduction</h2>
This project is part of a SIEM lab designed to monitor Windows Event for security-related activities, such as failed login attempts, successful logins, and privilege escalations. <br />
It includes real-time alerting for potential brute-force attacks to enhance incident response capabilities.

<h2>System Setup</h2>
<h3>Technologies Used</h3>

- [Splunk Enterprise 9.4.0 (Installed on Ubuntu 24.04.1)](https://www.splunk.com/en_us/download/splunk-enterprise.html)
- [Splunk Universal Forwarder (Installed on Windows 10 Enterprise VM)](https://www.splunk.com/en_us/download/universal-forwarder.html)
- Windows Event Logs (Security Logs).

<h3>Environment Setup Steps</h3>
<h4>1. Install Splunk Enterprise on the Ubuntu machine</h4>

- [Download Splunk Enterprise](https://www.splunk.com/en_us/download/splunk-enterprise.html)
- 
- Enable receiving on port 9997:

```bash
sudo /opt/splunk/bin/splunk enable listen 9997
sudo /opt/splunk/bin/splunk restart
```
<h4>2. Install the Universal Forwarder on the Windows Machine</h4>

- [Download Splunk Universal Forwarder](https://www.splunk.com/en_us/download/universal-forwarder.html)
- Run the executable file and follow the wizard installation (you can skip 
