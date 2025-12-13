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

![WhatsApp Image 2025-11-13 at 21 44 53_52b7ea71](https://github.com/user-attachments/assets/4dab43f4-74cb-460d-aeaa-838e512bb6e0)
![WhatsApp Image 2025-11-17 at 20 39 06_0c20e140](https://github.com/user-attachments/assets/d4b5370f-504a-4b54-9b9c-61c2895e3e88)
![WhatsApp Image 2025-11-18 at 09 44 27_54827867](https://github.com/user-attachments/assets/ae57b016-0cab-46e9-a033-271f1efe42bc)
