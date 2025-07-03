# Assignment-7
# Assignment Question
1. Data Type Identification
Create four variables, one each for age, height, name, and whether you're a
student. Print the type of each variable.
2. Function Creation
Write a function called greet_ user(name) that returns a welcome message.
3. Mini Login System (Input + Conditions)
Ask the user to enter a username and password. If the username is "admin" and
the password is "1234", print "Login successful"; otherwise, print "Access denied".
4. Basic Calculator (Functions + Conditions)
Build a calculator that can add, subtract, multiply, or divide two numbers based
on user input.
5. Age Categorizer
Ask the user to enter their age and print the category:
0-12: Child, 13-19: Teen, 20-64: Adult, 65+: Senior.
   
 # Python variables to solve the question
## 1. Data Type Identification
   
age = 23            # integer
height = 5.6        # float
name = "Adeyemi Tomiwa"   # string
student = True   # boolean

print("Type of age:", type(age))
print("Type of height:", type(height))
print("Type of name:", type(name))
print("Type of student:", type(student))

## 2. Function Creation
   
  def greet_user(name):
    return f"Welcome, {name}!"

message = greet_user("Tomiwa")
print(message)

## 3. Mini Login System (Input + Conditions)
   
Get username and password from user
username = input("Enter your username: ")
password = input("Enter your password: ")

 Check credentials
if username == "Adetomiwa-123" and password == "1234456":
    print("Login successful")
else:
    print("Access denied")

  ## 4. Basic Calculator (Functions + Conditions)
     
    Define functions for each operation
def add(x, y):
    return x + y
def subtract(x, y):
    return x - y
def multiply(x, y):
    return x * y
def divide(x, y):
    if y != 0:
        return x / y
    else:
        return "Cannot divide by zero"
        
    Get user inputs
num1 = float(input("Enter the first number: "))
num2 = float(input("Enter the second number: "))
operation = input("Choose operation (add, subtract, multiply, divide): ")

    Perform calculation
if operation == "add":
    result = add(num1, num2)
elif operation == "subtract":
    result = subtract(num1, num2)
elif operation == "multiply":
    result = multiply(num1, num2)
elif operation == "divide":
    result = divide(num1, num2)
else:
    result = "Invalid operation selected"

print("Result:", result)
 
## 5. Age Categorize
   
 age = int(input("Enter your age: "))

if age >= 0 and age <= 12:
    print("You are a Child.")
elif age >= 13 and age <= 19:
    print("You are a Teen.")
elif age >= 20 and age <= 64:
    print("You are an Adult.")
elif age >= 65:
    print("You are a Senior.")
else:
    print("Invalid age entered.")
