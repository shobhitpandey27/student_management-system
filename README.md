# Student Management System

## Project Overview

Hey everyone! This is my semester project for our **Python Essentials** course[cite: 1]. I created a simple, menu-driven **Student Management System** in Python to help keep track of student details, grades, and attendance without having to maintain manual registers[cite: 1].

The program runs directly in the terminal and lets you add, search, update, and remove student profiles[cite: 1]. You can also log subject marks, set attendance percentages, and check out class-wide stats[cite: 1]. All the records are saved automatically to a JSON file so your data stays safe even after you close the program[cite: 1].

---

## Objectives

- **Go Digital:** Replace paper registers with a quick CLI app[cite: 1].
- **Stay Organized:** Keep student records formatted and stored cleanly in one place[cite: 1].
- **Automate Calculations:** Let Python handle mark totals, percentages, and letter grades[cite: 1].
- **Track Attendance:** Monitor attendance percentages easily[cite: 1].
- **Learn by Doing:** Put foundational Python concepts (functions, file handling, loops, dictionaries) into practice[cite: 1].

---

## Core Features

### 1. Student Profile Management
- Add new student entries[cite: 1].
- View the complete list of students[cite: 1].
- Search for specific students using their Student ID[cite: 1].
- Update details or delete student entries[cite: 1].
- Automatic check to prevent duplicate Student IDs[cite: 1].

### 2. Marks & Grades
- Log and update subject marks[cite: 1].
- Automatically calculate total marks, percentage, and assigned grade[cite: 1].

### 3. Attendance Tracking
- Enter and update attendance percentages[cite: 1].
- Check individual attendance status[cite: 1].

### 4. Class Reports & Stats
- View individual student performance summaries[cite: 1].
- Check overall class statistics (average score, highest/lowest marks, topper info)[cite: 1].

---

## Tools & Tech Used

| Tool / Language | Purpose |
|---|---|
| **Python 3.9+** | Main programming language[cite: 1, 6] |
| **JSON** | Local file storage for saving data[cite: 1] |
| **unittest** | Built-in framework for unit testing[cite: 1] |
| **VS Code** | Code editor & terminal execution[cite: 1] |
| **Git & GitHub** | Version control and code backup[cite: 1] |

*Note: You don't need to install any external packages with `pip`. Everything runs using standard Python modules!*[cite: 1, 6]

---

## Project Structure

```text
Student-Management-System/
├── main.py
├── src/
│   ├── __init__.py
│   ├── menu.py
│   ├── student.py
│   ├── marks.py
│   ├── attendance.py
│   ├── reports.py
│   ├── validation.py
│   ├── file_handler.py
│   └── utils.py
├── data/
│   └── students.json
├── tests/
│   └── test_system.py
├── docs/
│   ├── PROJECT_REPORT.md
│   └── diagrams/
├── screenshots/
│   └── README.md
├── README.md
├── statement.md
├── requirements.txt
├── .gitignore
└── LICENSE
```[cite: 1]

---

## Getting Started

### Prerequisites
Make sure you have Python 3.9 or higher installed on your system[cite: 1, 6]:

```bash
python --version
```[cite: 1]

### Running the App
1. Open the project folder in VS Code or open your terminal inside the directory[cite: 1].
2. Run the program using:

```bash
python main.py
```[cite: 1]

---

## Application Menu

```text
========================================
       STUDENT MANAGEMENT SYSTEM
========================================

1. Add Student
2. View All Students
3. Search Student
4. Update Student
5. Delete Student
6. Add/Update Marks
7. Set Attendance
8. Generate Student Report
9. Class Statistics
0. Exit
```[cite: 1]

---

## How Data is Stored

Instead of setting up a heavy database, I used a lightweight JSON file located at `data/students.json`[cite: 1]. It’s easy to inspect and edit if needed[cite: 1].

Sample record structure:
```json
{
    "S101": {
        "name": "Rahul Sharma",
        "age": 18,
        "branch": "CSE",
        "semester": 1,
        "marks": {
            "Python": 85,
            "C++": 78
        },
        "attendance": 92
    }
}
```[cite: 1]

---

## Input Validation

I added input checks to make sure the program doesn't crash on bad inputs[cite: 1]:
- Student ID cannot be left blank or duplicated[cite: 1].
- Marks and Attendance values must strictly be numbers between 0 and 100[cite: 1].
- Age and Semester inputs must be valid positive integers[cite: 1].

---

## Grade Criteria

| Percentage Range | Grade |
|---|---|
| 90% – 100% | **A+** |
| 80% – 89% | **A** |
| 70% – 79% | **B** |
| 60% – 69% | **C** |
| 50% – 59% | **D** |
| Below 50% | **F** |

[cite: 1]

---

## Running Unit Tests

To test if the core logic works properly[cite: 1]:

```bash
python -m unittest discover -s tests
```[cite: 1]

---

## Future Scope

Some features I want to add in future semesters[cite: 1]:
- Desktop GUI layout using Tkinter[cite: 1].
- Database migration to SQLite or MySQL[cite: 1].
- User authentication (Admin vs Student login)[cite: 1].
- Exporting grade cards to PDF/Excel format[cite: 1].
- Performance analytics graphs using Matplotlib[cite: 1].

---

## Lessons Learned

Building this project gave me hands-on experience with[cite: 1]:
- Loops, functions, and dictionary operations in Python[cite: 1].
- Reading and writing JSON files using standard file handling[cite: 1].
- Handling exceptions with `try-except` blocks[cite: 1, 2].
- Structuring code cleanly into separate modules[cite: 1].
- Basic automated testing and Git commands[cite: 1].

---

**Author:** Shobhit Pandey  
**Course:** B.Tech CSE (1st Year)  
**College:** VIT Bhopal University  
**License:** MIT License[cite: 1, 5]