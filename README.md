# System-Health-monitoring-Using-Ansible.
System Health Monitoring Ansible 
Title: System Health Monitoring Ansible Script

Description:
This Ansible script provides health monitoring capabilities for a system, allowing you to monitor various aspects such as hard disk utilization, RAM and CPU utilization, and network utilization. The script includes alerting mechanisms to notify you in case of any issues.

Features:
1. Hard Disk Utilization: Monitors the utilization of a specific folder and takes appropriate actions based on the utilization thresholds. When the utilization exceeds the soft limit of 70%, it creates a tar archive of the last three files in the folder. If the utilization reaches the hard limit of 90%, it moves the tar archive to another location and deletes the oldest tar files.

2. RAM and CPU Utilization: Monitors processes that consume more than 70% of CPU or RAM. The script identifies these processes and triggers an alert to notify you of the high utilization.

3. Network Utilization: Monitors processes that utilize the maximum bandwidth and performs traffic analysis. It helps identify processes that consume excessive network resources. Alerts are triggered when significant network traffic anomalies are detected.

This script is designed to be run on a virtual machine (VM) and can be easily integrated into your existing Ansible playbook or deployment pipeline. It provides an automated and proactive approach to system health monitoring, allowing you to identify and address potential issues before they impact the system's performance and stability.

To use this script, ensure that you have Ansible installed on your system. You can execute the script by running the Ansible playbook with the appropriate inventory and variables, as per your environment setup.

Please find the complete Ansible script for system health monitoring in the repository. Feel free to contribute, suggest improvements, and report any issues you encounter.

Note: This script assumes a Linux-based operating system. Adjustments may be required for other operating systems.

Example usage:
```
ansible-playbook systemhealthmonitoring.yml -i inventory.ini
```

We hope this script helps you effectively monitor the health of your system and mitigate potential issues.
