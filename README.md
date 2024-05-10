<h1>Secure-Web-Hosting-with-AWS-S3-and-CORS-Integration-</h1>

<h2>Description</h2>

Implemented a comprehensive web hosting solution on AWS, leveraging S3 for static website hosting with CORS enabled for seamless integration. Orchestrated the deployment of an EC2 instance in a public subnet, implementing stringent security protocols to restrict HTTP access while permitting SSH only from specified origins. Configured the EC2 instance with Apache HTTP Server to serve dynamic web applications, ensuring clear differentiation from S3-hosted content through unique titles. This project showcases expertise in cloud infrastructure design, security implementation, and web server configuration for scalable and distinguishable web services.
<br />
<br />
<br />
<h2>
<p align="center">
Main Diagram<br/>
 <br />
<img src="https://imgur.com/pRuazAk.png" height="40%" width="80%" alt="Disk Sanitization Steps"/></p>
<br /></h2>
<br />
<h2>Languages and Utilities Used</h2>

- <b>Bash scripting for EC2 user data initialization.</b>
- <b>JSON for specifying CORS rules and EC2 security group settings.</b>
- <b>AWS CLI (Command Line Interface) for managing AWS resources and configurations.</b>
- <b>Boto3 Python library for programmatic interaction with AWS services, utilized for deploying EC2 instances.</b>
- <b>Apache HTTP Server (httpd) for serving dynamic web applications.</b>

<h2>Environments Used </h2>

- <b>AWS Cloud environment was utilized for deploying and managing resources.</b>
- <b>Linux-based operating system for EC2 instances, likely Amazon Linux or Ubuntu, to support Apache HTTP Server and Bash scripting.</b>

<h2>Program walk-through:</h2>

- Created an S3 bucket for hosting a static website.
- Provisioned an Amazon EC2 instance in a public subnet within the default VPC.
- Configured the EC2 instance's security group to allow HTTP access from the internet and SSH access restricted to a designated laptop.
- Installed and configured the Apache HTTP Server (httpd) on the EC2 instance either via user data property during deployment or manually post-deployment.
- Ensured that the web applications served by the EC2 instance and S3 bucket have distinct titles for easy differentiation.
- Implemented all resources creation either through Python scripting or via the GUI-based AWS Management Console.
- Ensured network connectivity requirements:
  - Users from the internet can access applications hosted on both EC2 and S3 bucket.
  - Admin can access the EC2 instance via SSH only from the designated laptop.
  - Restricted connectivity to EC2 instance to only SSH and HTTP protocols.
  - Maintained separation between the applications served by Amazon EC2 and the S3 bucket.




<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
