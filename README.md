                                                                                                            [![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)

[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15366068&assignment_repo_type=AssignmentRepo)

# SE-Assignment-6

Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

Questions:

1.  Python Basics:

    - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.
    - **Answer** Python is a programming language. Some of its key features are that its easy to learn and use, it is dynamically typed and executed line by line. It has a vast standard library. For example in web development, python frameworks provide tools and libraries for database access, templating, and routing.

2.  Installing Python:

    - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.
    - **Answer** Go to your web browser and search for python download. Click on the first link,download the latest version for your operating system. For Windows, go to the downloaded installer, click "Add Python to PATH", and click "Install Now" to run the installer. You can check the python version you have installed in your files. Ensure you have the lates pip by running this command "pip install --upgrade pip". With the virtual environment active, you can now install packages using pip command "pip install package_name". When you are done with your virtual environment, just run "deactivate".

3.  Python Syntax and Semantics:

    - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.
    - **Answer** By typing "print("Hello World")" which is the function call. The print() Function is used to output text to the console. The string is what is inside the parentheses, it is then closed by single or double qoutes.

4.  Data Types and Variables:

    - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.
    - **Answer** Integer (int) it represents whole numbers, positive or negative, without a fractional part like 1 or -2. Float (float): are real numbers with a fractional part, using decimal points like example 0.5,-0.78. String (str): inclosed inside the parentheses, is used to store text. Boolean (bool): one of two values, right or wrong, true or false. List (list):Are ordered collections of items, which can be of different types. Tuple (tuple): Similar to lists, but immutable (cannot be changed after creation). Dictionary (dict): are key-value pairs, used for mapping unique keys to values. Set (set): Represents unordered collections of unique items for example ('apple', 'banana', 'cherry').

5.  Control Structures:

    - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.
    - **Answer** Conditional statements are used to execute different blocks of code based on different a certain condition. The `if-else` statement evaluates a condition and executes the corresponding block of code based on whether the condition is True or False. For example if a number is 10, write "number = 10"
      if number > 0:
      print("The number is positive.")
      else:
      print("The number is not positive.")
    - Loops in python are used to repeatedly execute a block of code for as long as the condition is true. The `for` loop is used to iterate over a sequence, for example:
      vegetables = ["carrot", "potato", "tomato"]
      for veggie in vegitables:
      print(veggie)

6.  Functions in Python:

    - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.
    - **Answer** Functions in python are blocks of reusable code that perform a specific task. They are useful because they help break down complex problems into smaller ones that are more manageable. You can be able to reuse code without rewriting it. Functions make code easier to read and maintain.
    - A Python function that takes two arguments and returns their sum is return, for example:
      def add_numbers(a, b):
      return a + b

7.  Lists and Dictionaries:

    - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.
    - **Answer** Lists in Python maintain order of items as they were added, they can also be modified. They can have items of the same or different types. Items in a list are accesesed by their position starting from 0.
    - Dictionaries in Python have no order, the keys are unordered, and must be immutable data type.
    - Creating a list of numbers: numbers = [1, 2, 3, 4, 5]
      -Creating a dictionary with some key-value pairs: student = {
      "name": "Alice",
      "age": 22,
      "degree": "Data Sciences"
      }

8.  Exception Handling:

    - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.
    - **Answer** Exception handling in Python is a mechanism that is used to handle runtime error, making sure that the program can run without problems.
    - To use `try`, `except`, and `finally` :
      try:
      numerator = 10
      denominator = 0
      result = numerator/denominator
      print(result)
      except:
      print("Error: Denominator cannot be 0.")
      finally:
      print("This is finally block.")

9.  Modules and Packages:

    - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.
    - **Answer** A module in Python is a file that has definitions and statements, they are used to break large programs into smaller, managable, and organized ones. A package in Python is a way of organizing related modules in a directory hierachy.
    - To import a module, you can write this command: "import my_module
      result = my_module.add(5, 3)" where "my_module" is what you have named your own module.
      -To use math write : "import math"
      Here are the functions you can use:
      "math.sqrt" is used to find the square root of a number.
      "math.factorial" calculates the factorial of a number.
      "math.pi" provides the value of Pi.
      "math.sin" calculates the sine of an angle (in radians).
    - for example:
      result_sqrt = math.sqrt(16)
      print(f"The square root of 16 is {result_sqrt}")
      with this output: The square root of 16 is 4.0

10. File I/O:

    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.
    - **Answer** By using the "with" statement you can be able to read and write to your files in python.
    - for example: read_file.py
      def read_file(file_path):
      try:
      with open(file_path, 'r') as file:
      content = file.read()
      print(content)
      except FileNotFoundError:
      print(f"The file at {file_path} does not exist.")
      except IOError:
      print(f"An error occurred while reading the file at {file_path}.")
      The read method is used to read the entire file.

    - To write to the file you just use "write_to_file":

      def write_to_file(file_path, lines):
      try:
      with open(file_path, 'w') as file:
      for line in lines:
      file.write(line + '\n')
      print(f"Successfully wrote to {file_path}.")
      except IOError:
      print(f"An error occurred while writing to the file at {file_path}.")
      The function "write_to_file" takes the file path and and the list of lines(/n) to write in.

# Submission Guidelines:

- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].
