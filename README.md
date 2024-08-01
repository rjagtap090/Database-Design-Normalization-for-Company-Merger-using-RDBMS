Database Design & Normalization for Company Merger using RDBMS

Overview

This project focuses on integrating post-merger datasets using Relational Database Management Systems (RDBMS). The primary goal was to employ normalization techniques along with SQL joins and unions to eliminate data redundancy and ensure data integrity. This project was carried out as part of a course at the University of Delaware from February 2023 to May 2023.

 Features

- Normalization: Applied normalization rules to organize database structure, ensuring minimal redundancy and dependency.

- SQL Joins and Unions: Used SQL joins and unions for merging datasets and enabling efficient data retrieval.

- Data Integrity: Ensured data integrity through proper database design and management practices.

- Efficient Data Retrieval: Facilitated informed decision-making through optimized data retrieval processes.

 Skills Demonstrated

- RDBMS: Utilized relational database management systems to handle and manage data.

- Database Design: Designed database schemas to accommodate merged data.

- Data Analysis: Conducted data analysis to ensure the quality and integrity of integrated datasets.

- Data Management: Managed large datasets to support business requirements post-merger.

- Data Cleaning: Cleaned and prepared data for integration.

- Microsoft SQL Server: Implemented the project using Microsoft SQL Server.

Methodology

1. Data Integration:

   - Gathered datasets from merging companies.

   - Cleaned and prepared data for integration.

2. Normalization:

   - Applied normalization techniques to organize the database structure.

   - Ensured minimal data redundancy and dependency.

3. Database Design:

   - Designed database schemas to support the merged data.

   - Used SQL joins and unions for data integration.

4. Implementation:

   - Implemented the database design using Microsoft SQL Server.

   - Verified data integrity and optimized retrieval processes.

 SQL Code(More indepth in ACCESS file)

```sql

-- Example of creating normalized tables

CREATE TABLE Employees (

    EmployeeID INT PRIMARY KEY,

    FirstName NVARCHAR(50),

    LastName NVARCHAR(50),

    DepartmentID INT,

    FOREIGN KEY (DepartmentID) REFERENCES Departments(DepartmentID)

);

CREATE TABLE Departments (

    DepartmentID INT PRIMARY KEY,

    DepartmentName NVARCHAR(50)

);

-- Example of using SQL JOIN

SELECT Employees.EmployeeID, Employees.FirstName, Employees.LastName, Departments.DepartmentName

FROM Employees

INNER JOIN Departments ON Employees.DepartmentID = Departments.DepartmentID;

-- Example of using SQL UNION

SELECT EmployeeID, FirstName, LastName FROM EmployeesOld

UNION

SELECT EmployeeID, FirstName, LastName FROM EmployeesNew;

```

Results

- Data Integrity: Ensured through effective normalization and database design.

- Efficient Retrieval: Enabled fast and reliable data access for decision-making.

- Scalable Design: Created a scalable database structure to accommodate future growth.

Author

- Rishabh Jagtap  [Email](mailto:rjagtap9299@gmail.com))

Acknowledgments

- Professors and Mentors at the University of Delaware

- Department of Business Analytics and Information Management
