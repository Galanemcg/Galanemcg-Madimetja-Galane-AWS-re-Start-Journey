**SECURITY LABS SCREENSHOTS**

<img width="600" height="600" alt="image" src="https://github.com/user-attachments/assets/fbb75a08-01dd-4ac8-ad69-63ef950ce751" />


You may have configured permissions via IAM roles to allow Inspector to access and scan these resources.

Triggered Your First Scan

The green banner “Welcome to Inspector. Your first scan is underway” confirms that you initiated the first scan.

This scan checks for critical vulnerabilities across your environment.

Reached the Dashboard View

The dashboard shows environment coverage (e.g., Lambda functions at 100%) and critical findings (currently 0 across all categories).

You can now explore findings by resource type (EC2, Lambda, containers, etc.) and dive deeper into security insight.

---

<img width="600" height="600" alt="image" src="https://github.com/user-attachments/assets/c0647996-a089-422d-afb3-9daacbd80082" />
Enabled Amazon Inspector

I activated Inspector to scan EC2, ECR (Elastic Container Registry), and Lambda functions.

This step involved setting up permissions and enabling scanning across your AWS account or member accounts.

Triggered Your First Scan

The blue banner “Welcome to Inspector…” confirms that scanning is active.

Inspector began analyzing your resources for known vulnerabilities using CVE (Common Vulnerabilities and Exposures) data.

Navigated to Findings → All Findings

You clicked into the Findings section and selected All findings to view every vulnerability detected so far.

This view ranks findings by severity and shows details like:

CVE ID (e.g., CVE-2024-35195)

Impacted resource (e.g., get-request)

Type (e.g., Package)

Severity (e.g., Medium)

---

<img width="600" height="600" alt="image" src="https://github.com/user-attachments/assets/edde0fb1-796a-44ce-8893-8674f3559e5d" />

Enabled Inspector and Activated Scanning

I configured Amazon Inspector to scan EC2 instances, container repositories (ECR), and Lambda functions.

This included setting up permissions and enabling standard scanning for supported resource types.

Navigated to Account Management → Lambda Functions

You clicked into the Account Management section of Inspector.

Then selected the Lambda Functions tab to view scanning coverage and status.

---

<img width="600" height="600" alt="image" src="https://github.com/user-attachments/assets/a354c628-51ff-474b-98ad-d3282162458e" />

Enabled Inspector Scanning for Lambda Functions

I previously activated Amazon Inspector to scan EC2, ECR, and Lambda.

This step ensures your Lambda functions are monitored for package-level vulnerabilities.

Navigated to Resources Coverage → Lambda Functions

I clicked into the Resources Coverage section on the left sidebar.

Then selected Lambda Functions to view which functions are being scanned.

Viewed Scanning Details for Each Function

The table shows:

Function names (e.g., generate-..., get-reque...)

AWS account ID

Runtime (Python-based)

Status: Actively monitored

Last scanned date: November

Filters confirm you're viewing:

Resource type: AWS Lambda Function

Scan type: PACKAGE

---

<img width="600" height="600" alt="image" src="https://github.com/user-attachments/assets/4dbdc13b-f3c6-4912-b89e-ed749d9c85cb" />

Navigated to Fleet Manager → Managed Nodes

I clicked into Fleet Manager, a sub-feature of Systems Manager.

Then selected Managed Nodes to view all EC2 instances that are registered and actively monitored.

Viewed Node Details

The dashboard shows 6 managed nodes, with 3 visible in the screenshot:

Linux-3 and Linux-1 running Amazon Linux

Windows-1 running Microsoft Windows

All nodes are in Running status.

A banner suggests enabling Default Host Management Configuration to automatically manage EC2 instances in your account and region.

---

<img width="600" height="600" alt="image" src="https://github.com/user-attachments/assets/52955a71-e1ef-465c-a2a0-36e9bfb9fcb5" />

Navigate to Patch Manager
In the left-hand sidebar of Systems Manager, scroll down to Node Tools.

Click on Patch Manager.

Step 5: Access Compliance Reporting
Inside Patch Manager, you'll see tabs like:

Compliance reporting

Patch baselines

Patches

Click on Compliance reporting to view patch status across your managed nodes.

Step 6: View Node Patching Details
You’ll now see a list of nodes with patching status.

You can:

Click View log to see patching activity.

Click View detail for more insights.

Use Export to S3 to save reports.

---

<img width="600" height="600" alt="image" src="https://github.com/user-attachments/assets/5662d1c4-cd58-42ee-8bab-f3018725e1c2" />

In the AWS Console search bar, type IAM.

Click on IAM (Identity and Access Management) from the results.

Step 3: Navigate to Account Settings
In the left-hand sidebar, under Access management, click on Account settings.

Step 4: Review or Configure Password Policy
You'll now see the Password policy section.

This is where you can:

Set minimum password length.

Require uppercase, lowercase, numbers, and special characters.

Set password expiration (e.g., 90 days).

Allow users to change their own passwords.

Prevent reuse of previous passwords.

---

<img width="600" height="600" alt="image" src="https://github.com/user-attachments/assets/4594fc56-3d2d-4bea-9994-9db8940f3a6c" />

Attach a Policy to the Group
Inside the group details, go to the Permissions tab.

Click Add permissions > Attach policies directly.

Search for AmazonEC2ReadOnlyAccess — this is an AWS managed policy.

Select it and click Next, then Add permissions.

Step 5: Review Policy Details (Optional but Recommended)
After attaching the policy, you can click on it to view its JSON definition.

This shows what actions are allowed:

ec2:Describe* — lets users view EC2 resources.

elasticloadbalancing:Describe* — view ELB settings.

cloudwatch:ListMetrics — access CloudWatch metrics.

All actions are set to "Effect": "Allow" and "Resource": "*" meaning full read-only access across your account.

---

<img width="600" height="600" alt="image" src="https://github.com/user-attachments/assets/6a227492-ecfe-4c50-af07-50e94d6b5c16" />

Create a Subscription
In the SNS dashboard, click Subscriptions in the sidebar.

Click Create subscription.

Step 5: Fill in Subscription Details
Topic ARN: Paste the ARN of your SNS topic.

Protocol: Select Email from the dropdown.

Endpoint: Enter your email address (e.g., galanemcg@gmail.com).

Step 6: Confirm the Subscription
After clicking Create subscription, AWS will send a confirmation email to the address you entered.

Open the email and click the Confirm subscription link.

---

![WhatsApp Image 2025-11-25 at 19 42 56_b7bb86cb](https://github.com/user-attachments/assets/85f46702-3a36-4934-a4c3-1d9bc0522a34)
![WhatsApp Image 2025-11-25 at 19 46 52_8690892b](https://github.com/user-attachments/assets/c06b5549-569d-49f1-907a-bc4078a309d9)
