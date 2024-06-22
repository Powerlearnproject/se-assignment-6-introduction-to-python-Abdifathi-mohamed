[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15307666&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.

   Python is a widely-used programming language, renowned for its popularity and versatility. It is often employed on servers to develop web applications.

   Features
     Easy to learn, write and read
     Interpreted Language
     Large standard library

   Python is applied in:
     Web Development
     Data Analyst
     Machine Learning and AI
   

2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.


Visit the official Python website python.org.
Navigate to the Downloads section and select the Python version for Windows.
Double-click the downloaded installer file.
Check the box labeled "Add Python to PATH".
Select "Install Now" or customize the installation by choosing "Customize installation".
Open Command Prompt. Type python --version and press Enter. It should display the installed Python version.
Alternatively, type python and press Enter to start the Python interactive shell.
pip usually comes bundled with Python. Verify by typing pip --version in Command Prompt.
Navigate to your project directory in Command Prompt.
Run python -m venv env to create a virtual environment named env.
Activate the virtual environment with .\env\Scripts\activate.


3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.
   
   Basic python program to print Hello World.
     print("Hello, World!")

   Explanation:
    print is a command in Python that tells the computer to display something on the screen.
    Parentheses () hold the thing you want to display. In this case, it’s the text "Hello, World!".
    A string is a type of information that consists of letters, numbers, and symbols. It is surrounded by quotes. In this example, "Hello, World!" is a string.


4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.

   Basic Data Types and There descriptions:
    1. Integer(int): whole numbers without decimals.
       example: 3, -4

       x = 4

    2. Floating (float): Numbers that have decimal points.
       example: 20.5
       y = 20.5

    3. String (srr): Characters or Text Type enslosed in    quotes  - single or double
     example: "Hello Wolld"

     Name = "Asha"


5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.

   Conditional statements in Python allow you to execute certain blocks of code based on whether a condition is true or false. These statements help control the flow of the program by making decisions. The main conditional statements in Python are if, elif, and else, for and while loop.

  Example for `if-else`

   number = 10

      if number > 0:
        print('Positive number')

      else:
        print('Negative number')

      print('This statement always executes')

      # output
      Positive Number


   Example `for` loop
      values = range(4)
      # iterate from i = 0 to i = 3
      for i in range(4):
        print(i)

      # output
      0
      1
      2
      3


6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

   A function is a block of code that performs a specific task.
   Functions are usefull in modularization, code reusability, and testing and debugging.

   
   Example:

    def sum(x, y):
      return x + y

     num = 40
     num1 = 30
     result = sum(num, num1)
     print(f"The sum of {num} and {num1} equals:", result)


   

7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.

   Lists allow us to store a sequence of items in a single variable while dictionary is a collection of items, similar to lists and tuples but each item in a dictionary is a key-value pair.

   # a list of three elements
    ages = [19, 26, 29]

     country_capitals = {
       "Germany": "Berlin", 
       "Canada": "Ottawa", 
       "England": "London"
      }

    # access list
      print(ages)

    # access the value of keys
      print(country_capitals["Germany"])  
      print(country_capitals["England"]) 


8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.

   Exception handling in Python is a way to deal with errors that may occur during program execution. It allows you to handle these errors gracefully without the program crashing.
   
   # Example

       try:
        numerator = 10
        denominator = 0

       result = numerator/denominator

       print(result)
      except:
       print("Error: Denominator cannot be 0.")
    
      finally:
       print("This is finally block.")


9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.

   A module is a piece of software that has a specific functionality. Modules in Python are just Python files with a .py extension. The name of the module is the same as the file name. A Python module can have a set of functions, classes, or variables defined and implemented.
   
   Packages are namespaces containing multiple packages and modules. They're just directories, but with certain requirements.

   # Example 
    import math 
    r = 4
    pie = math.pi

    print(pie * r * r)


    # output
    50.2654824574  



10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.


   # script that reads the content of a file and prints it to the console

   # Specify the file path
    file_path = "example.txt"

   # Open the file in read mode
    with open(file_path, "r") as file:
      # Read the entire content of the file
      file_content = file.read()

   #  Print the content to the console
   print("Content of the file:")
   print(file_content)


   # Script to write a list of strings to a file

     # Specify the file path
     file_path = "output.txt"

     # List of strings to write to the file
      strings_list = ["Hello", "World", "Python", "File", "IO"]

     # Open the file in write mode
       with open(file_path, "w") as file:
     # Write each string from the list to the file
      for string in strings_list:
        file.write(string + "\n")

      print(f"Strings have been written to {file_path}")


# References:
- W3 Schools
- Learn Python
- Geeks for Geeks
- Youtube


# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


