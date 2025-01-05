#include <iostream>
#include <iomanip>

using namespace std;

const int MAX_STUDENTS = 100;
const int DAYS_IN_WEEK = 7;

int main() {
    string students[MAX_STUDENTS];
    int studentCodes[MAX_STUDENTS];
    int studyHours[MAX_STUDENTS][DAYS_IN_WEEK];
    int totals[MAX_STUDENTS];
    double averages[MAX_STUDENTS];
    int numStudents = 0;
    int totalSum = 0;

    while (true) {
        if (numStudents == 0) {
            cout << "Welcome to the Student Study Hours Tracker!" << endl;
            cout << "1. Add Student" << endl;
            cout << "3. Exit" << endl;
        } else {
            cout << "Welcome to the Student Study Hours Tracker!" << endl;
            cout << "1. Add Student" << endl;
            cout << "2. See Results" << endl;
            cout << "3. Search Student" << endl;
            cout << "4. Delete Student" << endl;
            cout << "5. Edit Student Hours" << endl;
            cout << "6. Exit" << endl;
        }
     int choice;
        cout << "Enter your choice: ";
        cin >> choice;

        switch (choice) {
            case 1: {
                cout << "Enter student name: ";
                cin >> students[numStudents];
                cout << "Enter student code: ";
                cin >> studentCodes[numStudents];

                for (int j = 0; j < DAYS_IN_WEEK; ++j) {
                    int hours;
                    do {
                        cout << "Enter study hours for day " << j + 1 << " (<=24): ";
                        cin >> hours;
                    } while (hours < 0 || hours > 24);
                    studyHours[numStudents][j] = hours;
                }

                totals[numStudents] = 0;
                for (int j = 0; j < DAYS_IN_WEEK; ++j) {
                    totals[numStudents] += studyHours[numStudents][j];
                    totalSum += studyHours[numStudents][j];
                }
                averages[numStudents] = static_cast<double>(totals[numStudents]) / DAYS_IN_WEEK;
                numStudents++;
                break;
            }

            case 2: {
                if (numStudents == 0) {
                    cout << "Please add students first." << endl;
                    break;
                }

                cout << "Total Study Hours for All Students: " << totalSum << endl;
                cout << "Overall Average Study Hours per Day: " << (double)totalSum / (numStudents * DAYS_IN_WEEK) << endl;
                cout << "-------------------------------------------------------------------------------------------" << endl;
                cout << "| Stud. Name  | Stud.Code |  Mon |  Tue |   Wed |  Thu | Fri | Sat  |  Sun  |  Tot |  Avg |" << endl;
                cout << "-------------------------------------------------------------------------------------------" << endl;
                for (int i = 0; i < numStudents; ++i) {
                    cout << "| " << setw(11) << left << students[i] << " | " << setw(10) << right << studentCodes[i];
                    for (int j = 0; j < DAYS_IN_WEEK; ++j) {
                        cout << " | " << setw(4) << right << studyHours[i][j];
                    }
                    cout << " | " << setw(4) << right << totals[i] << " | " << setw(4) << fixed << setprecision(2) << right << averages[i] << " |" << endl;
                }
                cout << "-------------------------------------------------------------------------------------------" << endl;
                break;
            }

            case 3: {
                if (numStudents == 0) {
                    cout << "Please add students first." << endl;
                    break;
                } 
               string searchName;
                int searchCode;
                cout << "1. Search by name" << endl;
                cout << "2. Search by code" << endl;
                cout << "Enter your choice: ";
                cin >> choice;

                if (choice == 1) {
                    cout << "Enter student name: ";
                    cin >> searchName;
                } else {
                    cout << "Enter student code: ";
                    cin >> searchCode;
                }
bool found = false;
                for (int i = 0; i < numStudents; ++i) {
                    if ((students[i] == searchName) || (studentCodes[i] == searchCode)) {
                        cout << "Student: " << students[i] << " (Code: " << studentCodes[i] << ")" << endl;
                        cout << "Total study hours: " << totals[i] << endl;
                        cout << "Average study hours per day: " << averages[i] << endl;
                        cout << "---------------------" << endl;
                        cout << "| Day | Study Hours |" << endl;
                        cout << "---------------------" << endl;
                        for (int j = 0; j < DAYS_IN_WEEK; ++j) {
                            cout << "| " << setw(3) << right << j + 1 << " | " << setw(11) << right << studyHours[i][j] << " |" << endl;
                        }
                        cout << "--------------------------------------------------------" << endl;
                        found = true;
                        break;
                    }
                }
if (!found) {
                    cout << "Student not found." << endl;
                }
                break;
            }

            case 4: { // Delete Student
                if (numStudents == 0) {
                    cout << "No students to delete." << endl;
                    break;
                }

                int searchCode;
                cout << "Enter the code of the student to delete: ";
                cin >> searchCode;

                bool found = false;
                for (int i = 0; i < numStudents; ++i) {
                    if (studentCodes[i] == searchCode) {
                        found = true;

                        // Adjust total sum
                        totalSum -= totals[i];

                        // Shift students left
                        for (int j = i; j < numStudents - 1; ++j) {
                            students[j] = students[j + 1];
                            studentCodes[j] = studentCodes[j + 1];
                            totals[j] = totals[j + 1];
                            averages[j] = averages[j + 1];
                            for (int k = 0; k < DAYS_IN_WEEK; ++k) {
                                studyHours[j][k] = studyHours[j + 1][k];
                            }
                        }
   numStudents--;
                        cout << "Student deleted successfully." << endl;
                        break;
                    }
                }

                if (!found) {
                    cout << "Student with code " << searchCode << " not found." << endl;
                }
                break;
            }

            case 5: { // Edit Student Hours
                if (numStudents == 0) {
                    cout << "No students to edit." << endl;
                    break;
                }

                int searchCode;
                cout << "Enter the code of the student to edit: ";
                cin >> searchCode;

                bool found = false;
                for (int i = 0; i < numStudents; ++i) {
                    if (studentCodes[i] == searchCode) {
                        found = true;

                        cout << "Editing hours for " << students[i] << " (Code: " << studentCodes[i] << ")" << endl;

                        // Adjust total sum and recalculate totals
                        totalSum -= totals[i];
                        totals[i] = 0;

                        for (int j = 0; j < DAYS_IN_WEEK; ++j) {
                            cout << "Enter new study hours for day " << j + 1 << " (<=24): ";
                            int newHours;
                            do {
                                cin >> newHours;
                            } while (newHours < 0 || newHours > 24);

                            studyHours[i][j] = newHours;
                            totals[i] += newHours;
                            totalSum += newHours;
                        }

                        averages[i] = static_cast<double>(totals[i]) / DAYS_IN_WEEK;
                        cout << "Student hours updated successfully!" << endl;
                        break;
                    }
                }

                if (!found) {
                    cout << "Student with code " << searchCode << " not found." << endl;
                }
                break;
            }

            case 6:
                cout << "Goodbye!" << endl;
                return 0;

            default:
                cout << "Invalid choice. Please try again." << endl;
        }
    }
}

