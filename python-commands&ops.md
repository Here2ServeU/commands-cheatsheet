# Python Command Reference Guide

A comprehensive guide to commonly used Python commands, operations, and features for scripting, development, and data analysis.

---

## Getting Started
1. **`python --version`**: Displays the installed version of Python.
2. **`python`**: Launches the Python interactive shell.
3. **`python <script_name>.py`**: Runs a Python script.
4. **`pip install <package>`**: Installs a Python package from PyPI.
5. **`pip list`**: Lists all installed Python packages.
6. **`pip freeze > requirements.txt`**: Saves a list of installed packages and their versions to a file.
7. **`pip install -r requirements.txt`**: Installs packages from a requirements file.

---

## Variables and Data Types
8. **`x = 10`**: Assigns a value to a variable.
9. **`type(x)`**: Returns the type of a variable (e.g., `int`, `str`).
10. **`x = "Hello"`**: Creates a string variable.
11. **`x = [1, 2, 3]`**: Creates a list.
12. **`x = (1, 2, 3)`**: Creates a tuple.
13. **`x = {"key": "value"}`**: Creates a dictionary.

---

## Input and Output
14. **`print("Hello, World!")`**: Prints a message to the console.
15. **`name = input("Enter your name: ")`**: Takes user input from the console.
16. **`f"Hello, {name}!"`**: Formats strings using f-strings.

---

## File Operations
17. **`with open("file.txt", "r") as file:`**: Opens a file for reading.
18. **`file.read()`**: Reads the content of a file.
19. **`file.write("Hello, World!")`**: Writes data to a file.
20. **`os.remove("file.txt")`**: Deletes a file (requires `import os`).

---

## Loops and Conditionals
21. **`if x > 0:`**: Executes a block of code if the condition is true.
22. **`for i in range(5):`**: Iterates over a range of numbers.
23. **`while x < 5:`**: Loops while a condition is true.
24. **`break`**: Exits a loop prematurely.
25. **`continue`**: Skips the current iteration of a loop.

---

## Functions and Classes
26. **`def greet(name):`**: Defines a function.
    ```python
    def greet(name):
        return f"Hello, {name}!"
    ```
27. **`class MyClass:`**: Defines a class.
    ```python
    class MyClass:
        def __init__(self, name):
            self.name = name
    ```
28. **`my_obj = MyClass("Python")`**: Creates an object of the class.

---

## Error Handling
29. **`try:`**: Attempts to execute a block of code.
30. **`except Exception as e:`**: Catches and handles exceptions.
    ```python
    try:
        x = 10 / 0
    except ZeroDivisionError as e:
        print("Error:", e)
    ```

---

## Common Libraries
31. **`import math`**: Imports the `math` library for mathematical operations.
    - **`math.sqrt(16)`**: Calculates the square root of 16.
32. **`import random`**: Imports the `random` library.
    - **`random.randint(1, 10)`**: Generates a random integer between 1 and 10.
33. **`import datetime`**: Imports the `datetime` library.
    - **`datetime.datetime.now()`**: Gets the current date and time.

---

## Data Structures
34. **`x.append(4)`**: Adds an item to a list.
35. **`x.remove(3)`**: Removes an item from a list.
36. **`x.keys()`**: Returns the keys of a dictionary.
37. **`x.values()`**: Returns the values of a dictionary.
38. **`x[0]`**: Accesses the first element of a list or tuple.

---

## Data Analysis (Pandas and Numpy)
39. **`import pandas as pd`**: Imports the Pandas library.
    - **`df = pd.DataFrame(data)`**: Creates a DataFrame.
    - **`df.head()`**: Displays the first few rows of a DataFrame.
40. **`import numpy as np`**: Imports the NumPy library.
    - **`np.array([1, 2, 3])`**: Creates a NumPy array.

---

## Virtual Environments
41. **`python -m venv <env_name>`**: Creates a virtual environment.
42. **`source <env_name>/bin/activate`**: Activates the virtual environment (Linux/Mac).
43. **`<env_name>\Scripts\activate`**: Activates the virtual environment (Windows).
44. **`deactivate`**: Exits the virtual environment.

---

## Debugging and Testing
45. **`import pdb; pdb.set_trace()`**: Adds a breakpoint for debugging.
46. **`assert x == 10`**: Tests a condition; raises an error if false.
47. **`unittest`**: Standard library for writing and running tests.

---

This guide covers essential Python commands and concepts to help you navigate your Python projects with ease. Bookmark it for quick reference!
