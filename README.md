# cgpa-calculator


#include <iostream>
using namespace std;

int main() {
    int n;
    float marks, total = 0, cgpa;

    cout << "Enter number of subjects: ";
    cin >> n;

    for (int i = 1; i <= n; i++) {
        cout << "Enter marks of subject " << i << " (out of 100): ";
        cin >> marks;
        total = total + marks;
    }

    float percentage = total / n;
    cgpa = percentage / 9.5;

    cout << "Percentage = " << percentage << "%" << endl;
    cout << "CGPA = " << cgpa << endl;

    return 0;
}
