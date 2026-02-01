# Enterprise Expense Management Portal

## Overview
The **Enterprise Expense Management Portal** is a web-based application built using **ASP.NET WebForms** and **SQL Server**.  
It allows users to manage daily expenses by organizing them into categories and visualizing spending through a dashboard.

This project was developed to gain hands-on experience with **enterprise-level concepts** such as authentication, authorization, database-first design, stored procedures, and centralized exception handling using WebForms.

---

## Features

### Authentication & Authorization
- Forms Authentication implemented for secure login
- Role-based authorization for **Admin** and **User**
- Page-level access control based on roles

### User Functionality
- Secure login
- Create and manage expense categories
- Add expenses under each category
- View all expenses on a dashboard
- Edit or delete expenses
- Pie chart visualization for category-wise expense distribution

### Admin Functionality
- Create users
- Assign roles (Admin / User)
- Access admin-level dashboard
- Manage application access using authorization rules

---

## Technology Stack
- **Frontend:** ASP.NET WebForms, HTML, CSS, Bootstrap, JavaScript
- **Backend:** C#, .NET
- **Database:** SQL Server
- **Data Access:** Database-First approach with Stored Procedures
- **Authentication:** Forms Authentication
- **Visualization:** Pie Chart

---

## Application Flow
1. User logs in using Forms Authentication
2. Role-based authorization determines page access
3. Users create categories and add expenses
4. All database operations are handled via stored procedures
5. Dashboard displays expense data and visual insights
6. Admin users manage users and roles

---

## Error Handling & Logging
- Centralized exception handling implemented using `Global.asax`
- All unhandled exceptions are captured at a single point
- Errors are logged using a common logging utility
- Users are redirected to login page without exposing technical details

This approach improves maintainability and reflects real-world production practices.

---

## Database Design
- SQL Server database using Database-First approach
- Stored procedures used for:
  - User authentication
  - Expense category management
  - Expense CRUD operations
  - User and role management
- Improves performance and security

---

## What I Learned
- ASP.NET WebForms page lifecycle
- Forms Authentication and role-based authorization
- Writing and consuming SQL Server stored procedures
- Implementing centralized exception handling
- Building dashboards with data visualization
- Applying enterprise concepts in a WebForms application

---

## Future Enhancements
- User-level dashboard improvements
- Expense filtering by date and category
- Pagination for large datasets

---

## About the Project
This project was developed by a **C# developer with 3 years of experience** as part of learning and applying **ASP.NET WebForms** in an enterprise-style application.

---

## Why This Project
This application demonstrates:
- Strong backend fundamentals
- SQL and stored procedure expertise
- Secure authentication and authorization
- Centralized error handling
- Practical use of ASP.NET WebForms in real-world scenarios

---

## Setup & Run Steps (SQL Server Configuration)

Follow the steps below to run the application locally.

### 1. Prerequisites
- Visual Studio (2019 or later)
- .NET Framework / .NET version used in the project
- SQL Server (LocalDB or SQL Server Express)
- SQL Server Management Studio (SSMS)

---

### 2. Database Setup
1. Open **SQL Server Management Studio**
2. Create a new database (example: `EnterpriseExpenseDB`)
3. Execute the provided SQL scripts from `script.sql` file:
   - Tables
   - Stored Procedures
