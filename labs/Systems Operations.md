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

![WhatsApp Image 2025-12-03 at 21 03 07_c92dc70d](https://github.com/user-attachments/assets/6984998c-b088-4c27-8685-86c5f2152030)
