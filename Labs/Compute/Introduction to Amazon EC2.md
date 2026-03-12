# Amazon EC2: Web Server Deployment and Management



## Introduction
Amazon Elastic Compute Cloud (Amazon EC2) is a web service that provides resizable compute capacity in the cloud. It is designed to make web-scale cloud computing easier for developers.

---

## Topics Covered
This repository demonstrates practical experience with AWS EC2. The following tasks were completed:

* **Instance Launch:** Launched a web server with termination protection enabled.
* **Monitoring:** Monitored the EC2 instance to track performance and health.
* **Security Configuration:** Modified the security group used by the web server to allow inbound HTTP access.
* **Vertical Scaling:** Resized the Amazon EC2 instance to adapt to scaling needs.
* **Safeguards:** Tested termination protection to ensure the server cannot be accidentally deleted.
* **Clean Up:** Disabled protection and successfully terminated the EC2 instance.
<img width="297" height="180" alt="Screenshot 2026-03-11 at 13 58 34" src="https://github.com/user-attachments/assets/53b16932-c050-4ac4-a545-ce5813add556" />

In this project, I deployed an Apache web server on an Amazon EC2 instance. I automated the server setup using a User Data bash script and enhanced security by disabling SSH access, deploying the instance within a custom VPC, and enabling Termination Protection. Finally, I monitored the instance's health and performance using Amazon CloudWatch and EC2 status checks, and tested the remote screenshot feature for troubleshooting.

First, it was not working. 

<img width="425" height="404" alt="Screenshot 2026-03-11 at 14 22 41" src="https://github.com/user-attachments/assets/5d3078c0-4a53-485b-ba17-e19ed71d7f52" />

Then I fixed security settings and server become avaliable.

<img width="426" height="126" alt="Screenshot 2026-03-11 at 14 23 50" src="https://github.com/user-attachments/assets/bfa601d2-3979-4468-8cad-e1c5003ec59d" />

