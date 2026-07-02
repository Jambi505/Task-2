# Task-2
Simple Calculator
#include <iostream>

int main() {
    double num1, num2;
    char op;

    std::cout << "Enter first number, operator (+, -, *, /), and second number: ";
    std::cin >> num1 >> op >> num2;

    switch(op) {
        case '+': std::cout << "Result: " << num1 + num2; break;
        case '-': std::cout << "Result: " << num1 - num2; break;
        case '*': std::cout << "Result: " << num1 * num2; break;
        case '/': 
            if (num2 != 0) std::cout << "Result: " << num1 / num2;
            else std::cout << "Error! Division by zero.";
            break;
        default: std::cout << "Invalid operator!";
    }
    return 0;
}
