# 🧠 Secure Quiz Platform (Java OOP Mini Project)

### 📘 Overview
The **Secure Quiz Platform** is a Java-based mini project built using **Object-Oriented Programming (OOP)** principles.  
It allows **teachers** to create and manage quizzes and **students** to attempt them in a secure environment with automatic evaluation.  
All quiz data and user details are stored safely using file-based storage.

---

## 🎯 Features

### 👨‍🏫 Teacher
- Register & login securely  
- Create quizzes (text or MCQs)  
- Add, update, and delete questions  
- View student scores and statistics  

### 👨‍🎓 Student
- Register & login  
- Attempt available quizzes (only once)  
- Get instant results after submission  

### 🔒 Security
- Encoded passwords (Base64)  
- Role-based access (Teacher/Student)  
- Random question order for fairness  
- Single attempt rule per quiz  

---

## ⚙️ Tech Stack

| Component | Technology |
|------------|-------------|
| **Language** | Java 17+ |
| **Paradigm** | Object-Oriented Programming |
| **Storage** | File Handling (`.txt`) |
| **Security** | Base64 Password Encoding |
| **IDE** | IntelliJ IDEA / Eclipse / VS Code |
| **UI** | Console-based (Scanner Input) |

---

## 🧩 Class Structure

| Class | Description |
|--------|--------------|
| `User` | Abstract parent class for Teacher & Student |
| `Teacher` | Manages quiz creation & results |
| `Student` | Handles quiz participation & scoring |
| `Question` | Stores individual MCQ question & options |
| `Quiz` | Holds quiz details, list of questions, and evaluation logic |
| `QuizManager` | Central class for managing quizzes & results |
| `AuthService` | Handles login, registration & password encoding |
| `Result` | Stores and displays quiz performance |
| `Main` | Entry point with menu-driven console interface |

---

## 📁 Project Structure
SecureQuizPlatform/
├── src/com/quiz/platform/
│ ├── User.java
│ ├── Teacher.java
│ ├── Student.java
│ ├── Question.java
│ ├── Quiz.java
│ ├── QuizManager.java
│ ├── AuthService.java
│ ├── Result.java
│ └── Main.java
└── data/
├── users.txt
├── quizzes.txt
└── results.txt


Sample Output
===== SECURE QUIZ PLATFORM =====
1. Login
2. Register
3. Exit
> 1

Enter Role (Teacher/Student): Student
Enter Username: madhav
Enter Password: *****

Login Successful ✅

Available Quizzes:
1. Java Basics
Enter Quiz ID: 1

Q1. What is JVM?
a) Java Virtual Machine
b) Java Vendor Module
c) Joint Vector Module
d) None
Answer: a

Quiz Completed!
Your Score: 8 / 10 (80%)
