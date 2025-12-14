**Networking Labs**

<img width="600" height="600" alt="image" src="https://github.com/user-attachments/assets/b05d36ff-edb6-48b2-94cf-e50dadbd4945" />

. Launched EC2 Instances
You clicked “Launch Instance” and configured the following:

AMI (Amazon Machine Image): Likely a free-tier eligible Linux image (e.g., Amazon Linux 2023 or Ubuntu).

Instance Type: t3.micro (free-tier eligible, suitable for basic workloads).

Key Pair: Created or selected an existing key pair for SSH access.

Network Settings:

VPC: vpc-0737386373d2360d3 (named VPC1).

Subnet: Availability Zone us-west-2a.

Storage: Default EBS volume (usually 8 GiB).

Security Group: Allowed SSH (port 22) and possibly HTTP/HTTPS if web access was needed.

---

<img width="600" height="600" alt="image" src="https://github.com/user-attachments/assets/d96055a4-ead4-463b-9429-3d65762040b9" />

I landed on the VPC Dashboard, which summarizes your networking resources:

VPCs: 1 (likely named VPC1 — matches your EC2 instance config).

Subnets: 4 (used to segment your VPC across availability zones).

Route Tables: 1 (controls traffic routing within your VPC).

Internet Gateway: 1 (enables internet access for public subnets).

Security Groups & Network ACLs: 1 each (used for traffic filtering and access control).

4. Confirmed Network Setup for EC2
This step helps verify that your EC2 instances are correctly connected to:

A VPC with internet access.

A subnet in us-west-2a.

A security group allowing SSH (port 22) and possibly HTTP/HTTPS.

---

<img width="600" height="600" alt="image" src="https://github.com/user-attachments/assets/3cfc2f20-2e1c-447b-9827-b23ef3279607" />

Navigated to the VPC Service
From the AWS Console home, you searched for or clicked on VPC (Virtual Private Cloud).

This service lets you build a custom, isolated network environment in the cloud.

3. Clicked “Create VPC”
You chose to manually create a VPC instead of using the default one.

This gives you full control over IP ranges, subnets, gateways, and routing.

4. Configured VPC Settings
Resources to create: You selected “VPC only”, meaning you’ll manually add subnets, route tables, and gateways later.

Name tag: You entered Test VPC to help identify this VPC in your dashboard.

IPv4 CIDR block: You manually input 192.168.0.0/18, which defines the private IP range for your VPC.

This gives you 16,382 usable IP addresses, suitable for a medium-sized network.

IPv6 CIDR block: You chose “No IPv6 CIDR block”, keeping it simple for now.

---

<img width="600" height="600" alt="image" src="https://github.com/user-attachments/assets/8d6ad258-1afe-43cc-bfd6-4e02ed768118" />

Opened the VPC Service
You navigated to VPC (Virtual Private Cloud) from the AWS Console home.

3. Created a Custom VPC
You clicked “Create VPC” and configured the following:

Name tag: Test VPC — helps identify your VPC in the dashboard.

IPv4 CIDR block: 192.168.0.0/16 — a large private IP range offering 65,536 IP addresses, suitable for complex network setups.

IPv6 CIDR block: None selected — keeping it IPv4-only for simplicity.

Resources to create: You chose “VPC only”, meaning you'll manually add subnets, route tables, and gateways later.

4. VPC Successfully Created
AWS confirmed the creation with a green banner.

You’re now viewing the details of your VPC, including:

VPC ID: vpc-06e3159bbc09a7547

DNS resolution: Enabled (important for hostname-based communication).

Main route table: rtb-01e7459f90344f67

Main network ACL: acl-0b763b30b62fd1031

Block Public Access: Off (you’ll manage access via security groups and gateways).

DHCP option set: Default — used for assigning internal IP settings.

---


<img width="600" height="600" alt="image" src="https://github.com/user-attachments/assets/f6f4b72d-22b9-4563-bcc9-0d7b5e8a71c1" />

![WhatsApp Image 2025-11-21 at 23 02 15_c280fe33](https://github.com/user-attachments/assets/d5978fc0-f8b1-43b6-a834-4c1b2f009b8e)
