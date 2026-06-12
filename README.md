# Task 1 - Launch a Virtual Machine on AWS EC2

## Objective

Launch an Ubuntu EC2 virtual machine on AWS Cloud and configure an Apache web server.

## Tools Used

* AWS EC2
* Ubuntu Server 26.04 LTS
* Apache2 Web Server
* EC2 Instance Connect

## Instance Details

* Instance Name: RD-INFRO-Task1
* Instance ID: i-0510332e90f448175
* Instance Type: t3.micro
* Public IP Address: 51.20.105.236
* Operating System: Ubuntu Server 26.04 LTS

## Steps Performed

1. Logged in to the AWS Management Console.
2. Created a new EC2 instance named "RD-INFRO-Task1".
3. Selected Ubuntu Server 26.04 LTS as the operating system.
4. Chose the t3.micro instance type.
5. Generated and downloaded a new key pair.
6. Configured security group settings and allowed SSH access.
7. Launched the EC2 instance successfully.
8. Connected to the instance using EC2 Instance Connect.
9. Updated the package repository.
10. Installed Apache2 Web Server.
11. Started and enabled the Apache2 service.
12. Verified that the Apache service was running successfully.
13. Accessed the Apache default web page using the public IP address.

## Commands Used

```bash
sudo apt update
sudo apt upgrade -y
sudo apt install apache2 -y
sudo systemctl start apache2
sudo systemctl enable apache2
sudo systemctl status apache2
```

## Result

Successfully launched an AWS EC2 virtual machine, connected to the Ubuntu server, installed and configured Apache2 Web Server, and verified successful deployment by accessing the Apache default webpage through the public IP address.

## Screenshots Included

1. EC2 Instance Running
2. Ubuntu Terminal Access
3. Apache2 Service Status
4. Apache Default Web Page
