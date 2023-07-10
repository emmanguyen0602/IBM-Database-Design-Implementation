# Project : Database Design and Implementation
## Scenario  
In this scenario, you have recently been hired as a Data Engineer by a New York based coffee shop chain that is looking to expand nationally by opening a number of franchise locations. As part of their expansion process, they want to streamline operations and revamp their data infrastructure.

Your job is to design their relational database systems for improved operational efficiencies and to make it easier for their executives to make data driven decisions.

Currently their data resides in several different systems: accounting software, suppliers’ databases, point of sales (POS) systems, and even spreadsheets. You will review the data in all of these systems and design a central database to house all of the data. You will then create the database objects and load them with source data. Finally, you will create subsets of data that your business partners require, export them, and then load them into staging databases that use different RDBMS.

## Software used in this project  
In this project, you will use **PostgreSQL Database**, **IBM Db2 Database**, and **MySQL**. These are all relational database management systems (RDBMS) designed to efficiently store, manipulate, and retrieve the data.  

## Data used in this project  
In this project, you will be working with a subset of data from the Coffee shop sample data.

You will use a modified version of the data for the project, so to succeed in the project, download the linked files when prompted in the instructions. You do not need to use any data from the original source.

In your scenario, you will be working with data from the following sources:

- Staff information held in a spreadsheet at HQ
- Sales outlet information held in a spreadsheet at HQ
- Sales data output as a CSV file from the POS system in the sales outlets
- Customer data output as a CSV file from a bespoke customer relationship management system
- Product information maintained in a spreadsheet exported from your supplier’s database

## Objectives  
After completing this lab, you will be able to:

- Identify entities.
- Identity attributes.
- Create an entity relationship diagram (ERD) using the pgAdmin ERD Tool.
- Normalize tables.
- Define keys and relationships.
- Create database objects by generating and running the SQL script from the ERD Tool.
- Create a view and export the data.
- Create a materialized view and export the data.
- Import data into a Db2 database.
- Import data into a MySQL database.
## Task 1: Identify entities
The first step when designing a new database is to review any existing data and identify the entities for your new system.

1. The following image shows sample data from each of the data sources that you will be working with to design your new central database. Review the image and identify the entities you plan to create.
![existing_data](https://github.com/emmanguyen0602/IBM-Database-Design-Implementation/blob/main/Images/existing_data.png)
2. Make a list of the entities you have identified.
## Task 2: Identify attributes
In this task, you will identify the attributes for one of the entities that you plan to create.

1. Using the information from the sample data in the image from Task 1, identify the attributes for the entity that will store the sales transaction data.

2. Make a list of the sales transaction attributes that you identified.
3. 
## Task 3: Create an ERD  
Now that you have defined some of your attributes and entities, you can determine the tables and columns for them and create an ERD.

1. Open a new terminal from the side-by-side Cloud IDE.
2. Use the start_postgres command to start a PostgreSQL service session in the Cloud IDE.
3. Use the pgAdmin weblink to open pgAdmin in a new tab in your browser.
4. Create a new database named COFFEE, view the schemas in the new COFFEE database, and then start a new ERD project.
5. Add a table to the ERD for the sale transactions entity using the information in the following table. Consider what naming convention to use so that your colleagues will be able to understand your data and to ensure that the names are valid in other RDBMS. And use the sample data shown in the image in Task 1 to determine appropriate data types for each column.  
![image1](https://github.com/emmanguyen0602/IBM-Database-Design-Implementation/blob/main/Images/Task3A%20(1).png)
6. Take a screenshot of your ERD and save it as Task3A.png or Task3A.jpg.
7. Add a table to the ERD for the product entity using the information in the following table. Consider what naming convention to use so that your colleagues will be able to understand your data and to ensure that the names are valid in other RDBMS. And use the sample data shown in the image in Task 1 to determine appropriate data types for each column.  
![image2](https://github.com/emmanguyen0602/IBM-Database-Design-Implementation/blob/main/Images/Task3B%20(1).png)
