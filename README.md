# Employee Management System

## Description
The **Employee Management System** is a Java-based application designed to manage employee information, authentication, and administrative operations in an organization. It enables managers to add, update, and remove employees, as well as define roles and validate user input. The project includes various classes for managing authentication, input validation, and sorting algorithms.

## Features
- User authentication system (Managers and Regular Employees)
- Secure login with password validation
- Employee profile management (update name, surname, role, email, etc.)
- Manager functionalities:
  - Hire and fire employees
  - Assign and delete roles
  - View all employees and their details
- Regular employee functionalities:
  - Update personal profile
  - Change password upon first login
- Sorting algorithms implementation for employee data
- Secure database connection with MySQL

## Technologies Used
- **Java** (Core application logic)
- **MySQL** (Database for storing employee details)
- **JDBC** (Java Database Connectivity for database operations)
- **GitHub** (Version control and collaboration)

## Project Structure
```
├── src
│   ├── Main.java                # Main class for application execution
│   ├── Authentication.java      # Handles user login authentication
│   ├── Database.java            # Handles database connection and queries
│   ├── Employee.java            # Abstract class for employee data management
│   ├── Manager.java             # Class for Manager-specific operations
│   ├── RegularEmployee.java     # Class for Regular Employee operations
│   ├── InputValidation.java     # Handles various input validation processes
│   ├── SortingAlgorithms.java   # Implements various sorting algorithms
│   ├── ascii-art.txt            # ASCII art displayed at application startup
│   ├── mysql-connector-j-9.1.0.jar # MySQL JDBC Driver
├── Database
│   ├── firmms_employees.sql     # SQL script for creating employee table
│   ├── firmms_roles.sql         # SQL script for creating roles table
├── README.md                    # Documentation for the project
```

## Setup Instructions
### 1. Clone the Repository
```sh
git clone https://github.com/yarenbulut/employee-management-system.git
cd employee-management-system
```

### 2. Configure Database
1. Ensure MySQL is installed and running.
2. Create a database named `firmms`.
3. Run the provided SQL scripts (`firmms_employees.sql` and `firmms_roles.sql`) to set up the database structure.
4. Update `DATABASE_URL`, `USERNAME`, and `PASSWORD` in `Database.java` according to your MySQL configuration.

### 3. Compile and Run
```sh
javac Main.java
java -cp ".;mysql-connector-j-9.1.0.jar" Main
```

## Usage
1. **Login**: Enter your username and password.
2. **Manager Operations**:
   - View all employees
   - Hire and fire employees
   - Assign and manage roles
3. **Regular Employee Operations**:
   - View and update profile
   - Change password upon first login

## Sorting Algorithms Implemented
- **Radix Sort**
- **Shell Sort**
- **Heap Sort**
- **Insertion Sort**
- **Java Collections Sort**

## Contributors
- **Hatice Yaren Bulut** 
- **Barış Can Aslan**
- **Figen Demir**
- **Çağla Hepyükselenler**

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

## Contact
For any questions, reach out via [GitHub Issues](https://github.com/yarenbulut/employee-management-system/issues).
