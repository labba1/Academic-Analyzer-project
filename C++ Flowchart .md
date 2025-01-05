### Problem Analysis
#### Input

**User Choices:**

 1. Option to add a student.
 2. Option to view total study hours    and averages.
 3. Option to search for a student by name or code.
 
**Student Inputs:**

 1. Student name and code.
 2. Daily study hours for a week.
 
#### Output

**Display Messages:**

 1. Welcome messages based on the number of students.
 2. Total study hours and averages for all students.
 3. Details of a specific student if found.
 4. Messages for invalid choices or when no students are added.

 **Reports:**

 1. Total weekly study hours.
 2. Average daily study hours.
 3. Breakdown of study hours for each day.
 
#### Operations

**Adding Students:**

 1. Input student name and code.
 2. Input daily study hours.
 3. Calculate totals and averages.
    
**Viewing Data:**

 1. Check if there are students added.
 2. Display study hours and averages.
 3. Print a list of all students.
    
**Searching for Students:**

 1. Input search criteria.
 2. Search and display details if the student is found.


### Flow Chart
```mermaid
flowchart TB
    A[Start] --> B[Initialize Variables]
    B --> C{numStudents == 0?}
    C -->|Yes| D[Display Welcome Message and Add Student Option]
    C -->|No| E[Display Welcome Message with All Options]
    
    D --> F[Enter User Choice]
    E --> F
    
    F --> G{User Choice}
    
    G -->|1| H[Enter Student Name and Code]
    H --> I[Enter Study Hours for Each Day]
    I --> J[Calculate Totals and Averages]
    J --> K[Increment numStudents]
    K --> F
    
    G -->|2| L{numStudents == 0?}
    L -->|Yes| M[Display Please add students first.]
    L -->|No| N[Display Total Study Hours and Averages]
    N --> O[Print Student List]
    O --> F
    
    G -->|3| P{numStudents == 0?}
    P -->|Yes| Q[Display Please add students first.]
    P -->|No| R[Search by Name or Code]
    R --> S[Enter Search Criteria]
    S --> T[Search for Student]
    T --> U{Student Found?}
    U -->|Yes| V[Display Student Details and Study Hours]
    U -->|No| W[Display Student not found.]
    V --> F
    W --> F
    
    G -->|4| X[Display Good Bye!]
    X --> Y[End]
    
    G -->|Other| Z[Display Invalid choice. Please try again.]
    Z --> F
```
