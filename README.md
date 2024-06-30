[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15350208&assignment_repo_type=AssignmentRepo)

# SE-Assignment-6

 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.
   Python is a widely used high-level programming language known for its simplicity, readability, and versatility. Key features include a clear syntax, a large standard library, support for multiple programming paradigms, and a strong community. Python is popular for web development (Django, Flask), data science and machine learning (NumPy, Pandas, scikit-learn), automation, scientific computing, GUI applications, game development, and education due to its ease of learning and extensive ecosystem of libraries and frameworks. Its portability across platforms further enhances its appeal for diverse development tasks.

2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.
   For Windows:
   Install Python:

   Visit the official Python website and download the latest Python installer for Windows.
   Run the installer and select the option to add Python to PATH during installation.
   Verify Installation:

   Open Command Prompt (cmd) or PowerShell.
   Type python --version or python -V to check the installed Python version.
   Type python to enter the Python interactive shell; exit() to exit.

   Set Up Virtual Environment:

   Install virtualenv if not already installed: pip install virtualenv.
   Navigate to your project directory in Command Prompt or PowerShell.
   Create a virtual environment: python -m venv myenv.
   Activate the virtual environment:
   Command Prompt: myenv\Scripts\activate
   PowerShell: .\myenv\Scripts\Activate.ps1
   You will see (myenv) indicating the virtual environment is active.
   Install packages inside the virtual environment using pip.

3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.
   print("Hello, World!")
   Print statement displays the content in the double quotation marks.
   String literals i.e "Hello, World in this case is enclosed in "" or ''

   When you run this program, Python executes it line by line.
   The print("Hello, World!") statement tells Python to output the text "Hello, World!" to the console.
   After executing this line, the program finishes its execution.

4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.
   In Python, basic data types include:
   Integer (int): Whole numbers without decimals (e.g., 10).
   Float (float): Real numbers with decimals (e.g., 3.14).
   String (str): Sequence of characters (e.g., "Alice").
   Boolean (bool): Represents True or False.
   List (list): Ordered collection of items (e.g., [1, 2, 3]).
   Tuple (tuple): Immutable ordered collection (e.g., (10, 20)).
   Dictionary (dict): Collection of key-value pairs (e.g., {'name': 'Bob', 'age': 30})

   Script:

# Variables of different data types

   x = 10        # Integer
   y = 3.14      # Float
   name = "Alice"  # String
   is_valid = True  # Boolean

   numbers = [1, 2, 3, 4, 5]  # List
   coordinates = (10, 20)     # Tuple
   person = {'name': 'Bob', 'age': 30}  # Dictionary

# Outputting values of variables

   print("Integer:", x)
   print("Float:", y)
   print("String:", name)
   print("Boolean:", is_valid)
   print("List:", numbers)
   print("Tuple:", coordinates)
   print("Dictionary:", person)

5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.
   They are control structures that allow you to execute certain blocks of code conditionally or repeatedly.
   #Example of an if-else statement
   x = 10

   if x > 5:
      print("x is greater than 5")
   else:
      print("x is not greater than 5")

   #Example of a for loop
   fruits = ["apple", "banana", "cherry"]

   for fruit in fruits:
      print(fruit)

6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.
   Functions in Python are blocks of reusable code designed to perform a specific task. They are useful for organizing code into manageable parts, improving code readability, and promoting code reusability.

   def sum_two_numbers(a, b):
    return a + b
   #Calling the function and storing the result in a variable
   result = sum_two_numbers(5, 3)

   #Printing the result
   print("The sum is:", result)

