# DB_Creation_Population

## Objective
[Brief Objective]
### GitHub Project Description

This project is a comprehensive exploration of various methods to create a new database in SQL Server Management Studio (SSMS) and populate it using CSV flat files. It includes:
- Setting up a database structure manually and via scripts.
- Importing data using tools like the SQL Server Import and Export Wizard.
- Handling a CSV file to create a table within a new database.

The goal is to make it easier to learn and apply best practices for setting up and populating databases in SQL Server.

[Tools Used]

Microsoft Excel
SQL Management Studio

## Steps

First, locate the dataset or CSV file you’ll be using to upload data into the database table.
![image](https://github.com/user-attachments/assets/26c47895-4468-4034-a7d4-9ef6385028a7)

Next, launch SQL Management Studio as an Administrator and connect using Windows Authentication. 


![image](https://github.com/user-attachments/assets/2e703442-ce91-4605-b8ad-189116709629)
![image](https://github.com/user-attachments/assets/09e0fd37-9e5a-48cc-a734-85cd33f099e8)
![image](https://github.com/user-attachments/assets/986a2686-23cd-47fa-b95b-d75834b2ba2f)



Once connected, we’ll cover the first method for creating a new database: right-clicking on "Databases" in the Object Explorer.

![image](https://github.com/user-attachments/assets/40d2a4c7-4748-49c2-81a0-8473c6a2dd76)

 
Select New Database as your option.

![image](https://github.com/user-attachments/assets/7ab79eff-4db0-481e-b059-2b905a9a890b)


In the **Database Name** field, enter "Student_per1" and click **OK**. This completes the first method for manually creating a database.

![image](https://github.com/user-attachments/assets/87eb656a-2d3d-40f8-aecd-6b2a7e7ac465)
![image](https://github.com/user-attachments/assets/0b4d963b-a350-482a-a81a-cf81d3f15e05)

 
Next, you can create a new database based on an existing one. To do this, right-click on the original database and select **"New Database"**.

![image](https://github.com/user-attachments/assets/41022b96-47ba-4299-bb33-55bca008a161)

Enter "Student_per1test" in the **Database Name** field and click **OK** to create your second database.

![image](https://github.com/user-attachments/assets/712df87a-9cbc-4a04-9084-229ee1c96425)
![image](https://github.com/user-attachments/assets/d9b8b6db-3f36-4bf9-8536-04384dd3b689)



You can also create a new database using an SQL query. Simply select **New Query** from the menu and write your SQL statement.

![image](https://github.com/user-attachments/assets/56c81592-fab6-4453-8ae6-5c45029423d3)

 
Write the query: `CREATE DATABASE Student_per2;` and click **Execute** to create your third database using an SQL query.

![image](https://github.com/user-attachments/assets/363836ff-953b-46db-9b7b-f1da134ce436)
![image](https://github.com/user-attachments/assets/2bebbf49-a0b5-479c-92b5-e92a1372f0f5)


Now that we’ve covered three different ways to create a database, we’ll use the Import Wizard to upload a CSV file into the main **Student_per1** database. Right-click on the **Student_per1** database, go to **Tasks**, and select **Import Flat File**.

![image](https://github.com/user-attachments/assets/51f62c02-f348-4a21-8191-88bbc3ecf793)

![image](https://github.com/user-attachments/assets/9d4f4734-3082-4c11-842f-ff797a6f2e52)


Click **Browse**, locate the **StudentPerformance.csv** file, and select **Open**. Once done, click **Next** to proceed.

![image](https://github.com/user-attachments/assets/3ee003fe-6146-4545-b49f-0dfab8127081)
![image](https://github.com/user-attachments/assets/0f8c29cc-48b9-47e9-b4ed-aea2d256f230)









Once completed, click "Close" and query the database to view the newly imported data. Be sure to select *Student_per1* as the database.

Type `SELECT * FROM dbo.StudentsPerformance;` and click "Execute" to view the newly imported data.

 
This concludes the creation of databases, tables, and data import for this project.![image](https://github.com/user-attachments/assets/b175669f-fdf0-4df6-beaf-6717643cf8fe)
