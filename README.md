Simple Python Calculator

This is a basic Python program that performs simple math operations.
You can add, subtract, multiply, and divide two numbers.

Features

Addition

Subtraction

Multiplication

Division

Easy to use

Works in the terminal

How to Run

Save the code as calculator.py

Open terminal or command prompt

Run this command:

python calculator.py

Code
print("----- Simple Calculator -----")

while True:
    print("\nChoose an operation:")
    print("1. Addition (+)")
    print("2. Subtraction (-)")
    print("3. Multiplication (*)")
    print("4. Division (/)")
    print("5. Exit")

    choice = input("Enter your choice (1-5): ")

    if choice == "5":
        print("Exiting... Goodbye!")
        break

    num1 = float(input("Enter first number: "))
    num2 = float(input("Enter second number: "))

    if choice == "1":
        print("Result =", num1 + num2)

    elif choice == "2":
        print("Result =", num1 - num2)

    elif choice == "3":
        print("Result =", num1 * num2)

    elif choice == "4":
        if num2 == 0:
            print("Error! Cannot divide by zero.")
        else:
            print("Result =", num1 / num2)

    else:
        print("Invalid choice! Please enter 1 to 5.")
