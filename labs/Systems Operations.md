**Systems Operations**

<img width="600" height="600" alt="image" src="https://github.com/user-attachments/assets/7fd43094-9d21-49c2-8aec-f0a634e6e87a" />

. Created a Route Table
You configured the following:

Name tag: public.route.table — indicating this will be used for public-facing resources.

Route table ID: rtb-027c50b77d0c3b0a6 — automatically assigned by AWS.

VPC association: Linked to your Test VPC (vpc-06e3159bbc09a7547).

Main: No — this is a custom route table, not the default one.

AWS confirmed successful creation with a green banner.

6. Viewed Route Details
Under the Routes tab, you see:

Destination: 192.168.0.0/18 — matches your subnet range.

Target: local — allows internal communication within the VPC.

Status: Active — ready to route traffic.

---

<img width="600" height="600" alt="image" src="https://github.com/user-attachments/assets/8e16d53b-d793-432b-ab7d-16381d7581b8" />

I used the JSON editor to define the policy’s actions:
This allows the user to perform list operations on AWS CloudFormation — useful for viewing stacks, templates, or resources without making changes.

5. Viewed Policy Summary
You’re now on the policy details page, reviewing:

Creation timestamp: December 03, 2025.

Permissions tab: Shows the JSON-based rules.

Entities attached: You can attach this policy to users, groups, or roles.

Policy versions: Currently only one version exists.

