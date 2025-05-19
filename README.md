# SAP ABAP Employee Management System

<p align="center">
  <img src="./SAP_DP_Pic1.png" alt="DBMS Overview" width="600px"/>
</p>


## 🔍 Overview  
This project is a Dialog-based application developed using **SAP ABAP** for **SmartLogic** to manage employee records efficiently. It demonstrates real-world use of **SE11 tables**, **module pool programming**, **subroutines**, and **tabstrip controls** to deliver a structured and user-friendly experience within the SAP GUI environment.

## 🧱 Key Features

### 👤 User Authentication (Screen 0100)
- Login using Employee Number.
- Password format: First name + last 3 digits of EMP_NO.
- Error handling with success/failure messages.

### 📝 Employee Registration (Screen 0200)
- Form-based entry with input validation.
- Email: Minimum 8 characters, at least one digit.
- Password confirmation and EMP_NO auto-generation.
- Fields are disabled after successful registration.

### 📋 Employee Record Management (Screen 0300)
- Department filtering using F4 help (e.g., HR, IT Support).
- Table control with editable Email ID.
- Email validation and confirmation popup before saving.
- Button to access Admin Controls.

### 🛠 Admin Functions (Screen 0400)
- **Insert Tab (0401):** Add new employees with validation.
- **Delete Tab (0402):** Select and delete multiple records.
- Tabstrip for easy navigation with dynamic screen behavior.

## 🧪 Technical Architecture

- **Database Table:** `Z021EMPLOYEE`  
  Fields: EMP_NO (PK), EMP_NAME, GENDER, EMAIL_ID, DEPT.
  
- **Program Structure:**
  - `TOP`: Global data, types.
  - `O01`: PBO modules.
  - `I01`: PAI modules.
  - `F01`: Subroutines (FORM routines) for reusable logic.

- **Screens:**
  - 0100: Login  
  - 0200: Registration  
  - 0300: Employee Records (with popup 0301)  
  - 0400: Admin Functions (with subscreens 0401, 0402)

## ▶️ How to Use

1. Execute the program (e.g., `/nZ544_EMP_MANAGE`).
2. Register a new employee → Login.
3. View and manage records by department.
4. Admin users can insert or delete employee records.

## 🔮 Future Enhancements
- Role-based user access.
- Enhanced reporting features.
- Workflow integration (e.g., approvals).
- Mobile-responsive SAP GUI design.

