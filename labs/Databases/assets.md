# **Databases**

<img width="600" height="600" alt="image" src="https://github.com/user-attachments/assets/eedbf5c7-b6b2-433a-8084-57247ab5cca6" />


How I started the lab,
To begin the lab:

- Logged into AWS Console: I accessed my AWS account through the AWS Management Console.
- Navigated to DynamoDB: I searched for “DynamoDB” in the AWS services menu and opened the dashboard.
- Clicked “Create Table”: On the DynamoDB homepage, I saw a prompt to “Create a new table to start exploring DynamoDB.” I clicked the Create Table button.

---
<img width="600" height="600" alt="image" src="https://github.com/user-attachments/assets/9a021533-dcf7-4090-b143-17c1b70b70f5" />


- Navigated to EC2: I searched for “EC2” in the services menu and opened the EC2 dashboard.
- Launched a new instance
- Clicked on “Launch Instance”
- Gave the instance a name: Command Host
- Selected an Amazon Machine Image (AMI): ami-02373b999c076305d
- Chose an instance type: t3.micro (suitable for basic workloads)
- Left monitoring disabled for simplicity
- Configured security settings and networking as default
- Started the instance: After reviewing the settings, I launched the instance and waited for it to enter the “Running” state.


---
<img width="600" height="600" alt="image" src="https://github.com/user-attachments/assets/b853b7b7-b337-4943-8ad4-27d7e7e72e76" />


- Opened the terminal: I accessed the MariaDB environment through a terminal interface.
- Connected to the database: Logged into the MariaDB server and selected the world database.
- Created a table: Used the CREATE TABLE command to make a new table called city with columns Name and     Region.
- Dropped tables:
- Removed the city table using DROP TABLE world.city;
- Also deleted the country table with DROP TABLE world.country;
- Checked remaining tables: Ran SHOW TABLES; to confirm that no tables were left in the world database.
- Dropped the database: Executed DROP DATABASE world; to remove the entire database.

---
<img width="600" height="600" alt="image" src="https://github.com/user-attachments/assets/d414e324-76f8-4275-8698-ef3e3377aa03" />


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

---

![WhatsApp Image 2025-11-24 at 20 41 58_b9442268](https://github.com/user-attachments/assets/434dd2bd-f2a4-401e-b5ee-a74486eacb28)

- Accessed the lab environment: I logged into the lab interface where I could interact with a command host terminal.
- Connected to the database: The command host was pre-configured to connect to the world database using MariaDB.
- Explored the database structure:
- Viewed the tables country and city
- Observed how queries are sent from the user to the command host, then to the database
- Ran SQL statements:
- Used commands like CREATE, SHOW, ALTER, and DROP
- Practiced creating and deleting tables
- Viewed query results returned from the database to the command host



