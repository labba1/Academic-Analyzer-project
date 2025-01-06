# Academic Study Performance Analyser 
Prepared by: SWEG Section A (2017/25)

■ Table of Contents

1. [Introduction](#introduction)
2. [What This Program Does](#what-this-program-does)
3. [Key Features](#key-features)
4. [Getting Started](#getting-started)
   - [What You Need](#what-you-need)
   - [Installing and Running the Program](#installing-and-running-the-program)
5. [How to Use the Program](#how-to-use-the-program)
   - [Step-by-Step Instructions](#step-by-step-instructions)
6. [Example Input and Output](#example-input-and-output)
7. [Contributing](#contributing)
8. [Credits](#credits)

## Introduction

Are you a student wanting to easily track your study hours and see your study pattern during the week? The Academic Study Performance Analyzer is a C++ program designed to assist second-year Software Engineering students in tracking their daily study hours leading up to final exams. By recording study hours each day, students can better organize their study schedules.

Students often record their daily study time in notebooks but struggle to summarize and analyze this data. This program allows students to input their study hours for each day of the week and generates a report showing the study hours for each day, the total weekly study hours, and the average study hours per day.

## What This Program Does

Have you ever written down your study hours in a notebook and then struggled to understand your overall study habits? This program helps you:

- Record your daily study hours: Enter how many hours you studied each day of the week.
- See your total study time: Find out how many hours you studied in total during the week.
- Know your average daily study time: See the average number of hours you studied per day.
- Find your data quickly: If there are many students using the program, you can easily search for your records by name or student ID.

This program is perfect for students preparing for exams or anyone who wants to keep track of their study habits.
## Key Features

Here's what this program can do:

- Data Storage: Utilizes parallel arrays to store:
  - Student names or IDs
  - Study hours for each day of the week (7 days)
- Calculations:
  - Computes total study hours for the week
  - Calculates average study hours per day
- Search Functionality: Enables searching for specific students by name or ID.
- Output: Displays results in a clear tabular format.
- Easy Input: You'll be prompted to enter your name (or student ID) and study hours for each day of the week.
- Organized Data: The program keeps track of all your data in an organized way internally.
- Clear Results: You'll see a nicely formatted table showing:
  - Your study hours for each day of the week.
  - Your total study hours for the week.
  - The average study hours per day across all students.
- Searchable: You can easily search for your study data by entering your name or student ID.
- Handles Many Students: This program can handle data for a large class without a limit on the number of students.
- ## Getting Started

### What You Need

- A Computer: You need a computer where you can run this program.
- C++ Compiler: You will need to install a C++ compiler that allows you to run the program. If you don't have this, you can find installation guides online.
- This Program's Files: You will also need the program's files that are hosted in this repository.

### Installing and Running the Program: Simple Instructions

1. Download the Code Files: On the GitHub page for this project, find the green button that says "Code". Click on it and choose the "Download ZIP" option. This will download all of the program's files.
2. Unzip the Files: Find the file that you downloaded, it will be called something like "study-performance-analyzer-main.zip" or similar, and extract its contents by unzipping it. You can do this by right-clicking the file and selecting "Extract All".
3. Open a Terminal: Open the terminal app on your computer. This might be called Command Prompt, Command Line, Terminal, or other names depending on your system.
4. Navigate to the Project Folder: In your terminal application, type the command cd followed by the path to the folder you just extracted. For example, if you have extracted the program files into a folder called study-performance-analyzer, you would type cd path/to/study-performance-analyzer.

## How to Use the Program

Once the program is running, it will ask you for some information:

1. Number of Students: The program will first ask for the number of students you are tracking the information for.
2. Student Data: For each student, the program will ask for the student name or ID, and the number of hours they studied for each day of the week (from Day 1 to Day 7).
3. Results Table: After you've entered all the student information, the program will show you a table with your data organized in a way that makes it easy to understand and see the overall weekly study patterns.
4. Search Data: After all the data has been entered, you can search for a particular student using their name or student ID.

### Step-by-Step Instructions

1. Enter the Number of Students: When the program starts, it will first ask you how many students you want to track the data for.
2. Enter Each Student's Data:
   - The program will then ask for the name or student ID of each student.
   - After that, it will ask for the study hours for each day of the week (Day 1 to Day 7) for each student.
3. See the Results Table: Once you’ve entered all the information, the program will display a table with all the data you entered, the total weekly study time for each student, and the overall daily average.
4. Search for a Student: The program will ask if you would like to search for the data of a particular student. If you answer yes, you will be prompted to enter the name or ID of the student that you are looking for.

## Example Input and Output

### Example Input

![Example Input](https://github.com/user-attachments/assets/6606ae4d-838d-4f57-a39c-0017eda6ec9c)

### Example Output

![Example Output](https://github.com/user-attachments/assets/e00b4161-570e-4fe8-97c9-5f308deb4feb)

## Contributing

If you have coding experience and want to help improve this program, here's how:

1. Get a Copy of the Code: Make a copy of this project by clicking the "Fork" button on GitHub.
2. Make Your Changes: Add new features, fix bugs, or improve the code as you like.
3. Test Your Changes: Make sure that your changes don't break the program.
4. Suggest Your Changes: Share your changes by creating a "pull request," which is a way to suggest your changes to the original project.

## Credits

Here are the contributors to the "Academic-Analyzer-project" repository along with their contributions:

Arsema Seife (@Arsema137)

Contributions: Assisted with the development of the code and readme file,also contributed to the documentation.

Aster-Teshome (@Aster-Teshome)

Contributions: Assisted with the development of the code and flow chart,also contributed to the documentation.

Beamlak Atilabachaw (@labba1)

Contributions: Project lead,contributed to the documentation and Assisted with the development of the code and read me file.

Barkot Zerihun (@BarkiZed)

Contributions: Assisted with the development of the code,read me file also the documentation and created detailed samples of the output for the users.

Abigiya Fikru (@AbigiyaFikru)

Contributions: Assisted with the development of the code,read me file and documentation, also provided quality assurance of the program.

Barkot Frew (@Barkotfrew)

Contributions:  Assisted with the development of the code,readme file and documentation,also contributed to create a sample of the user interface and experience design.