7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.
   Lists are ordered collections accessed by index, suitable for storing sequences of elements whereas dictionaries are unordered collections accessed by keys, ideal for storing key-value pairs with fast lookup.
   #Creating a list of numbers
   numbers_list = [1, 2, 3, 4, 5]

   #Creating a dictionary with key-value pairs
   person = {
      'name': 'Alice',
      'age': 30,
      'city': 'New York'
   }

   #Printing the list and dictionary
   print("List of Numbers:", numbers_list)
   print("Dictionary:", person)

   #Accessing elements by index in the list
   print("\nAccessing elements in the list:")
   print("First element:", numbers_list[0])
   print("Second element:", numbers_list[1])

   #Accessing elements by key in the dictionary
   print("\nAccessing elements in the dictionary:")
   print("Name:", person['name'])
   print("Age:", person['age'])
   print("City:", person['city'])

   #Modifying elements in the list and dictionary
   numbers_list[2] = 10
   person['age'] = 32

   print("\nModified List of Numbers:", numbers_list)
   print("Modified Dictionary:", person)

   #Adding elements to the list and dictionary
   numbers_list.append(6)
   person['gender'] = 'Female'

   print("\nList after adding element:", numbers_list)
   print("Dictionary after adding key-value pair:", person)

   #Removing elements from the list and dictionary
   numbers_list.remove(4)
   del person['city']

   print("\nList after removing element:", numbers_list)
   print("Dictionary after deleting key 'city':", person)

8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.
   Exception handling in Python refers to the process of managing and responding to errors that occur during program execution.

# Example of exception handling

   def divide_numbers(a, b):
      try:
         result = a / b
         print(f"Result of division: {result}")
      except ZeroDivisionError:
         print("Error: Division by zero!")
      except TypeError as e:
         print(f"Error: {e}")
      finally:
         print("Executing finally block.")
         # Clean-up code can go here (e.g., closing files, releasing resources)

# Test cases

   divide_numbers(10, 2)    # Normal case: no exception
   divide_numbers(10, 0)    # Handling ZeroDivisionError
   divide_numbers(10, '2')  # Handling TypeError

9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.
   Modules:
   Definition: Modules are files containing Python code that define functions, classes, and variables. They allow you to organize and reuse code across different Python scripts.
   Purpose: Modules help in keeping related code together, improving code organization, and facilitating code reuse.
   Example: A module can be a .py file containing functions and classes related to specific tasks, such as math operations, file handling, or data manipulation.

   Packages:
   Definition: Packages are namespaces that contain multiple modules. They provide a hierarchical structure to organize related modules.
   Purpose: Packages help in structuring large Python projects, preventing naming conflicts, and improving code maintainability.
   Example: Packages are directories containing __init__.py files and submodules, allowing for easy organization and distribution of Python code.

   To import and use a module in your Python script, you use the 'import' statement followed by the module name.

# Example of importing and using the math module

   import math

# Using math functions

   print("Square root of 16:", math.sqrt(16))  # Output: 4.0 (square root)
   print("Value of pi:", math.pi)  # Output: 3.141592653589793 (constant pi)

10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.
    To read from a file in Python, you typically follow these steps:
    Open the File: Use the open() function with the file path and mode ('r' for reading).
    Read from the File: Use methods like read(), readline(), or readlines() to access the file content.
    Close the File: Use the close() method to close the file after reading.

# Example of reading from a file and printing its content

# Specify the file path

   file_path = 'sample.txt'

# Open the file in read mode ('r')

   try:
      with open(file_path, 'r') as file:
         # Read and print the entire content of the file
         file_content = file.read()
         print("File Content:\n", file_content)
   except FileNotFoundError:
      print(f"Error: The file '{file_path}' was not found.")
   except IOError as e:
      print(f"Error: Unable to read the file '{file_path}'. {e}")

# Example of writing to a file

# List of strings to write to the file

   lines = [
      "Line 1: Hello, World!",
      "Line 2: Python is awesome.",
      "Line 3: Writing to files in Python."
   ]

# Specify the file path

   output_file = 'output.txt'

# Open the file in write mode ('w')

   try:
      with open(output_file, 'w') as file:
         # Write each line from the list to the file
         for line in lines:
               file.write(line + '\n')
      print(f"Successfully wrote {len(lines)} lines to '{output_file}'.")
   except IOError as e:
      print(f"Error: Unable to write to the file '{output_file}'. {e}")

# Submission Guidelines

- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].
