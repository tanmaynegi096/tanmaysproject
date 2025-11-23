# Student Academic Performance Tracker

## 1. Project Overview
The **Student Academic Performance Tracker** is a modular Python-based application designed to help university students manage their academic records. It allows students to input course details, credit values, and grades to automatically calculate their GPA/CGPA. 

This project addresses the problem of manual grade tracking, which is often error-prone and decentralized. The system ensures data persistence using JSON storage and provides a clean command-line interface for interaction.

## 2. Features
* **Course Management (CRUD):** Add new completed courses with specific credits and grade points.
* **Automated Calculation:** Instantly calculates weighted GPA based on input data.
* **Data Persistence:** Automatically saves all user data to a local `json` database, ensuring data is not lost when the program closes.
* **Input Validation:** Robust error handling ensures the program does not crash on invalid inputs (e.g., entering text instead of numbers).
* **Modular Architecture:** The codebase is split into distinct modules for better maintainability and readability.

## 3. Technology Stack
* **Language:** Python 3.x
* **Data Storage:** JSON (File I/O)
* **Libraries:** `json`, `os`, `sys` (Standard Library)
* **Architecture:** Modular Programming

## 4. Project Structure
The project follows a modular directory structure to separate concerns:

```text
Student-Performance-Tracker/
│
├── data/
│   └── grades.json            # Persistent database file
│
├── src/
│   ├── __init__.py            # Package initialization
│   ├── models.py              # Class definitions (Course objects)
│   ├── data_handler.py        # Handles reading/writing to JSON
│   ├── calculator.py          # Logic for GPA algorithms
│   └── input_validator.py     # Error handling utilities
│
├── main.py                    # Application Entry Point
├── requirements.txt           # Dependencies
└── README.md                  # Project Documentation
