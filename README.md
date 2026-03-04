# OOP-week 1Lab 02-task 1
#include <iostream>
using namespace std;

class Student {
private:
    string name;
    int rollNumber;
    float marks;

public:
    // Function to take input from user
    void getData() {
        cout << "Enter Name: ";
        cin.ignore();          // To clear buffer
        getline(cin, name);

        cout << "Enter Roll Number: ";
        cin >> rollNumber;

        cout << "Enter Marks: ";
        cin >> marks;
    }

    // Function to display student information
    void displayData() {
        cout << "\n--- Student Information ---" << endl;
        cout << "Name: " << name << endl;
        cout << "Roll Number: " << rollNumber << endl;
        cout << "Marks: " << marks << endl;
    }
};

int main() {
    Student s1;   // Creating object

    s1.getData();     // Calling input function
    s1.displayData(); // Calling display function

    return 0;
}
