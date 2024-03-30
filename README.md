# ALB-Hands-On

Welcome to the ALB Hands-On project! In this project, we'll walk through setting up an Application Load Balancer (ALB) on AWS and distributing traffic between two EC2 instances running Apache HTTP Server.

𝗧𝗮𝘀𝗸 𝗢𝘃𝗲𝗿𝘃𝗶𝗲𝘄:

The task at hand was to create an Application Load Balancer (ALB) to evenly distribute HTTP traffic across two EC2 instances. Each instance served a simple "Hello" webpage. Additionally, I aimed to configure listener rules to handle /error requests and respond with a custom error message to showcase advanced ALB functionalities.

### Step 1: Launch EC2 Instances
- Create two EC2 instances with HTTP traffic allowed.
- In the user data, install and configure Apache HTTP Server to print "Hello" on each instance.

![EC2 Instances](https://github.com/RimshaAzmat/ALB-HandOn/assets/144583193/5c2db0cc-f18d-4b82-bb7f-6dde09e279ac)

### Step 2: Create Load Balancer (ALB)
- Create a new security group allowing only HTTP traffic.
- Create a target group for the ALB and add the EC2 instances to it.
- 
![ALB Hands-On](https://github.com/RimshaAzmat/ALB-HandOn/assets/144583193/1b8c6a12-54dd-4d3c-b837-4ec4f44ba8ed)

![Security Group](https://github.com/RimshaAzmat/ALB-HandOn/assets/144583193/1caf45c3-7f8a-4dcf-9f41-9f286633d420)

![Target Group](https://github.com/RimshaAzmat/ALB-HandOn/assets/144583193/1d69cf27-cab3-413e-b869-25cf5901dea7)

### Step 3: Configure Listener Rules
- Configure listener rules to handle `/error` requests and respond with a custom error message.
- Test the ALB by copying the DNS name and accessing it multiple times to see traffic switching between instances.

![Listener Rules](https://github.com/RimshaAzmat/ALB-HandOn/assets/144583193/efc13a50-0bdc-4ade-b0e0-605133bef5c2)

### Additional Features:
- Explore advanced configurations like changing security group settings and listener rules.
- Experiment with error responses for specific request conditions.

![Error Response](https://github.com/RimshaAzmat/ALB-HandOn/assets/144583193/4ddc6e35-4637-430b-aa39-e736f2b0adb3)

### Get Started:
Clone or fork this repository to your local machine and follow the step-by-step instructions in the README.md file to set up your ALB Hands-On environment on AWS.

