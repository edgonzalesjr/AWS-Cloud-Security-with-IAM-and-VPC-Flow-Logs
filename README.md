## Objective
To develop hands-on cybersecurity skills through practical, real-world applications of AWS services, focusing on Identity and Access Management (IAM), VPC networking, and log-based monitoring.

### Skills Learned
- IAM User and Role Management
  - Creation and management of IAM users, roles, and permissions.
  - Crafting and assigning IAM policies for resource access, with a focus on AWS S3 permissions.
  - Setting up IAM user groups for efficient permission management across a team or organization.
- VPC Networking
  - Designing and configuring a Virtual Private Cloud (VPC), including public subnet.
  - Configuring Internet Gateways and Route Tables for secure and efficient traffic management.
  - Deploying and securing EC2 instance in public subnet.
  - SSH access to EC2 instances, emphasizing secure methods for managing cloud resources.
- Monitoring and Flow Logs
  - Setting up VPC flow logs to capture network traffic for auditing and troubleshooting.
  - Creating and managing CloudWatch log groups to store flow logs.
  - Configuring IAM roles for access to CloudWatch logs and analyzing traffic data for security issues.
  - Verifying traffic flow and log entries by pinging external IPs from EC2 instance.
- Cloud Infrastructure Security
  - Identifying and mitigating security risks by properly configuring IAM policies and VPC settings.    
  - Using cloud-native monitoring tools to improve security visibility and ensure compliance. 

### Tools Used
- AWS Management Console: Used to create, configure, and manage AWS resources such as IAM users, VPCs, EC2 instances, and CloudWatch log groups.
- IAM (Identity and Access Management): For creating users, roles, and policies to control access to AWS services and resources securely.
- Amazon VPC (Virtual Private Cloud): For creating and managing a private network with public and private subnets, security groups, route tables, and internet gateways.
- EC2 (Elastic Compute Cloud): Used to deploy and manage virtual instances within AWS for hands-on learning and testing.
- CloudWatch: For monitoring AWS resources and setting up log groups to track VPC flow logs and network traffic.
- SSH (Secure Shell): To securely access and manage EC2 instances in a cloud environment.

## Practical Exercises

<p align="center">
<img src="https://imgur.com/VRQu1W0.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/nP3IAxw.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>AWS Console Login and Home page.</b>
<br/>

