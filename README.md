# Student Management System

## Project Overview

The **Student Management System** is a Python-based console application developed for managing student information in a simple and organized way.

The project allows the user to add, view, search, update, and delete student records. It also includes options for managing marks and attendance and generating basic academic reports.

Student information is stored in a JSON file, so the data is saved even after the program is closed.

This project was created as part of the **Python Essentials** course to apply Python concepts in a practical project.

## Objectives

- To manage student information digitally.
- To store student records in an organized format.
- To reduce manual work involved in maintaining student records.
- To calculate marks, percentage, and grades automatically.
- To manage student attendance.
- To generate simple academic reports.
- To practice Python programming and project development.

## Features

### Student Management
- Add a new student
- View all students
- Search for a student
- Update student information
- Delete a student
- Prevent duplicate student IDs

### Marks Management
- Add marks for subjects
- Update marks
- Calculate total marks
- Calculate percentage
- Calculate grade

### Attendance Management
- Add attendance percentage
- Update attendance
- Check attendance status

### Reports and Statistics
- Individual student reports
- Class average
- Highest percentage
- Lowest percentage
- Topper information

### Data Storage

Student information is stored in:

```text
data/students.json
```

## Technologies Used

| Technology | Purpose |
|---|---|
| Python | Main programming language |
| JSON | Storing student data |
| unittest | Testing |
| VS Code | Development |
| Git | Version control |
| GitHub | Repository and project hosting |

No external Python packages are required.

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
```

## Requirements

Python **3.9 or later** is recommended.

Check your Python version:

```bash
python --version
```

The project uses only Python standard libraries.

## How to Run

Open the project folder in VS Code and open the terminal.

Run:

```bash
python main.py
```

## Main Menu

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
```

## Data Storage

The project uses a JSON file instead of a database.

File location:

```text
data/students.json
```

Example:

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
```

JSON was used because it is easy to read and suitable for a small project.

## Input Validation

The project checks user input before storing it.

Examples:

- Student ID cannot be empty.
- Duplicate student IDs are not allowed.
- Marks must be between 0 and 100.
- Attendance must be between 0 and 100.
- Age and semester must contain valid values.
- Student names are checked before being stored.

## Grade System

| Percentage | Grade |
|---|---|
| 90–100 | A+ |
| 80–89 | A |
| 70–79 | B |
| 60–69 | C |
| 50–59 | D |
| Below 50 | F |

## Testing

Tests are included in:

```text
tests/test_system.py
```

Run the tests using:

```bash
python -m unittest discover -s tests
```

The tests cover adding, updating and deleting students, duplicate IDs, marks, grades, attendance, and helper functions.

## Project Documentation

Additional documentation is available in the `docs` folder.

It includes:

- Project report
- System architecture
- Workflow
- Use-case diagram
- Sequence diagram
- Component diagram
- Data/storage design

The project statement and scope are available in:

```text
statement.md
```

## Screenshots

Screenshots of the running application can be added to:

```text
screenshots/
```

Recommended screenshots include the main menu, student records, marks, attendance, reports, class statistics, and test results.

## Non-Functional Requirements

### Performance
The application should perform normal operations quickly for a small or medium-sized student dataset.

### Usability
The menu-based interface is simple and easy to use from the terminal.

### Reliability
Student data is stored in a JSON file so it can be loaded again when the program is restarted.

### Maintainability
The program is divided into multiple modules, making it easier to understand and modify.

### Error Handling
The program validates user input and handles common invalid inputs without unnecessarily terminating.

### Resource Efficiency
The project uses lightweight JSON storage and Python standard libraries.

## GitHub and Version Control

Git is used to track changes in the project.

After making changes:

```bash
git add .
git commit -m "Updated Student Management System"
git push
```

## Future Improvements

Some features that could be added later are:

- Graphical interface using Tkinter
- SQLite or MySQL database
- Login and authentication
- Admin and student accounts
- PDF report generation
- Excel export
- Student performance graphs
- Subject-wise analysis
- Web-based version

## Learning Outcomes

While developing this project, I practiced:

- Variables and data types
- Conditional statements
- Loops
- Functions
- Lists and dictionaries
- Modules
- File handling
- JSON
- Input validation
- Exception handling
- Unit testing
- Git and GitHub
- Project organization

## Conclusion

The Student Management System is a simple Python project designed to manage student information, marks, attendance, and reports.

The project helped me understand how different Python concepts can be combined to create a complete application. It also gave me practical experience with file handling, modular programming, testing, and GitHub.

## Author

**Name:** Shobhit Pandey  
**Course:** B.Tech CSE  
**Year:** 1st Year  
**College:** VIT Bhopal University

## License

This project is licensed under the **MIT License**. See the `LICENSE` file for more information.
