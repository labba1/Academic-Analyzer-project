Problem Analysis
Input

1.User Choices:
 • Option to add a student.
 • Option to view total study hours    and averages.
 • Option to search for a student by name or code.
2.Student Inputs:
 • Student name and code.
 • Daily study hours for a week.
 
Output

1.Display Messages:
 • Welcome messages based on the number of students.
 • Total study hours and averages for all students.
 • Details of a specific student if found.
 • Messages for invalid choices or when no students are added.
 2.Reports:
 • Total weekly study hours.
 • Average daily study hours.
 • Breakdown of study hours for each day.
 
Operations

1.Adding Students:
 • Input student name and code.
 • Input daily study hours.
 • Calculate totals and averages.
2.Viewing Data:
 • Check if there are students added.
 • Display study hours and averages.
 • Print a list of all students.
3.Searching for Students:
 • Input search criteria.
 • Search and display details if the student is found.


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
