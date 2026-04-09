 SOC Lab: Endpoint Monitoring & Log Ingestion with Splunk

 📌 Overview

This project demonstrates the setup of a Security Operations Center (SOC) lab for collecting, forwarding, and analyzing endpoint logs using *Splunk* and *Sysmon*.

The lab simulates real-world log ingestion and troubleshooting scenarios, including identifying and resolving permission issues that prevented log collection.

---

 Architecture

. Windows 10 Endpoint (Sysmon)
. Splunk Universal Forwarder
. Splunk Enterprise (Indexer)

---

 Tools Used

. Splunk Enterprise  
. Splunk Universal Forwarder  
. Sysmon  
. Windows 10 Virtual Machine (VirtualBox)

---

 Issues Encountered

. Logs not appearing in Splunk despite forwarder connectivity  
. Permission errors preventing access to Sysmon logs  
. Misconfigured input settings  

---

 Troubleshooting Process

. Verified forwarder status and connectivity  
. Checked receiving ports on Splunk indexer  
. Investigated splunkd.log for errors  
. Identified permission restrictions on Sysmon log files  
. Updated service account permissions  
. Restarted Splunk forwarder and validated ingestion  

---

 Evidence of Log Pipeline

### Forwarder Monitoring
![](screenshots/forwarder_monitoring.png)

### Permission Issue
![](screenshots/forwarder_permission.png)

### Service Running
![](screenshots/forwarder_service.png)

### Forwarder Connected
![](screenshots/forwarder2_connected.png)

### Receiving Port Configured
![](screenshots/receiving_port.png)

### Sysmon Input Configured
![](screenshots/sysmon_input.png)

### Sysmon Logs in Splunk
![](screenshots/sysmon_logs.png)

### Additional Sysmon Logs
![](screenshots/sysmon_logs2.png)

### Sysmon Operational Logs
![](screenshots/sysmon_operational_logs.png)

---

 Key Takeaways

 Connectivity does not guarantee log ingestion  
 Service account permissions are critical for log access  
 splunkd.log is essential for troubleshooting  
 Practical SOC troubleshooting skills are key to real-world environments  
