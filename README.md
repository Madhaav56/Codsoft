

def simple_calculator():
    print("Simple Calculator")
    print("Choose an operation:")
    print("1. Addition (+)")
    print("2. Subtraction (-)")
    print("3. Multiplication (*)")
    print("4. Division (/)")
    
    try:
        # Getting user inputs
        first_number = float(input("Enter the first number: "))
        second_number = float(input("Enter the second number: "))
        operation = input("Enter the operation (1/2/3/4): ")
        
        # Performing calculations based on the selected operation
        if operation == '1':
            result = first_number + second_number
            print(f"The sum of {first_number} and {second_number} is {result}.")
        elif operation == '2':
            result = first_number - second_number
            print(f"The difference between {first_number} and {second_number} is {result}.")
        elif operation == '3':
            result = first_number * second_number
            print(f"The product of {first_number} and {second_number} is {result}.")
        elif operation == '4':
            if second_number != 0:
                result = first_number / second_number
                print(f"The quotient of {first_number} and {second_number} is {result}.")
            else:
                print("Error: Cannot divide by zero.")
        else:
            print("Invalid operation selection. Please choose 1, 2, 3, or 4.")
    except ValueError:
        print("Invalid input. Please enter numeric values for numbers.")

# Run the simple calculator
simple_calculator()
