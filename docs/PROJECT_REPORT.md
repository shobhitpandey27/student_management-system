# Student Management System
## Project Report

### 1. Cover Page

**Project Title:** Student Management System  
**Course:** Python Essentials  
**Student Name:** Replace with your name  
**Registration Number:** Replace with your registration number  
**Institution:** VIT Bhopal University  
**Academic Year:** 2026–2027

---

## 2. Introduction

Student record management is an important activity in educational institutions. Information such as student details, marks, attendance, and academic performance needs to be stored and accessed regularly.

The Student Management System developed in this project is a console-based Python application that provides a structured method for managing student records. The project demonstrates core Python concepts such as functions, modules, dictionaries, loops, conditional statements, file handling, JSON, exception-aware programming, and testing.

---

## 3. Problem Statement

Manual management of student information can be slow and error-prone. Searching paper records, updating marks, calculating percentages, and tracking attendance manually may cause duplication, calculation mistakes, and difficulty in maintaining consistent records.

The project solves this problem by providing a Python-based system that stores student information digitally and supports CRUD operations, academic management, attendance, and reporting.

---

## 4. Objectives

- Build a menu-driven Python application.
- Manage student records using CRUD operations.
- Store data permanently using JSON.
- Manage marks and attendance.
- Calculate percentages and grades automatically.
- Generate student reports and class statistics.
- Validate user input.
- Organize the application using multiple Python modules.
- Apply Git and GitHub for version control.

---

## 5. Functional Requirements

### 5.1 Student Management
- Add student
- View students
- Search student
- Update student
- Delete student

### 5.2 Marks Management
- Add marks
- Update marks
- Calculate total
- Calculate percentage
- Calculate grade

### 5.3 Attendance Management
- Store attendance percentage
- Display attendance status

### 5.4 Reports and Analytics
- Generate individual reports
- Calculate class average
- Find highest and lowest percentage
- Display topper

### 5.5 Data Storage
- Store student records in JSON
- Load saved records when the program starts
- Save changes automatically

---

## 6. Non-Functional Requirements

### Performance
The program should perform student operations quickly for small and medium datasets.

### Usability
The program should provide a simple menu-driven interface.

### Reliability
Student data should remain stored after the program closes.

### Maintainability
The system should use separate modules for different responsibilities.

### Error Handling
Invalid IDs, ages, marks, attendance values, and menu choices should be detected.

---

## 7. System Architecture

The application follows a modular architecture:

- `main.py` starts the program.
- `menu.py` handles user interaction.
- `student.py` handles student CRUD operations.
- `marks.py` handles marks and grades.
- `attendance.py` handles attendance.
- `reports.py` generates reports and analytics.
- `validation.py` validates inputs.
- `file_handler.py` handles JSON storage.
- `utils.py` contains reusable display functions.

See `docs/diagrams/architecture.md`.

---

## 8. Design Diagrams

The repository includes:

- Use Case Diagram
- Workflow Diagram
- Sequence Diagram
- Component Diagram
- Storage / ER Diagram
- System Architecture Diagram

All diagrams are stored in `docs/diagrams/`.

---

## 9. Design Decisions and Rationale

### JSON Storage
JSON was selected because it is simple, human-readable, built into Python, and suitable for a beginner-level project.

### Modular Design
Each major responsibility is placed in a separate file. This improves readability, debugging, maintainability, and testing.

### Student ID as Key
Student ID is used as the unique key in the JSON structure, which makes searching records straightforward.

### Console Interface
A console interface was chosen because the course focuses on Python fundamentals rather than GUI or web development.

---

## 10. Implementation Details

### Student Management
CRUD operations are implemented in `student.py`.

### Academic Calculations
Marks are stored subject-wise. Percentage is calculated as the average of subject marks. Grade is generated from the percentage.

### Attendance
Attendance is stored as a percentage. Students with 75% or higher are shown as eligible.

### Validation
Validation functions ensure that entered values are meaningful and within acceptable ranges.

### File Handling
`file_handler.py` reads and writes `data/students.json`.

---

## 11. Screenshots / Results

Add screenshots before final submission:

1. Main menu
2. Add student operation
3. View students
4. Search result
5. Marks entry
6. Attendance entry
7. Student report
8. Class statistics

Store screenshots in the `screenshots/` folder.

---

## 12. Testing Approach

The project uses Python's built-in `unittest` framework.

Tests cover:

- Adding a student
- Rejecting duplicate student IDs
- Updating a student
- Deleting a student
- Marks and percentage calculation
- Grade generation
- Attendance status
- Helper calculation functions

Run tests using:

```bash
python -m unittest discover -s tests
```

---

## 13. Challenges Faced

- Organizing the project into multiple modules
- Maintaining data between program runs
- Validating different types of input
- Avoiding duplicate student IDs
- Calculating reports from stored marks
- Writing isolated tests without modifying real project data

---

## 14. Learnings and Key Takeaways

This project helped in understanding:

- Python functions and modules
- Dictionaries and nested data
- File handling
- JSON serialization
- Conditional statements and loops
- Input validation
- Code organization
- CRUD operations
- Unit testing
- Git and GitHub workflow

---

## 15. Future Enhancements

- GUI using Tkinter
- SQLite or MySQL database
- Login and role-based access
- CSV/PDF report export
- Fee management
- Course registration
- Web dashboard
- Cloud database
- REST API

---

## 16. References

- Python official documentation
- Git documentation
- GitHub documentation
- Course notes and Python Essentials learning material
