# Fundamentals of Coding
## Operations
### Conditionals

Conditionals in programming are statements or constructs that allow the execution of different code blocks based on whether a certain condition evaluates to true or false. They are fundamental to controlling the flow of a program and making decisions within it

Conditionals are essential for writing programs that can react to different inputs or situations dynamically. They allow programs to make decisions and adapt their behavior accordingly, making them powerful tools for building complex logic in software.

#### If Else
An if-else block is a fundamental construct in programming languages that allows for conditional execution of code. It's used to make decisions based on certain conditions. Here's how it generally works:
```python
if condition:
    # Block of code to execute if the condition is True
else:
    # Block of code to execute if the condition is False
```
In this structure:

The if statement checks a condition. If the condition is true, the code inside the if block is executed.
If the condition is false, the code inside the else block is executed.
Here's a simple Python example:

```python
x = 10

if x > 5:
    print("x is greater than 5")
else:
    print("x is not greater than 5")

```
In this example, if x is greater than 5, it prints "x is greater than 5"; otherwise, it prints "x is not greater than 5".

Additionally, you can have multiple elif (short for "else if") statements to check for multiple conditions:

```python
if condition1:
    # Block of code to execute if condition1 is True
elif condition2:
    # Block of code to execute if condition2 is True
elif condition3:
    # Block of code to execute if condition3 is True
...
else:
    # Block of code to execute if none of the above conditions are True

```
This construct allows for branching logic, where the program can follow different paths depending on the evaluation of conditions.


#### Switch
Switch statements are a type of conditional statement found in many programming languages. They provide a way to select one of many code blocks to be executed based on the value of a variable or expression.

Here's a basic structure of a switch statement:
```java
switch (expression) {
    case value1:
        // code block to execute if expression equals value1
        break;
    case value2:
        // code block to execute if expression equals value2
        break;
    // additional cases as needed
    default:
        // code block to execute if expression doesn't match any case
}
```

Here's a simple example in Java:
```java
int day = 3;
String dayName;

switch (day) {
    case 1:
        dayName = "Monday";
        break;
    case 2:
        dayName = "Tuesday";
        break;
    case 3:
        dayName = "Wednesday";
        break;
    // additional cases as needed
    default:
        dayName = "Unknown";
}
System.out.println("Day is: " + dayName);

```

In this example, if the variable day has a value of 3, it will execute the code block under case 3, assigning the value "Wednesday" to the variable dayName.

Key features of switch statements:

- They evaluate the value of an expression against a list of possible values.
- They offer an alternative to long sequences of if-else if-else statements when you have many conditions to check.
- Each case must end with a break statement to prevent execution from falling through to the next case.
- The default case is optional and is executed if none of the other cases match the expression's value.
- Switch statements are available in languages like Java, C, C++, C#, and others, though they may have slight syntax variations between languages.

### Iteratives
Iteratives, also known as loops, are programming constructs that allow you to repeatedly execute a block of code multiple times until a certain condition is met or for a specified number of iterations. They are essential for automating repetitive tasks and for iterating over collections of data.

There are several types of iterative constructs commonly found in programming languages:
#### For Loop
For loops: These loops are used when you know exactly how many times you want to execute a block of code. They typically have a loop variable that is incremented or decremented with each iteration.

Example (in Python):
```python
for i in range(5):
    print(i)
```

This will print numbers from 0 to 4.
#### While Loop
While loops: These loops are used when you want to execute a block of code as long as a specified condition is true. The condition is checked before each iteration.

Example (in Python):
```python
i = 0
while i < 5:
    print(i)
    i += 1
```

This will print numbers from 0 to 4.

Iteratives are fundamental to programming because they allow you to write efficient and concise code that can handle repetitive tasks or process large amounts of data without having to manually write the same instructions over and over again.

## Data Objects
 In programming, data objects are variables or entities that hold data or information. They are used to represent real-world objects, concepts, or values within a program. Data objects can take various forms depending on the programming language and the specific needs of the program.

Here are some common types of data objects:

1. **Primitive Data Types**: These are basic data types provided by programming languages to represent simple values. Examples include integers, floating-point numbers, characters, and boolean values.

2. **Arrays**: Arrays are data objects that can hold multiple values of the same type. They provide a way to organize and store collections of data elements under a single name.

3. **Objects**: Objects are instances of classes in object-oriented programming languages. They encapsulate data (attributes or properties) and behaviors (methods or functions) into a single entity. Objects can represent real-world entities or abstract concepts.

    Objects are a collection of data types meant to represent some entity. For example a customer may have attributes such as name, address, contact information. In out application we may need a customer object to represent the customer entity so we cal fulfill orders. So the customer object will have a string name, string address, and maybe another data type for the contact information. Grouping data in objects helps organize how we pass data in an application as well as structure the data once we save it to storage such as the database.

4. **Structures**: Structures are data objects that group together different variables of different data types under a single name. They are similar to objects but are typically used in languages that do not support object-oriented programming.

5. **Collections**: Collections are data structures that hold multiple elements of the same or different types. They provide operations for adding, removing, and accessing elements, making them useful for managing dynamic sets of data.

6. **Files and Streams**: Files and streams are data objects used for input and output operations in many programming languages. They represent external sources of data (files) or streams of data (such as network connections or standard input/output).

Data objects are essential components of programming because they allow developers to represent and manipulate data within their programs. By organizing data into objects, arrays, or other structures, programmers can write code that is more modular, maintainable, and scalable. Additionally, data objects facilitate communication between different parts of a program and enable interaction with external systems or resources.