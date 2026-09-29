# Student Record & Performance Management System

A console-based **Student Record Management System** built entirely with Python
dictionaries, submitted as a VITyarthi "Build Your Own Project" for the
**Python Essentials** course.

## Overview

The system lets a user (e.g. a class teacher or coordinator) maintain student
academic records — Registration Number, Name, Phone Number, Date of Birth, and
Semester Marks (out of 200) — entirely in memory, using a dictionary of
dictionaries keyed by Registration Number. It also computes class-wide
performance statistics on demand.

This project is intentionally scoped to use **only Python dictionaries** for
data storage, with no external files, databases, or third-party libraries, to
stay aligned with the topics covered in the course syllabus.

## Features

- **Add New Student Record** — add a student with full input validation
  (rejects duplicate Registration Numbers, empty fields, and non-numeric or
  out-of-range marks).
- **Display All Records** — view every stored record in a formatted table,
  sorted by Registration Number.
- **Edit Existing Student Record** — update any field of an existing record;
  leaving a prompt blank keeps that field's current value.
- **View Class Statistical Summary** — see the total number of students, the
  class average score, and the highest- and lowest-scoring students.
- **Menu-driven navigation** — a simple numbered menu (1–5) loops until the
  user chooses to exit.

## Technologies / Tools Used

- **Language:** Python 3 (standard library only, no third-party packages)
- **Data structure:** nested `dict` (dictionary of dictionaries)
- **Interface:** command-line / console

## Steps to Install & Run

1. Make sure Python 3 is installed:
   ```bash
   python3 --version
   ```
2. Clone this repository:
   ```bash
   git clone <your-repo-url>
   cd <your-repo-folder>
   ```
3. Run the program:
   ```bash
   python3 Main.py
   ```
4. Use the on-screen menu (options 1–5) to add, view, edit, or analyse
   student records. Choose option 5 to exit.

> **Note:** Records are held in memory only for the duration of one run. This
> is a deliberate scope decision (see the project report) to stay aligned
> with the dictionary-only concepts taught in the course — data is not saved
> to a file or database, so it resets each time the program is restarted.

## Instructions for Testing

The program was tested manually by running it and exercising every menu
option with both valid and invalid input. Suggested test flow:

1. Run `python3 Main.py` and choose **1** to add two or three student
   records with valid data.
2. Choose **1** again and try a duplicate Registration Number, an empty
   name, and an out-of-range marks value (e.g. `300`) to confirm each is
   rejected with a clear message.
3. Choose **2** to confirm all added records display correctly, sorted by
   Registration Number.
4. Choose **3** to edit one record — try an unknown Registration Number
   first (should show "not found"), then a valid one, updating only one
   field and leaving the others blank (should keep the old values).
5. Choose **4** to view the class statistical summary and confirm the
   average, highest, and lowest scores are correct.
6. Choose **5** to exit.

Full screenshots of this test flow are included in the project report
(`VITyarthi_Project_Report_Chitransh_Pandey.pdf`).

## Screenshots

See the project report PDF for annotated screenshots of every module in
action, including validation behaviour.

## Author

**Chitransh Pandey**
Vellore Institute of Technology, Bhopal
Registration No.: 26BCE10832
Course: Python Essentials
