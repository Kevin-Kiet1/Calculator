# Calculator
#Simple Interactive Calculator in python

def interactive_calculator():
    '''() -> float

    precondition: operation must be within ['+', '-', '*', '/'] and num1 and num2 must be numbers

    Takes in no parameters but user input and returns a float
    '''
    
    num1 = float(input("Please enter your first number: "))
    num2 = float(input("Please enter your second number: "))
    operation = input("Please enter an operation (+, -, *, /): ")

    while operation not in ['+', '-', '*', '/']:
      print("Invalid option")
      operation = input("Please enter an operation (+, -, *, /): ")

    while operation in ['+', '-', '*', '/']:
      if operation == '+':
        return num1 + num2
      elif operation == '-':
        return num1 - num2
      elif operation == '*':
        return num1 * num2
      elif operation == '/':
        return num1 / num2

interactive_calculator()
