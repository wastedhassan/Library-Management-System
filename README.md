# 🏛️ Advanced Library Management System – Java OOP + DSA + GUI

A fully-featured **Library Management System** built from scratch in Java, showcasing **Object-Oriented Programming**, **Data Structures & Algorithms**, and **Swing GUI**. Designed for performance, scalability, and real-world usability.

---

## ✨ Features

- **✅ Full OOP Implementation**  
  Encapsulation, Inheritance, Polymorphism, Abstraction with 10+ well-structured classes.

- **✅ Role-Based Access Control**  
  Separate interfaces for **Admin**, **Teacher**, and **Student** with customized menus.

- **✅ High-Performance Data Management**  
  Uses `HashMap` for **O(1) lookups** (ISBN→Book, UserID→User) and dual hash maps for real-time borrow tracking.

- **✅ Persistent Storage**  
  File I/O for books, users, and borrow records with `.txt`-based persistence.

- **✅ Input Validation & Custom Exceptions**  
  Robust validation with custom exceptions like `BookNotAvailableException`.

- **✅ Dual Interface**  
  **Console-based** and **Swing GUI** versions included – switch between them seamlessly.

- **✅ Efficient Borrow System**  
  Tracks active borrows using `HashMap<User, ArrayList<BorrowRecord>>` and `HashMap<Book, BorrowRecord>`.

---

## 🗂️ Project Structure
src/
├── Book/ # Abstract Book + PhysicalBook, EBook, PlayBook
├── User/ # Abstract User + Student, Teacher, Administrator
├── Library/ # Core system with HashMap-based management
├── Utilities/ # BorrowRecord, Validator, custom exceptions
├── FileHandling/ # FileManager for save/load operations
├── GUI/ # Swing-based interface (Login, Dashboard, Search, etc.)
└── Main/ # Console & GUI entry points

text

---

## 🚀 Getting Started

### Prerequisites
- Java JDK 8 or later
- Any Java IDE (IntelliJ IDEA, Eclipse, VS Code) or command line

### Running the Console Version
```bash
javac -d out src/**/*.java
java -cp out Main
