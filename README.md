# 🏫 School Management System

A console-based Java application to manage Students and Teachers in a school. Built using Core Java following a clean **MVC (Model-View-Controller)** architecture with a Repository layer for efficient data handling.

---

## 📌 Features

- ➕ Add Student (ID, Name, Marks)
- ➕ Add Teacher (ID, Name, Subject)
- 🔍 Find Student by ID
- 🔍 Find Teacher by ID
- ❌ Delete Student by ID
- ❌ Delete Teacher by ID
- 📋 View All Students & Teachers
- 🔢 Get Total Count of Students and Teachers
- 🚫 Duplicate ID prevention

---

## 🏗️ Architecture

This project follows **MVC + Repository Pattern**:

| Layer | Class(es) | Responsibility |
|------------|---------------------------|------------------------------|
| Model | Person, Student, Teacher | Data structure |
| View | SchoolView | User interface (console) |
| Controller | SchoolController | Business logic & validation |
| Repository | StudentRepo, TeacherRepo | Data storage |

---

## 📁 Project Structure

```
SchoolManagementSystem/
├── Main.java
├── controller/
│   └── SchoolController.java
├── model/
│   ├── Person.java
│   ├── Student.java
│   └── Teacher.java
├── repository/
│   ├── StudentRepo.java
│   └── TeacherRepo.java
└── view/
    └── SchoolView.java
```

---

## 🧬 Class Overview

- 🔹 **Person** (Abstract Class) — Common fields: `id`, `name`. Defines abstract `display()`
- 🔹 **Student** — Extends Person, adds `marks`
- 🔹 **Teacher** — Extends Person, adds `subject`
- 🔹 **Repository Layer** — Array-based storage (capacity: 100), supports add/delete/search/count
- 🔹 **Controller** — Validates input, prevents duplicate IDs
- 🔹 **View** — Console UI using `Scanner`

---

## 🧠 Concepts Used

- Object-Oriented Programming (OOP)
- Inheritance & Abstraction
- Encapsulation
- MVC Architecture
- Repository Pattern
- Array-based Data Management

---

## 🚀 How to Run

### Prerequisites
- Java JDK 8 or higher
- IDE (IntelliJ / Eclipse / VS Code) or Terminal

### Steps

```bash
# Clone the repository
git clone https://github.com/Razeena-04/SchoolManagementSystem.git

# Navigate to project
cd SchoolManagementSystem

# Compile
javac -d out src/**/*.java src/Main.java

# Run
java -cp out Main
```

---

## 🖥️ Sample Output

```
-----------------School Management System-----------------
| 1. Add Student
| 2. Add Teacher
| 3. Find Student By ID
| 4. Find Teacher By ID
| 5. Delete Student By ID
| 6. Delete Teacher By ID
| 7. Get All
| 8. Get Count
| 9. Exit
Enter your choice: 1
Enter ID: 101
Enter Name: Razeena
Enter Marks: 95
Successfully added the Student: Razeena
```

---

## ⚠️ Limitations & Future Improvements

- Uses in-memory storage (data lost after exit)
- Can be extended with database (MySQL / MongoDB)
- UI can be upgraded to web or GUI (JavaFX / React)

---

## 👩‍💻 Author

**Razeena**  
B.Tech Artificial Intelligence and Data Science