---
![image](https://github.com/user-attachments/assets/a62e785a-73d2-47a2-ad3f-1e9b7fa31a47)

- IAM Roles and Users
<p align="center">
<img src="https://imgur.com/3s46rJu.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/L58bOaJ.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>Create IAM demo-user.</b>
<br/>

<p align="center">
<img src="https://imgur.com/bKasKFy.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/lo5Iki5.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/l2iZnoG.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/lng3syC.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>Granting demo-user console access. Login the IAM demo-user.</b>
<br/>

<p align="center">
<img src="https://imgur.com/3iizt44.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/OO8lfG4.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/0ygr74r.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/vNsxWJo.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>Create IAM Policy to allow demo-user to access the S3 bucket.</b>
<br/>

<p align="center">
<img src="https://imgur.com/dXgsb17.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/PrFhvuV.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/WHI4VqO.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/OkC9I1B.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/s4nWp4Z.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>Assign IAM Policy to demo-user. Access the S3 bucket with IAM demo-user.</b>
<br/>

---

- IAM Groups and Permissions
<p align="center">
<img src="https://imgur.com/4xCWI3t.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/RqcQY5f.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/07LiAlE.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>Create IAM demo-group.</b>
<br/>

<p align="center">
<img src="https://imgur.com/5kaEvTo.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/6MMCnGD.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/LlLTqg6.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>Add IAM demo-user to IAM demo-group.</b>
<br/>

<p align="center">
<img src="https://imgur.com/NpH9qbW.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/L5KYijF.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/GLOZkpy.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/yY6WZPf.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/MSfzO5A.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>Attach IAM Policy to demo-group. Access the S3 bucket with IAM demo-user. The demo-user inhirited the demo-group policy.</b>
<br/>

- AWS VPC Flow Logs
<p align="center">
<img src="https://imgur.com/f3Kbg5L.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>AWS VPC Flow logs diagram.</b>
<br/>

<p align="center">
<img src="https://imgur.com/6Gh8i8I.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/riVQ4JI.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>Create VPC.</b>
<br/>

<p align="center">
<img src="https://imgur.com/uop8uT3.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/j1JCrSi.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/jt7z6hk.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/iKZudxI.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>Create Public and Private Subnet.</b>
<br/>

<p align="center">
<img src="https://imgur.com/PSdHViS.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/YFAVzmQ.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/nHFxKIt.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/X8MSkZ6.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>Create Internet Gateway and Attach to VPC.</b>
<br/>

<p align="center">
<img src="https://imgur.com/i6IL1nn.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/aeuSlR7.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/CxtWZ1u.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>Create Public and Private Route table.</b>
<br/>

<p align="center">
<img src="https://imgur.com/6lpZFv3.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/3eRw0Vg.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/6hOsh2p.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/ZnVv995.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>Associate Public Route table to Public subnet and Private Route table to Private subnet.</b>
<br/>

<p align="center">
<img src="https://imgur.com/eKaKWeD.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/CsYus7b.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/5A5qxyF.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>Attach Public Route table to Internet Gateway. Public subnet is allowed to access the internet. Private subnet is prohibited to internet access.</b>
<br/>

<p align="center">
<img src="https://imgur.com/Jf19JEG.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/lGN7Mjo.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/rHRsRfA.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/NMSXre0.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/vGtkTak.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>Provision Public EC2 Instance in Public subnet.</b>
<br/>

<p align="center">
<img src="https://imgur.com/tuiE1jB.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/WUWWtT0.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/V7GKuVv.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>Create Log group in CloudWatch.</b>
<br/>

<p align="center">
<img src="https://imgur.com/lH7SlXT.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/86glVFo.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/nCn0Mb2.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/nCn0Mb2.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/O9y81cI.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/UfzOlRq.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/tR0Fshx.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/eWihtHl.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/mss6Yl4.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>Setup IAM Permission and Policy. VPC should use the correct IAM Permission and Policy to send Logs to dev-prj-log-group.</b>
<br/>

<p align="center">
<img src="https://imgur.com/I5legq0.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/FgewxQp.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/21xlgAk.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>Attach IAM role to IAM policy.</b>
<br/>

<p align="center">
<img src="https://imgur.com/0onl2Pz.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/p4D0Erm.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/7gFjUSK.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/RQ6GJp7.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/t7QSWT5.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>Create Flow Log.</b>
<br/>

<p align="center">
<img src="https://imgur.com/EUIShRy.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/CHa6I7A.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/R1ZsKOH.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/mfG2rmV.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>Check CloudWatch Log Group to see the logs coming in.</b>
<br/>

<p align="center">
<img src="https://imgur.com/oyvmjRS.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/reeMXZp.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<img src="https://imgur.com/9V4Yu0i.png" height="90%" width="90%" alt="Device Specification"/>
<br/>
<b>Test ping capture to the VPC Flow log and inspect network traffic coming in and going out to VPC.</b>
<br/>

## Outcome
- Practical Security Expertise
  - Ability to configure IAM policies, manage user access, and implement security best practices within AWS.
  - Develop a strong understanding of VPC networking, subnet configuration, and resource isolation to enhance cloud infrastructure security.
- Enhanced Monitoring and Incident Response
  - Proficient in setting up and analyzing VPC flow logs, identifying anomalies, and responding to potential security incidents effectively.
  - Ability to set up comprehensive monitoring solutions using CloudWatch for real-time visibility and security auditing.

## Acknowledgements
This project combines ideas and methods from various sources, such as the Youtube videos by Rahul Wagh and my IT experience. These resources provided the fundamental information and techniques, which were then modified in light of practical uses. 
 - [Amazon AWS](https://aws.amazon.com/)
 - [Rahul Wagh](https://www.youtube.com/playlist?list=PL7iMyoQPMtAN4xl6oWzafqJebfay7K8KP)

## Disclaimer
The sole goals of the projects and activities here are for education and ethical cybersecurity research. All work was conducted in controlled environments, such as paid cloud spaces, private labs, and online cybersecurity education platforms. Online learning and cloud tasks adhered closely to all usage guidelines. Never use these projects for improper or unlawful purposes. It is always prohibited to break into any computer system or network. Any misuse of the provided information or code is not the responsibility of the author or authors.
