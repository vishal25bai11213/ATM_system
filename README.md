# Student Management System

A command-line Python application for managing student records, grades, and tasks with priority-based task scheduling.

## Features

### Student Management
- Add, update, view, and delete student records
- Unique student ID generation (STU0001, STU0002, etc.)
- Roll number validation to prevent duplicates
- Automatic GPA calculation based on grades

### Grade Management
- Add multiple grades per student across different subjects
- Support for different semesters
- Automatic percentage and letter grade calculation
- Letter grade scale: A+ (90-100), A (80-89), B+ (70-79), B (60-69), C (50-59), D (40-49), F (<40)

### Task Management
- Create tasks with priority levels (high, medium, low)
- Automatic task ID generation (TSK0001, TSK0002, etc.)
- Priority-based task queue using heap data structure
- Track task status (pending/completed)
- Deadline tracking with overdue detection
- View next highest-priority pending task

### Reporting
- Class-wide statistics (total students, average GPA)
- Task summary (total tasks, pending tasks)
- Individual student reports with grades and task count

## Requirements

- Python 3.6 or higher
- No external dependencies (uses only standard library)

## Installation

1. Download the `student_management.py` file
2. Ensure Python 3.6+ is installed on your system
3. Run the program:

```bash
python student_management.py
```

## Usage

The program presents a menu-driven interface with the following options:

### Menu Options

1. **Add Student** - Create a new student record
2. **List Students** - View all students with their GPAs
3. **View Student** - Display detailed information for a specific student
4. **Update Student** - Modify student information
5. **Delete Student** - Remove a student and their associated tasks
6. **Add Grade** - Add a grade entry for a student
7. **Add Task** - Create a new task for a student
8. **View Tasks** - List all tasks (with optional status filter)
9. **Complete Task** - Mark a task as completed
10. **Delete Task** - Remove a task
11. **Next Task** - View the highest priority pending task
12. **Report** - Display system-wide statistics
13. **Exit** - Save and close the program

### Example Workflow

```
# Add a student
Choice: 1
Name: John Doe
Roll: CS001
Email: john@example.com

# Add a grade
Choice: 6
ID: STU0001
Sub: Mathematics
Mk: 85
Max: 100
Sem: Fall 2024

# Add a task
Choice: 7
Title: Complete Assignment 1
Desc: Submit math homework
Prio(high/medium/low): high
Due(YYYY-MM-DD): 2024-12-31
ID: STU0001

# View next priority task
Choice: 11
```

## Data Persistence

All data is automatically saved to `data.pkl` file using Python's pickle module. The data persists between sessions and includes:
- Student records with grades
- Task records with status

## File Structure

```
.
├── student_management.py    # Main program file
└── data.pkl                 # Auto-generated data file (created on first save)
```

## Classes Overview

### Grade
Represents a single grade entry with subject, marks, maximum marks, and semester information.

### Student
Represents a student with personal information and a collection of grades. Automatically calculates GPA.

### Task
Represents a task with priority, deadline, and status. Implements comparison for priority queue ordering.

### System
Main system class that manages students and tasks, handles data persistence, and provides all core functionality.

## Notes

- Student IDs are automatically generated and cannot be changed
- Roll numbers must be unique across all students
- Task priorities must be one of: high, medium, low
- Dates should be in YYYY-MM-DD format
- GPA is calculated on a 10-point scale
- Deleting a student automatically removes all their associated tasks

## Limitations

- Command-line interface only (no GUI)
- Single-user system (no authentication)
- Date validation is basic
- No backup/restore functionality
- No export to CSV/Excel

## Future Enhancements

- Graphical user interface
- Export reports to PDF/Excel
- Email notifications for overdue tasks
- Advanced search and filtering
- Multi-semester GPA tracking
- Attendance management

## License

This project is provided as-is for educational purposes.

## Support

For issues or questions, please refer to the code comments or modify according to your needs.