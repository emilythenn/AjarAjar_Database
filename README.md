# AjarAjar_Database

This repository contains the SQL scripts for a Relational Database Management System (RDBMS) designed to manage operations for Ajar Ajar, a non-profit tuition and volunteer organization. The system handles student enrollments, volunteer teaching assignments, financial donations, and operational logistics.

## 📂 Repository Structure

The project is organized into the following files:

| File Name | Description |
| :--- | :--- |
| **`ddl.sql`** | **Data Definition Language**: Contains scripts to drop existing tables and `CREATE` the database schema (Tables, Keys, Constraints). Run this first. |
| **`dml_and_dql.sql`** | **Data Manipulation & Query Language**: Contains `INSERT` statements to populate the database with sample data, followed by `SELECT` queries to generate reports. Run this second. |
| **`README.md`** | Project documentation. |

## 🏗️ System Modules

The database schema is normalized and divided into 7 core modules:

1.  **HR & Employment**: Manages employee contracts, banking details, and roles.
2.  **Parent & Student**: Handles student demographics, health records, and household income data for financial aid.
3.  **Volunteer & Subject**: Tracks volunteer experts, their majors, and the subjects available for tuition.
4.  **Budget & Program**: Manages fiscal budgets and specific educational programs.
5.  **Logistics & Teaching**: Links volunteers to students for classes and manages logistical tasks.
6.  **Student Process**: Tracks registration application statuses and academic history.
7.  **Finance & Reporting**: Records donors, donations, expenses, and generates tax-exempt receipts.

## 🚀 How to Run

To set up this database locally:

1.  **Prerequisites**: Ensure you have an Oracle Database environment (e.g., Oracle SQL Developer, SQL*Plus, or Oracle APEX) installed.
2.  **Execute DDL**:
    * Open `ddl.sql`.
    * Run the script to build the tables. (Note: The script includes "Clean Drop" commands to remove old tables before creating new ones).
3.  **Execute DML & DQL**:
    * Open `dml_and_dql.sql`.
    * Run the script to insert sample data and execute the test queries.

## 📊 Key Reporting Features

The `dml_and_dql.sql` file includes standard CRUD operations and **10 Special User Requirements**, including:

* **Medical Alert System**: Identifies active students with health conditions (e.g., Asthma) and retrieves emergency contacts.
* **Budget Overrun Detection**: Compares total program expenses against the allocated fiscal budget.
* **Volunteer Matching**: Finds certified volunteers based on their University Major who are currently unassigned.
* **Financial Aid Targeting**: Generates reports of applicants from households with income below RM1,500.
* **VIP Donor Tracking**: Identifies donors who have contributed more than RM5,000 annually.

## 🛠️ Built With

* **Oracle SQL** - Database Management System

## 📝 License

This project is created for educational/portfolio purposes.
