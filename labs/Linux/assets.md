**Linux Labs**

<img width="600" height="600" alt="image" src="https://github.com/user-attachments/assets/89b24385-adb1-42b1-ac0f-084df7a717a2" />

In this lab, I learned how to create a security group in AWS to control access to a database server.

Step 1: Navigating to VPC Security Groups
I started by logging into the AWS Management Console and going to the EC2 Dashboard. From there, I clicked on Security Groups under the Network & Security section.

---

<img width="600" height="600" alt="image" src="https://github.com/user-attachments/assets/b3218a6b-6876-4f5f-9336-e5b60dd67ac9" />

Step 2: Creating the Security Group
I clicked Create Security Group and gave it the name: DB Security Group

I added a description to explain its purpose: Permit access from Web Security Group

I selected the correct VPC where my resources are hosted.

Step 3: Setting Inbound Rules
I added an inbound rule to allow traffic from the Web Security Group. This means only the web server can talk to the database server — improving security.After reviewing the settings, I clicked Create Security Group. A green banner confirmed that the security group was created successfully.

---

<img width="600" height="600" alt="image" src="https://github.com/user-attachments/assets/8dd64634-cdd7-48cb-af35-ce252525afa7" />

ElastiCache This add-on helps speed up read performance by caching data. It can make MySQL databases up to 80x faster and reduce costs by up to 55%.

RDS Proxy This add-on helps manage database connections more efficiently. It allows applications to pool and share connections, making them more scalable and resilient to failures.

---

<img width="600" height="600" alt="image" src="https://github.com/user-attachments/assets/c9867f71-1478-44b0-aadd-3088e57a01ed" />

During the launch process, I created a new key pair or selected an existing one. This key pair is used to securely connect to the EC2 instance.

Step 3: Downloading PuTTY and PuTTYgen
Since I’m using Windows, I downloaded PuTTY and PuTTYgen. PuTTYgen helped me convert the .pem key file from AWS into a .ppk file, which PuTTY can use.

Step 4: Configuring PuTTY
I opened PuTTY and entered the public IP address of my EC2 instance in the “Host Name” field. I set the Port to 22 and selected SSH as the connection type. Under “Connection > SSH > Auth”, I browsed to the .ppk file I generated earlier.

Step 5: Connecting to the Instance
I clicked Open, and PuTTY launched a terminal window. I logged in using the username ec2-user, and the connection was successful.

---

![WhatsApp Image 2025-11-18 at 09 44 27_54827867](https://github.com/user-attachments/assets/ae57b016-0cab-46e9-a033-271f1efe42bc)
