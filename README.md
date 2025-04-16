
# Payroll Management System

## Overview

The **Payroll Management System** is a Java-based application that provides a user-friendly interface for managing employee payroll data. Built using **Swing** for the graphical user interface (GUI) and **MySQL** for the backend, this system allows users to add, view, and update employee records, calculate payrolls, and generate reports.

## Features

- **Employee Management**: Add, edit, and view employee details including personal and job-related information.
- **Payroll Calculation**: Automatically calculate the salary based on employee details, including basic salary, deductions, and allowances.
- **Data Persistence**: Store employee information in a MySQL database for easy retrieval and management.
- **Multi-step Employee Entry**: Simplified multi-step forms to add employees with all necessary details such as name, department, designation, and salary information.
- **Employee Search**: Search for employees based on various criteria.
- **Reports Generation**: Generate employee payroll reports in a structured format.
- **Photo Management**: Upload and manage employee photos as part of the profile.

## Technologies Used

- **Java**: Core programming language used for building the application.
- **Swing**: For creating the GUI (Graphical User Interface).
- **MySQL**: Database for storing employee and payroll data.
- **JDBC**: Java Database Connectivity for integrating MySQL with the Java application.

## Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/AdarshCodes1221/Payroll-Management-System.git
   ```

2. **Set up MySQL Database**:
   - Create a MySQL database.
   - Import the SQL schema from the `database/` folder into your MySQL instance.
   
3. **Configure Database Connection**:
   - Update the database connection details in the `config/DatabaseConfig.java` file:
     ```java
     public static final String DB_URL = "jdbc:mysql://localhost:3306/payroll_system";
     public static final String USER = "your-username";
     public static final String PASSWORD = "your-password";
     ```

4. **Compile and Run**:
   - Use your preferred Java IDE (IntelliJ IDEA, Eclipse, etc.) or compile from the command line:
     ```bash
     javac -d bin src/*.java
     java -cp bin Main
     ```

## Usage

1. **Start the Application**:
   Launch the application from your IDE or terminal.
   
2. **Login**:
   The system prompts for authentication (admin credentials to access the payroll management system).

3. **Manage Employees**:
   Use the system to add, update, or delete employee records. Employee information can include:
   - Name
   - Department
   - Job title
   - Salary details
   - Contact information
   
4. **Payroll Calculation**:
   After entering employee details, the system will automatically calculate the salary, considering deductions and allowances.

5. **Reports**:
   Generate employee payroll reports in CSV format or other customizable formats.

## Database Schema

### `employees` table:

| Column Name       | Type        | Description                |
|-------------------|-------------|----------------------------|
| first_name        | VARCHAR(50) | Employee's first name      |
| last_name         | VARCHAR(50) | Employee's last name       |
| date_of_birth     | DATE        | Employee's date of birth   |
| gender            | VARCHAR(10) | Employee's gender          |
| department        | VARCHAR(50) | Employee's department      |
| designation       | VARCHAR(50) | Employee's designation     |
| job_title         | VARCHAR(50) | Employee's job title       |
| status            | VARCHAR(20) | Employment status (active, inactive) |
| date_hired        | DATE        | Date of joining           |
| basic_salary      | DECIMAL(10, 2) | Basic salary of the employee |
| email             | VARCHAR(100) | Employee's email address  |
| contact           | VARCHAR(15)  | Employee's contact number |
| address_line1     | VARCHAR(255) | Employee's address (line 1) |
| address_line2     | VARCHAR(255) | Employee's address (line 2) |
| postal_code       | VARCHAR(10) | Postal code of the address |
| photo             | LONGBLOB    | Employee's photo           |

## Contributing

Contributions are welcome! If you have any suggestions or improvements, feel free to fork the repository and submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

![Screenshot 2025-04-16 221725](https://github.com/user-attachments/assets/7d2d8c44-c11c-4f4d-b48f-7219236c61af)
![Screenshot 2025-04-16 221702](https://github.com/user-attachments/assets/3450be6c-f939-4ff1-9e27-25b886e3e1ee)
![Screenshot 2025-04-16 221643](https://github.com/user-attachments/assets/db46b763-2286-4b6b-a01a-f4c97ca5b100)
![Screenshot 2025-04-16 221627](https://github.com/user-attachments/assets/52443890-802d-44a9-927b-5d3091ee5b35)
![Screenshot 2025-04-16 221611](https://github.com/user-attachments/assets/f7e60ba4-8023-4b42-9ec3-f38a2e480f5b)
![Screenshot 2025-04-16 221557](https://github.com/user-attachments/assets/2d391729-f140-4b36-b163-3d13aa17c596)
![Screenshot 2025-04-16 221541](https://github.com/user-attachments/assets/8e8460be-90c7-4284-99fd-064dc7fbf378)
![Screenshot 2025-04-16 221515](https://github.com/user-attachments/assets/492f0113-77a6-4f13-be2b-34a35ad60dec)
![Screenshot 2025-04-16 221333](https://github.com/user-attachments/assets/36559053-881e-42a5-8deb-0d0615ef1f13)
![Screenshot 2025-04-16 221249](https://github.com/user-attachments/assets/07b54eda-04e1-49f1-8e32-d75c5090c644)
