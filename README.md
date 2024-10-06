#include <iostream>
using namespace std;

int main() {
    double num1, num2;
    char operation;

    // Display available operations
    cout << "Enter an operation (+, -, *, /): ";
    cin >> operation;

    // Take two numbers as input
    cout << "Enter two numbers: ";
    cin >> num1 >> num2;

    // Perform the operation based on user input
    switch (operation) {
        case '+':
            cout << "Result: " << num1 + num2 << endl;
            break;
        case '-':
            cout << "Result: " << num1 - num2 << endl;
            break;
        case '*':
            cout << "Result: " << num1 * num2 << endl;
            break;
        case '/':
            if (num2 != 0)
                cout << "Result: " << num1 / num2 << endl;
            else
                cout << "Error: Division by zero!" << endl;
            break;
        default:
            cout << "Invalid operation!" << endl;
    }

    return 0;
}
