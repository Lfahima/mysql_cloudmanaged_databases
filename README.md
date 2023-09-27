# mysql_cloudmanaged_databases

## MySQL setup documentation for both Azure and GCP.
### GCP
For GCP I followed Professor Hants' instuctions from our zoom class. So, first I logged on to GCP using my Stony Brook email and created a new project under AHI-GCP since that is where we have our credits. 
For project name I typed HHA504-Assignment 4, for organziation I made sure it was stonybrook.edu, and for location I clicked AHI-GCP. 
I then navigated to the hamburger, and clicked SQL. I clicked create instance and chose MySQL, and selected ENABLING API.
I was then defualted to "create a My SQL instance" and these are the slections I made:
For "Choose a loud SQL Edition": Enterprise 
For Database Version: MySQL 8.0
For "Choose a preset for this edition...": Sandbox
Under "Customize your instance" and "Machine configuration": select Shared core and 1 vCPU, 0.614 GB
For Instance ID I typed fahima-mysql-assignment4 and set my password
Under connections, made sure it was set to Public IP, and then under "Add A Nerwork" for name I typed Allow All and under Network I typed 0.0.0.0/0 -- this is to make my instance public and allow anyone to connect to my database
Finally, clicked done and create instance
It took me exactly 6 mins and 15 seconds to create my instance. 
### Azure
For Azure, i followed the steps provided by Professors Hants' slides. So, first I logged on to my Azure account, confirming it was my Stony Brook email. 
I then went typed Azure Database for MySQL in the search bar and selected create.
I selected "Flexible Server. 
For the Resource Group Name I typed fahima-mysql-assignment4-azure
Burstable, B1ms
For Compute + Storage I left it at the default which was Burstable, B1ms 1 vCores, 2 GiB RAM, 20 GiB storage, Auto scale IOPS
In the networking tab, I made sure the "Connectivity method" was set to "Public access (allowed IP addresses) and Private endpoint"
I also added the "Firewall rules" which allows public access and had the 0.0.0.0
I made sure it read Compute Sku:USD 12.41/month on the right hand side
Creating my instance on Azure took much longer cmpared to GCP.



## My experience with MySQL Workbench, including the ERD creation and database interactions.
My experience with MySQL Workbench was positive, I did not find it very hard to use or work with. I also did not face any errors when creating my tables or running the commands. I found MySQL to be well organized. The only comaplaint I has was consantly having to quit everytime I wanted to go into another connection. 
I found the ERD creation to be very simple and straight-forward to generate. The ERD for both GCP and Azure were very interesting to view and analyze. 
The database interaction was also stright-forward, I did not run into any errors which I was very happy about. 
