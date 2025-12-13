**Amazon ec2**
## My Amazon EC2 Lab Journey

I started this lab by logging into the AWS Management Console and navigating to the EC2 (Elastic Compute Cloud) service. My goal was to launch a virtual server that could act as a basic web server.

### Step 1: Launching an EC2 Instance
- I clicked on **“Launch Instance”** to begin the setup.
- I gave my instance a name: **Web Server**.
- For the Amazon Machine Image (AMI), I selected **Amazon Linux 2**, which is commonly used for web hosting and testing.
- I chose the **t3.micro** instance type because it's free-tier eligible and suitable for lightweight tasks.

  ### Step 2: Configuring the Instance
- I kept the default network settings, which placed the instance in my default VPC and subnet.
- I made sure to enable **Auto-assign Public IP** so I could connect to the instance from my local machine.
- I created or selected an existing **key pair** to securely connect via SSH.

<img width="600" height="600" alt="image" src="https://github.com/user-attachments/assets/915ccc10-2c03-49f2-b004-fb34f2d2967c" />

---

### Step 3: Security Group Settings
- I configured the security group to allow **SSH (port 22)** so I could access the server.
- I also added a rule for **HTTP (port 80)** to allow web traffic, since this will be a web server.

### Step 4: Launch and Verify
- After reviewing all settings, I launched the instance.
- Once it was running, I went to the **Instances** section to confirm its status.
- The instance showed as **Running**, with the name **Web Server** and instance ID **i-06119798e5632cb25**.

<img width="600" height="600" alt="image" src="https://github.com/user-attachments/assets/27d555dc-bfc5-4032-af64-c6f2483a4a7b" />

---

### Step 5: Connecting to the Instance
- I clicked **Connect**, chose the SSH method, and used the terminal to access the server using the key pair.
- After successfully logging in, I updated the system and installed a simple web server (like Apache or Nginx).

### Step 6: Testing the Web Server
- I created a basic HTML page and placed it in the web server’s root directory.
- Then I opened the instance’s public IP in a browser to confirm the page was loading — and it worked!
  
<img width="600" height="600" alt="image" src="https://github.com/user-attachments/assets/15bb6aee-0b3d-4c56-8a42-49965872fc13" />

### Final Notes
- This lab helped me understand how to launch, configure, and connect to an EC2 instance.
- I practiced setting up a basic web server and learned how security groups control access.
- It was a great hands-on experience with AWS infrastructure.

---
