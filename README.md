# AWS configuration using Ansible
Create a bastion host , a control machine to configure a web server in aws 

## How to set up
* create 6 ec2 instances from aws console 2 bastion, 2 control, 2 webservers
* create an RDS databaase 
* create S3 Bucket to store .war file
* Create Ansible scripts to configure webserver, database from control
* ssh to bastion and to control box then run command : ansible-playbook -i inventory
* Test if the web page is running by opening dns of the loadbalancer
* If you see your index.html page/ todolist then it is working :)
