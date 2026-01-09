# 🏢 Employee Attendance & Payroll Management System (Full HR Database)

A complete HR-grade SQL project that manages employees, attendance,
leave records, salary components, overtime, and fully automated monthly
payroll processing using **MySQL**.\
This project demonstrates real-world database design, business logic,
and SQL automation using **procedures, triggers, constraints, and
views**.

------------------------------------------------------------------------

## 🚀 Features

### 👤 Employee Management

-   Stores employee info: name, department, role, salary, joining date\
-   Unique employee IDs\
-   Data validation using constraints

### 🕒 Attendance Tracking

-   Daily attendance logging\
-   Present / Absent / Leave status\
-   Overtime hour tracking

### 📝 Leave Management

-   Sick, Casual, and Paid leave records\
-   Auto integration with payroll

### 💰 Salary Structure

-   HRA, DA, Bonus stored per employee\
-   Used in payroll calculation

### 📊 Automated Payroll Processing

-   Total working days\
-   Present & absent days\
-   Overtime compensation\
-   Gross salary\
-   Net salary (after deductions)\
-   Fully automated via SQL **Stored Procedure**

### ⚡ Auto Payroll Trigger

-   Whenever attendance is added\
-   Payroll updates automatically

### 👀 Payroll Summary View

-   Clean report of each employee\
-   Easy to read monthly salary details

------------------------------------------------------------------------

## 🧱 Tech Stack

  Component       Technology
  --------------- -------------------------------------------
  Database        MySQL
  Language        SQL
  Concepts Used   Triggers, Views, Stored Procedures, Joins
  Tool            MySQL Workbench

------------------------------------------------------------------------

## 📂 Database Schema

### **Tables Used**

-   `employees`\
-   `attendance`\
-   `leave_records`\
-   `salary_structure`\
-   `payroll`

------------------------------------------------------------------------

## 🏗 ER Diagram (Textual)

    EMPLOYEES (1) ----- (∞) ATTENDANCE  
    EMPLOYEES (1) ----- (∞) LEAVE_RECORDS  
    EMPLOYEES (1) ----- (1) SALARY_STRUCTURE  
    EMPLOYEES (1) ----- (∞) PAYROLL

------------------------------------------------------------------------

## 🛠 How to Run This Project in MySQL Workbench

### **1. Create & Select Database**

``` sql
CREATE DATABASE employee_payroll;
USE employee_payroll;
```

### **2. Run All Table Creation Queries**

(Employees, Attendance, Salary Structure, Leave, Payroll)

### **3. Insert Sample Data**

### **4. Create Stored Procedure**

`calculate_payroll()`

### **5. Create Trigger**

`auto_update_payroll AFTER INSERT ON attendance`

### **6. Create Payroll Summary View**

### **7. Test Payroll**

``` sql
CALL calculate_payroll(1, 'Dec-2024');
SELECT * FROM payroll;
```

------------------------------------------------------------------------


## 🎯 Learning Outcomes

By completing this project, you master:

✔ Database Design\
✔ Real HR payroll logic\
✔ SQL joins & data relationships\
✔ Stored procedures & triggers\
✔ Views for reporting\
✔ Automating business logic

------------------------------------------------------------------------

## 👨‍💻 Author

**Your Name (replace here)**\
Data Analyst \| SQL Developer\
LinkedIn: *Add your profile link*

------------------------------------------------------------------------

## ⭐ Support

If you like this project, please ⭐ star the repository!\
It helps you grow in GitHub search rankings.
