# Advance-Calculator-Vithyarthi-Project-

import math

def calculator():
    while True:
        print("\n========== ADVANCED CALCULATOR ==========")
        print("1. Addition")
        print("2. Subtraction")
        print("3. Multiplication")
        print("4. Division")
        print("5. Power")
        print("6. Square Root")
        print("7. Cube Root")
        print("8. Factorial")
        print("9. Percentage")
        print("10. Sin")
        print("11. Cos")
        print("12. Tan")
        print("13. Logarithm")
        print("14. Natural Log (ln)")
        print("15. Absolute Value")
        print("16. Floor Value")
        print("17. Ceiling Value")
        print("18. π (Pi)")
        print("19. e (Euler's Number)")
        print("20. Exit")
        print("=========================================")

        choice = input("Enter your choice: ")

        # Addition
        if choice == "1":
            a = float(input("Enter first number: "))
            b = float(input("Enter second number: "))
            print("Result =", a + b)

        # Subtraction
        elif choice == "2":
            a = float(input("Enter first number: "))
            b = float(input("Enter second number: "))
            print("Result =", a - b)

        # Multiplication
        elif choice == "3":
            a = float(input("Enter first number: "))
            b = float(input("Enter second number: "))
            print("Result =", a * b)

        # Division
        elif choice == "4":
            a = float(input("Enter first number: "))
            b = float(input("Enter second number: "))

            if b == 0:
                print("Cannot divide by zero!")
            else:
                print("Result =", a / b)

        # Power
        elif choice == "5":
            a = float(input("Enter base: "))
            b = float(input("Enter power: "))
            print("Result =", a ** b)

        # Square Root
        elif choice == "6":
            a = float(input("Enter number: "))
            if a >= 0:
                print("Square Root =", math.sqrt(a))
            else:
                print("Cannot find square root of a negative number.")

        # Cube Root
        elif choice == "7":
            a = float(input("Enter number: "))
            print("Cube Root =", a ** (1/3))

        # Factorial
        elif choice == "8":
            a = int(input("Enter a positive integer: "))
            if a >= 0:
                print("Factorial =", math.factorial(a))
            else:
                print("Factorial is not possible for negative numbers.")

        # Percentage
        elif choice == "9":
            value = float(input("Enter value: "))
            percentage = float(input("Enter percentage: "))
            print("Result =", (value * percentage) / 100)

        # Sin
        elif choice == "10":
            a = float(input("Enter angle in degrees: "))
            print("Sin =", math.sin(math.radians(a)))

        # Cos
        elif choice == "11":
            a = float(input("Enter angle in degrees: "))
            print("Cos =", math.cos(math.radians(a)))

        # Tan
        elif choice == "12":
            a = float(input("Enter angle in degrees: "))
            print("Tan =", math.tan(math.radians(a)))

        # Logarithm
        elif choice == "13":
            a = float(input("Enter number: "))
            base = float(input("Enter base: "))
            if a > 0 and base > 0 and base != 1:
                print("Log =", math.log(a, base))
            else:
                print("Invalid number or base.")

        # Natural Log
        elif choice == "14":
            a = float(input("Enter number: "))
            if a > 0:
                print("ln =", math.log(a))
            else:
                print("Number must be greater than 0.")

        # Absolute Value
        elif choice == "15":
            a = float(input("Enter number: "))
            print("Absolute Value =", abs(a))

        # Floor
        elif choice == "16":
            a = float(input("Enter number: "))
            print("Floor =", math.floor(a))

        # Ceiling
        elif choice == "17":
            a = float(input("Enter number: "))
            print("Ceiling =", math.ceil(a))

        # Pi
        elif choice == "18":
            print("π =", math.pi)

        # Euler's Number
        elif choice == "19":
            print("e =", math.e)

        # Exit
        elif choice == "20":
            print("Thank you for using the calculator!")
            break

        else:
            print("Invalid choice! Please try again.")


calculator()