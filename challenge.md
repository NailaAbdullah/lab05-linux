# Challenge: Security Detective Report

## Question 1: Active User and Home Directory
- **Answer:** I am logged in as student. My home folder is /home/student.
- **Commands:** `whoami`, `pwd`

## Question 2: Hostname and OS Version
- **Answer:** The server hostname is ubuntu-lab01 running Ubuntu 24.04 LTS.
- **Commands:** `hostname`, `cat /etc/os-release`

## Question 3: RAM and Disk Usage
- **Answer:** The server has 1.9Gi total RAM and 4.0Gi of available disk space on root.
- **Commands:** `free -h`, `df -h /`

## Question 4: Login Shell Audit
- **Answer:** The users permitted to log in with /bin/bash are root, student, and lab5user (prior to deletion).
- **Commands:** `grep "/bin/bash" /etc/passwd`

## Question 5: Active Process Count
- **Answer:** There are currently around 220 running processes.
- **Commands:** `ps aux | wc -l`

## Question 6: User Lifecycle Timestamps
- **Answer:** User lab5user creation and deletion events were recorded in the authorization log.
- **Commands:** `sudo grep lab5user /var/log/auth.log`
