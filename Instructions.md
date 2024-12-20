# Project: Simple Student Management System

## Overview:
Create a file-based program to manage a small database of student records. The program will allow users to add, delete, display, and search for student records. All data will be stored in a file-based system, using a simple array of structs to hold the student records.

### Student Attributes:
Each student record will include the following attributes:
 - **ID**: A unique integer identifier for the student.
 - **Name**: The student's name (string).
 - **Age**: The student's age (integer).
 - **Grade**: The student's grade (float).

### Features:
The program will implement the following features:
- **Add a new student**: Input all student details (ID, Name, Age, Grade) and store the student record.
- **Delete a student record**: Remove a student record by their unique ID.
- **Display all students**: Print all stored student records in a readable format.
- **Search for a student by ID**: Look up and display a student's record using their unique ID.

### Requirements:
The program will meet the following requirements:
- **Generate student database** from a pre-defined file, `Students.txt`.
- **Use structs** to represent student records.
- **Store up to 100 student records** in an array.
- **Input validation**:
  - Ensure no duplicate student IDs.
  - Ensure the name contains characters.
  - Ensure the age is a positive integer.
  - Ensure the grade is between 0 and 120.
- **Generate an output file**, `Output.txt`, containing the results from all operations (add, delete, search, and display) along with success or failure messages.

### Files:
The project should consist of the following files:
- **main.c**: Entry point of the program, which handles user input and output.
- **student.c**: Contains functions for handling student-specific operations (e.g., add, delete, search).
- **student.h**: Declares the struct for student records and function prototypes.
- **Students.txt**: Contains initial data with predefined student records. The format is as follows:
  - `P`: Marks the beginning of a section.
  - `A:ID:Name:Age:Grade`: A record to be added.
  - `D:ID`: A record to be deleted.
  - `S:ID`: Search for a student by ID.
- **Output.txt**: The output file will contain results from executing the operations (adding, deleting, searching students, and displaying student records).

### Expected Project Structure:
Before Execution:

```bash
Simple Student Management System (Project folder)
|___build
|   |___main.o
|   |___student.o
|___headers
|   |___student.h
|___in
|   |___Students.txt
|___out
|___src
|   |___main.c
|   |___student.c
|___Run.exe
```

After Execution:

```bash
Simple Student Management System (Project folder)
|___build
|   |___main.o
|   |___student.o
|___headers
|   |___student.h
|___in
|   |___Students.txt
|___out
|   |___Output.txt // Created Output file
|___src
|   |___main.c
|   |___student.c
|___Run.exe
```


### `Students.txt` Format:
- `P` to mark the beginning of a section.
- `A:ID:Name:Age:Grade` for adding a new student record.
- `D:ID` for deleting a student record.
- `S:ID` to search for a student by ID.

### `Output.txt` Format:
- **All Students**: Displays all student records.
- **Add/Remove Messages**: Displays success or failure when adding or deleting students.
- **Search Messages**: Displays whether a student was found or not.
