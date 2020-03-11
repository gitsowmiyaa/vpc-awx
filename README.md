# vpc-awx

1. Create a VPC and attach the network to it
2. Create a Ubuntu EC2 instance
3. Install AWX on the Ubuntu machine


*************************************************************
*** Step 1 ***

VPC ID                        : vpc-028a74e3ef39d0944

Virtual Private Gateway ID    : vgw-0f0f8b5ee7070d97b

Subnet ID                     : subnet-004e097145d6d98ab

Route Table ID                : rtb-0b068e4f7d769be8e

Security Group ID             : sg-0c3c14e33e5d63d6b

Internet gateway ID           : igw-042b81b0831bd3dba

NetApp Security Group Ranges: Inbound rules
216.240.16.0/20
217.70.208.0/22
202.3.121.0/24

*** Step 2 ***
 Create Ubuntu Instance and enable the public IP

 *** Step 3 ***
 https://computingforgeeks.com/how-to-install-ansible-awx-on-ubuntu-linux/ 

root@ip-172-16-0-29:~/awx/installer# pwgen -N 1 -s 30
vtpRybypzOsmfnOcDtI8zpMGEMfZGY

docker logs -f awx_task <<== to check any errors after the containers are up ===>>

* One more for reference: https://www.howtoforge.com/how-to-install-ansible-awx-with-nginx-reverse-proxy-on-ubuntu-1804/