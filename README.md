# ISEA-bridging

Lab work and notes for the ISEA bridging course with Linux system administration, cloud infrastructure (AWS), server security, and automation.


Lab 1: Linux Fundamentals
- Installed and ran Ubuntu
- Practiced basic navigation: pwd, ls, cd
- Created directories and files with mkdir, touch
- Listed and checked the status of active system services
- Explored file/directory permissions with ls -l

Lab 2: Cloud vs On-Prem Cost Comparison & AWS EC2
- Compared cloud vs on-premise total cost of ownership (TCO)
    Cloud: ~$217.48/month
    On-prem: $3,140 first month, then $140/month (hardware, Windows Server license, setup, maintenance)
    Break-even point starts around month 37, after which the two options are nearly identical
- Launched an Ubuntu instance on AWS EC2
- Built a system monitoring script using a loop to auto-refresh stats without manual reruns

Lab 3: DNS, HTTPS, and Task Automation
- Registered a free subdomain on DuckDNS and pointed it to the AWS EC2 instance's public IP
- Set up a Let's Encrypt certificate; confirmed the site loads over a secure HTTPS connection
- Automated weekly system updates using crontab -e (0 2 * * 1) to run auto_update.sh, logging output to /var/log/task.log

Lab 4: Database Server (MariaDB)
- Installed and configured MariaDB
- Verified the setup by listing available databases