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
