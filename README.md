# Priyanshi-Bisht - Calculator Project
 def add(x, y):
    return x + y
 def subtract(x, y):
    return x - y
 def multiply(x, y):
    return x  y
 def divide(x, y):
    if y == 0:
        return "Error! Division by zero."
    return x / y
 def calculator():
    print("Select operation:")
    print("1. Add")
    print("2. Subtract")
    print("3. Multiply")
    print("4. Divide")
    while True:
        choice = input("Enter choice (1/2/3/4): ")
        if choice in ['1', '2', '3', '4']:
            num1 = float(input("Enter first number: "))
            num2 = float(input("Enter second number: "))
            if choice == '1':
                print(f"{num1} + {num2} = {add(num1, num2)}")
            elif choice == '2':
                print(f"{num1} - {num2} = {subtract(num1, num2)}")
            elif choice == '3':
                print(f"{num1}  {num2} = {multiply(num1, num2)}")
            elif choice == '4':
                print(f"{num1} / {num2} = {divide(num1, num2)}")
        else:
            print("Invalid input")
 
   next_calculation = input("Do you want to perform another calculation? 
(yes/no): ")
        if next_calculation.lower() != 'yes':
            break
 if __name__ == "__main__":
    calculator()
 How to Use the Code:
 1. Copy the code into a Python file (e.g., calculator.py).
 2. Run the file using Python (e.g., python calculator.py).
 3. Follow the prompts to perform calculations.
 This calculator will continue to prompt for new calculations until the user decides to exit

