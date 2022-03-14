# DevOps Practical challenge

Once we have ec2 machine we can launch using terraform.
I am using Ubuntu machine.
upate the packages using below command and install ansible in that machine.

Below 2 commands can be sent to userdata of ec2 server launch 

**sudo apt update**
**sudo apt install ansible**

After that clone this repo in machine using 

**git clone https://github.com/nirupbbnk/devops-practical-challenge.git**

**cd devops-practical-challenge**
**ansible-playbook nginx_Cron.yml**

This will install nginx and alter the content to 3.1
This will also generate a shell script **(weblog.sh)** to check the status of server response
At every minute this job runs the script and stores the result to **weblog.txt**


