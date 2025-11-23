# Project Statement: Student Academic Performance Tracker

## 1. Problem Statement
University students often struggle to maintain a centralized and accurate record of their academic performance across multiple semesters. 

The manual calculation of Weighted Grade Point Average (GPA) and Cumulative GPA (CGPA) is time-consuming and prone to human error, specifically when dealing with varying credit weights for different courses. Furthermore, students lack a simple, offline tool to quickly simulate how future grades might impact their overall academic standing.

## 2. Scope of the Project
The scope of this project is to develop a desktop-based Command Line Interface (CLI) application using Python.

**In Scope:**
* **Data Entry System:** A module to input course names, credit values, and obtained grade points.
* **Calculation Engine:** Algorithms to compute the weighted average (GPA) based on user input.
* **Local Storage:** Implementation of a file-handling system (JSON) to store student records permanently on the local machine.
* **Error Management:** A validation layer to handle incorrect user inputs (e.g., negative credits or non-numeric grades).

**Out of Scope:**
* Integration with external university servers or APIs.
* Multi-user authentication (currently designed for a single-user local environment).
* Mobile application interface.

## 3. Target Users
* **University Students:** The primary users who need to track their grades and monitor their academic progress semester by semester.
* **Academic Counselors:** Users who may wish to help students calculate potential outcomes for upcoming exams.

## 4. High-Level Features
1.  **Course Management:**
    * Ability to add new completed courses to the academic record.
    * Ability to view a list of all stored courses.

2.  **Automated Analytics:**
    * Instant calculation of GPA based on the formula: `Sum(Credits * GradePoint) / Sum(Credits)`.
    * Dynamic updates whenever a new course is added.

3.  **Data Persistence:**
    * Automatic saving of data to a structured JSON file.
    * Automatic loading of previous data upon application startup.

4.  **Robust Input Validation:**
    * Protects the system from crashing if the user enters text instead of numbers.
    * Ensures grade points and credits are within logical positive ranges.
