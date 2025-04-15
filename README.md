⚡ Electricity Billing Management System
An advanced electricity billing software application developed as part of the Advanced Internet Programming Lab (24CAP-652) using Java (Swing/Core) for frontend and MySQL for backend. The system automates the billing process, allowing both administrators and customers to interact with billing data through a user-friendly interface.

📋 Project Overview
The project digitizes the traditional electricity billing system, eliminating manual processes and reducing human errors. It provides functionalities for:

Managing customer data
Calculating monthly bills
Adding taxes and surcharges
Searching and viewing payment details
Performing administrative actions like creating, updating, and deleting customer records
🎯 Objectives
Automate the electricity billing and payment process
Improve efficiency by reducing manual work
Provide secure access for customers and administrators
Ensure accurate and real-time bill generation
Allow customers to view and update their details
🌐 Applicability & Scope
Scope:

Track consumption per month
Maintain customer history
Calculate monthly usage and total bills
Enable online payment and tax inclusion
Applicability:

Replaces traditional paper-based billing
Reduces staff overhead
Increases accessibility for customers
Minimizes errors and billing delays
🖥 Technology Stack
Layer	Technology
Frontend	Java (Swing / NetBeans)
Backend	MySQL
Database	Microsoft SQL Server (for integration)
OS	Windows 10
Hardware Requirements:

Processor: Intel Pentium V or higher
RAM: 16 GB
HDD: 2 TB
64-bit Bus, LCD Monitor, Keyboard & Mouse
🔐 Core Features
🔧 Admin Functionalities
Login / SignUp with security question
Add New Customer
Add Tax Details
Calculate Bill based on meter number and usage
View and Print Customer & Bill Details
Update/Delete Customer Information
👤 Customer Functionalities
Secure Login/SignUp using meter number
View Bill & Personal Information
Update Account Details
🗄 Database Tables
customer: Stores personal info like name, address, phone, meter number
login: Handles login credentials and security questions
tax: Stores tax rates, meter rent, and service charges
bill: Records monthly usage and total bill amounts
meter_info: Stores technical meter details
🧮 Sample SQL Statements
-- Creating a customer table
CREATE TABLE customer (
  name VARCHAR(30),
  meter_no VARCHAR(20) PRIMARY KEY,
  address VARCHAR(50),
  city VARCHAR(20),
  state VARCHAR(30),
  email VARCHAR(30),
  phone VARCHAR(30)
);

-- Inserting a customer
INSERT INTO customer VALUES ('Sai','12345','BTM','Bangalore','Karnataka','sai@gmail.com','9876543333');

-- Updating customer email
UPDATE customer SET email='su@gmail.com' WHERE meter_no='12345';

-- Deleting a customer
DELETE FROM customer WHERE meter_no='12345';
