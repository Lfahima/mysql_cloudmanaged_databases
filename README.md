# mysql_cloudmanaged_databases

## MySQL setup documentation for both Azure and GCP.
### GCP
For GCP I followed Professor Hants' instuctions from our zoom class and lecture slides. First, I logged on to GCP using my Stony Brook email and created a new project under AHI-GCP since that is where we have our student credits. 
For project name I typed HHA504-Assignment 4, for organziation I made sure it was stonybrook.edu, and for location I clicked AHI-GCP. 
I then navigated to the hamburger, and clicked SQL. I clicked create instance and chose MySQL, and selected ENABLING API.
I was then defualted to "create a My SQL instance" and these are the selections I made:
For "Choose a loud SQL Edition": Enterprise 
For Database Version: MySQL 8.0
For "Choose a preset for this edition...": Sandbox
Under "Customize your instance" and "Machine configuration": Selected Shared core and 1 vCPU, 0.614 GB
For Instance ID I typed fahima-mysql-assignment4 and set my password
Under connections, I made sure it was set to Public IP, and then under "Add A Network" for name I typed "Allow All" and under Network I typed 0.0.0.0/0 -- This is to make my instance is public and allows anyone to connect to my database
Finally, I clicked done and create instance
It took me exactly 16 mins and 15 seconds to create my instance. 
### Azure
For Azure, I followed the steps provided by Professors Hants' slides. So, first I logged on to my Azure account, confirming it was my Stony Brook email. 
I then typed Azure Database for MySQL in the search bar and selected create.
I selected "Flexible Server. 
For the Resource Group Name I typed fahima-mysql-assignment4-azure
For Compute + Storage I left it at the default which was Burstable, B1ms 1 vCores, 2 GiB RAM, 20 GiB storage, Auto scale IOPS
In the networking tab, I made sure the "Connectivity method" was set to "Public access (allowed IP addresses) and Private endpoint"
I also added the "Firewall rules" which allows public access and had the 0.0.0.0 already there
I made sure it read Compute Sku:USD 12.41/month on the right hand side, which matched the requirment of the assignment
Creating my instance on Azure took much longer compared to GCP. 


## My experience with MySQL Workbench, including the ERD creation and database interactions.
My experience with MySQL Workbench was positive, I did not find it very hard to use or work with. I also did not face any errors when creating my tables or running the commands. I found MySQL to be well organized. The only complaint I had was consantly having to quit everytime I wanted to go into another connection. 
I found the ERD creation to be very simple and straight-forward to generate. The ERD for both GCP and Azure were very interesting to view and analyze. 
The database interaction was also stright-forward, I did not run into any errors which I was very happy about. 
I was able to copy, paste, and run the codes (without errors) for demographics which was found in 1_1_create.sql, doctors which was found in 1_n_create.sql, medications and patient_medications which was found in m_n_create.sql. The only code I had to alter was patients -- I just added on to the code for patients found in 1_1_create.sql from 1_n_create.sql and m_n_create.sql. 

### Creating a new table
The table I created on my own was titled illness and it incorportated illness ID, illness name, and medication ID which was the foreign key. 
