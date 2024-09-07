# SwingLoginSystem
# Java Login and Signup System

This is a simple Java-based login and signup system with a graphical user interface (GUI) built using Swing. It allows users to sign up by entering a username and password, which are stored in a MySQL database. Users can then log in using their credentials.

## Features
- **Login Page**: Users can enter their username and password to log in.
- **Signup Page**: New users can sign up, and their information is saved in a MySQL database.
- **GUI**: The project uses Java Swing for the graphical user interface.

## Prerequisites

1. Java Development Kit (JDK) installed on your system.
2. MySQL database setup with the `test` schema and `details` table.
3. The following MySQL driver library: `mysql-connector-java`.

## Database Setup

Before running the program, ensure the following:

1. **Install MySQL**: Make sure MySQL is installed and running on your system.
2. **Create Database and Table**:
   - Open your MySQL command-line or any SQL client.
   - Create the `test` database:
     ```sql
     CREATE DATABASE test;
     ```
   - Create the `details` table within the `test` database:
     ```sql
     CREATE TABLE details (
       id INT AUTO_INCREMENT PRIMARY KEY,
       username VARCHAR(50),
       password VARCHAR(50)
     );
     ```

## Project Structure


## How to Run

1. **Clone the repository** or download the source code.
   
2. **Configure MySQL**:
   - Modify the connection details in `javapr.java`:
     ```java
     Connection con = DriverManager.getConnection("jdbc:mysql://localhost:3306/test", "root", "root");
     ```
   - Replace `"root"` and `"root"` with your MySQL username and password.

3. **Compile and Run the Code**:
   - Open a terminal or command prompt.
   - Navigate to the project directory.
   - Compile the Java file:
     ```bash
     javac javapr.java
     ```
   - Run the Java application:
     ```bash
     java javapr
     ```

4. The login window will appear. If you're a new user, click "SIGN UP" to register and save your credentials. After registering, you can log in with your username and password.

## Libraries Used

- **Java Swing**: For creating the graphical user interface.
- **MySQL Connector**: To connect the Java application to the MySQL database. Ensure that you have added the MySQL connector JAR to your classpath.

## Issues

If you encounter any issues, ensure:
- The MySQL database is running and the credentials are correct.
- The `mysql-connector-java` JAR is included in your classpath.

## License

This project is open-source and available under the [MIT License](LICENSE).
