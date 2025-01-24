# cloud-server
Cloud - final assignment

Objective: This project focuses on building a cloud infrastructure that's scalable, secure, and budget-friendly for a startup using AWS services. The main objective is to get the system ready for a launch in Europe while meeting specific business needs and ensuring robust security measures.

Overview of performed tasks (R/S):

R1: Basic Web Server	Through docker desktop

R2: Data Localization	Deployed infrastructure in the eu-central-1 region

R3: Budget Limit	Used t3. micro instances with auto-scaling capped at 5 instances and target 50% CPU utilization

R4: Scalability	Configured an Auto Scaling Group with 2 minimum instances and target tracking policies for scaling

R5: IP Restriction	Security group allows HTTP/HTTPS traffic only from IP 41.66.98.97 (my IP)

S1: ALB Access Only	ALB handles all traffic to EC2 instances, and instances are not directly exposed to the internet

S2: HTTPS Support	HTTPS was used during testing

S3: Instance Updates	Configured user data to update and secure instances on startup

S4: High Availability	Minimum of 2 instances running at all times through Auto scaling group (ASG)

S5: Restrict Traffic	Security groups only allow HTTP and HTTPS traffic
