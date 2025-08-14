# Java_Project_Ahir
.

💡 Features

✅ Connects Java to MySQL using JDBC
✅ Inserts new student records
✅ Displays all student records
✅ Updates existing student records
✅ Deletes records by ID
✅ Command-line based menu system

🛠️ Requirements

Java (JDK 8 or higher)

MySQL Server

MySQL Workbench (optional)

MySQL JDBC Driver (mysql-connector-java)

IDE like IntelliJ, Eclipse, or simple command line tools

🏗️ Database Setup

Create Database

CREATE DATABASE jdbcExample;


Create Table

USE jdbcExample;

CREATE TABLE students (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    email VARCHAR(100)
);

🔌 Configuration

Update your database credentials inside the Java file:

static final String DB_URL = "jdbc:mysql://localhost:3306/jdbcExample";
static final String USER = "root";
static final String PASS = "your_mysql_password";


Make sure the MySQL JDBC driver is in your classpath.
If using Maven, add:

<dependency>
    <groupId>mysql</groupId>
    <artifactId>mysql-connector-java</artifactId>
    <version>8.0.33</version>
</dependency>

🚀 Running the Project

Compile and run the Java file:

javac JdbccrudExample.java
java JdbccrudExample


You’ll see a menu:

1. Insert
2. Display
3. Update
4. Delete
5. Exit


Choose an option and follow the prompts.

📌 Notes

Uses PreparedStatement to prevent SQL injection

Demonstrates basic JDBC best practices

Ensure the MySQL server is running before executing

✅ Example

Inserting a student:

Enter name: John
Enter email: john@example.com
Student inserted successfully.


Displaying students:

ID: 1, Name: John, Email: john@example.com

📬 Contact

Created by Radhe Ahir
📧 Email: ahirradhe2000@gmail.com
🌐 GitHub: Radhe358
