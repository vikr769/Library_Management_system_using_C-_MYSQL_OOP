# 📚 Library Management System (C++ + MySQL)

A console-based **Library Management System** built using **C++**, **OOP (Object-Oriented Programming)**, and **MySQL** for backend database operations. This project allows **Admins** to manage books and students, and allows **Students** to borrow books from the library.

---

## 🚀 Features

- 👨‍💼 Admin can:
  - Add new books to the library
  - Register new students

- 👩‍🎓 Students can:
  - View all available books
  - Borrow books (if available)

- 🗃️ Data is stored in a **MySQL database**
- 🔗 Database connectivity is handled using the **MySQL C API**

---

## 🛠️ Technologies Used

- 💻 C++ (Dev C++ or any compatible IDE)
- 🧠 OOP Principles (Classes: `Student`, `Library`)
- 🗄️ MySQL Server 8.0
- 🧩 MySQL C API (`mysql.h`, `mysqld_error.h`)
- 🪟 Windows OS (`windows.h` used for system commands)

---

## 📁 Database Setup

Create a MySQL database called `mydb` and run the following SQL scripts:

```sql
CREATE TABLE lib (
    Name VARCHAR(100) NOT NULL,
    Quantity INT,
    PRIMARY KEY (Name)
);

CREATE TABLE student (
    Id VARCHAR(100) NOT NULL,
    PRIMARY KEY (Id)
);


##🔌 How to Connect C++ with MySQL (Dev C++ Setup)
Open your project in Dev C++

Go to: Project → Project Options

➤ Directories Tab
Library Directories:

vbnet
Copy
Edit
C:\Program Files\MySQL\MySQL Server 8.0\lib
Include Directories:

pgsql
Copy
Edit
C:\Program Files\MySQL\MySQL Server 8.0\include
C:\Program Files\MySQL\MySQL Server 8.0\include\mysql
➤ Parameters Tab
Under Linker, add:

diff
Copy
Edit
-lmysql
Save and rebuild your project.

🧪 Sample Output
markdown
Copy
Edit
Welcome To Library Management System

1. Administration.
2. User.
0. Exit.

Enter Choice:
