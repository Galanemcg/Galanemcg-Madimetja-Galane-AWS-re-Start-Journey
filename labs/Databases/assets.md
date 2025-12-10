# **Databases**

<img width="600" height="600" alt="image" src="https://github.com/user-attachments/assets/eedbf5c7-b6b2-433a-8084-57247ab5cca6" />


How I started the lab,
To begin the lab:

- Logged into AWS Console: I accessed my AWS account through the AWS Management Console.
- Navigated to DynamoDB: I searched for “DynamoDB” in the AWS services menu and opened the dashboard.
- Clicked “Create Table”: On the DynamoDB homepage, I saw a prompt to “Create a new table to start exploring DynamoDB.” I clicked the Create Table button.


![WhatsApp Image 2025-11-18 at 21 19 04_fcdc90bd](https://github.com/user-attachments/assets/134b0532-4cbd-4100-92a4-8bce9cf7afec)

- Navigated to EC2: I searched for “EC2” in the services menu and opened the EC2 dashboard.
- Launched a new instance
- Clicked on “Launch Instance”
- Gave the instance a name: Command Host
- Selected an Amazon Machine Image (AMI): ami-02373b999c076305d
- Chose an instance type: t3.micro (suitable for basic workloads)
- Left monitoring disabled for simplicity
- Configured security settings and networking as default
- Started the instance: After reviewing the settings, I launched the instance and waited for it to enter the “Running” state.




![WhatsApp Image 2025-11-17 at 22 37 12_5157117f](https://github.com/user-attachments/assets/9c3815c4-3a56-4ff0-9aed-fb0018e919ab)

- Opened the terminal: I accessed the MariaDB environment through a terminal interface.
- Connected to the database: Logged into the MariaDB server and selected the world database.
- Created a table: Used the CREATE TABLE command to make a new table called city with columns Name and     Region.
- Dropped tables:
- Removed the city table using DROP TABLE world.city;
- Also deleted the country table with DROP TABLE world.country;
- Checked remaining tables: Ran SHOW TABLES; to confirm that no tables were left in the world database.
- Dropped the database: Executed DROP DATABASE world; to remove the entire database.


![WhatsApp Image 2025-11-15 at 21 37 01_ea11ea3f](https://github.com/user-attachments/assets/bcc86865-eef7-4125-9faf-33158b5af60c)

- Navigated to RDS: I searched for “RDS” in the services menu and opened the dashboard.
- Created an Aurora database:
- Clicked on “Create database”
- Selected Amazon Aurora as the engine type
- Chose default settings for simplicity
- Named the database aurora
- Launched the cluster:
- Aurora created a regional cluster named aurora
- It also started provisioning an instance called aurora-instance-1 with the role of Writer
- Viewed database status:
- The cluster showed as Available
- The instance was still in the Creating state
- A success message confirmed the database was created


![WhatsApp Image 2025-11-24 at 20 41 58_b9442268](https://github.com/user-attachments/assets/434dd2bd-f2a4-401e-b5ee-a74486eacb28)
