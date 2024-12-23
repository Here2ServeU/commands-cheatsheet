Here’s a structured guide for essential Java commands and operations:

# Java Command Reference Guide

A comprehensive guide to commonly used Java commands, operations, and features for programming, compiling, and running Java applications.

---

## Getting Started
1. **`java --version`**: Displays the installed version of Java.
2. **`javac --version`**: Displays the installed version of the Java compiler.
3. **`javac <file_name>.java`**: Compiles a Java source file into bytecode (`.class` file).
4. **`java <class_name>`**: Executes a compiled Java program.
5. **`java -cp <directory> <class_name>`**: Specifies the classpath to run a program from a particular directory.
6. **`java -jar <file_name>.jar`**: Runs a Java program packaged as a JAR file.

---

## Variables and Data Types
7. **`int x = 10;`**: Declares and initializes an integer variable.
8. **`double y = 10.5;`**: Declares a floating-point variable.
9. **`String name = "Java";`**: Declares and initializes a string variable.
10. **`boolean isTrue = true;`**: Declares a boolean variable.
11. **`char letter = 'A';`**: Declares a character variable.
12. **`int[] numbers = {1, 2, 3};`**: Declares and initializes an array.

---

## Input and Output
13. **`System.out.println("Hello, World!");`**: Prints a message with a newline.
14. **`System.out.print("Enter your name: ");`**: Prints a message without a newline.
15. **`Scanner scanner = new Scanner(System.in);`**: Creates a scanner for user input.
    ```java
    String name = scanner.nextLine(); // Reads user input as a string
    ```
16. **`System.out.printf("Hello, %s!", name);`**: Formats and prints output.

---

## File Operations
17. **`File file = new File("file.txt");`**: Creates a File object.
18. **`file.exists()`**: Checks if the file exists.
19. **`FileWriter writer = new FileWriter("file.txt");`**: Creates a FileWriter to write data to a file.
20. **`BufferedReader reader = new BufferedReader(new FileReader("file.txt"));`**: Reads data from a file.

---

## Loops and Conditionals
21. **`if (x > 0) { ... }`**: Executes a block if the condition is true.
22. **`else if (x == 0) { ... }`**: Executes another block if the condition is true.
23. **`else { ... }`**: Executes a block if no conditions are met.
24. **`for (int i = 0; i < 10; i++) { ... }`**: Iterates over a range of numbers.
25. **`while (x > 0) { ... }`**: Repeats a block while the condition is true.

---

## Functions and Classes
26. **`public static int add(int a, int b) { ... }`**: Defines a static method.
    ```java
    public static int add(int a, int b) {
        return a + b;
    }
    ```
27. **`class MyClass { ... }`**: Defines a class.
28. **`public MyClass(String name) { ... }`**: Defines a constructor for the class.
29. **`MyClass obj = new MyClass("Java");`**: Creates an object of the class.

---

## Exception Handling
30. **`try { ... } catch (Exception e) { ... }`**: Handles exceptions that occur within the try block.
    ```java
    try {
        int result = 10 / 0;
    } catch (ArithmeticException e) {
        System.out.println("Error: " + e.getMessage());
    }
    ```
31. **`finally { ... }`**: Executes a block regardless of exceptions.

---

## Common Libraries
32. **`import java.util.ArrayList;`**: Imports the ArrayList class.
    - **`ArrayList<String> list = new ArrayList<>();`**: Creates a list.
    - **`list.add("Java");`**: Adds an item to the list.
33. **`import java.util.HashMap;`**: Imports the HashMap class.
    - **`HashMap<String, Integer> map = new HashMap<>();`**: Creates a key-value pair map.
34. **`import java.time.LocalDate;`**: Imports the `LocalDate` class.
    - **`LocalDate.now();`**: Gets the current date.

---

## Data Structures
35. **`list.size()`**: Returns the size of a list.
36. **`list.get(0)`**: Retrieves an element from a list by index.
37. **`map.put("key", 10);`**: Adds a key-value pair to a map.
38. **`map.get("key");`**: Retrieves a value by key.

---

## Debugging and Testing
39. **`System.out.println(variable);`**: Prints a variable for debugging purposes.
40. **`assert x > 0;`**: Asserts that a condition is true (use `-ea` flag to enable assertions).
41. **`JUnit`**: Use the JUnit library for unit testing.

---

This guide covers essential Java commands and concepts to help you write, debug, and run Java applications effectively. Bookmark it for quick reference!
