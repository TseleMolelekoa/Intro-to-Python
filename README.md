# Intro-to-Python
# Day 1
Python is an interpreted language. This means that a new executable file is created when you run your code. The next time that you execute your code, this new executable file is run instead of the original file. It is a relatively simple language that includes a standard library that provides modules for a large number of processes that programs deal with. This approach keeps Python simple yet reliable programming language. Python has an easy-to-use syntax that is focused on the programmer who must type in the program, read what was typed, and provide formal documentation for the program. Python strikes a good balance between fast compilations and readability, and it is easier to write applications. Python is implemented in C and relies on the extensive, well understood, portable C libraries. It fits seamlessly with UNIX, Linux, and POSIX environments. Since these standard C libraries are widely available for the various MS-Windows variants, and other non-POSIX operating systems, Python runs similarly in all environments. The Python programming language was created based on lessons learned during language and operating system support. 
Python is built from concepts in the ABC and Modula-3 languages.
# Comments in Python:
Comments are added to make the source code easier to understand. Comments in Python start with the hash character, #, and extend to the end of the physical line. A comment may appear at the start of a line or following whitespace or code, but not within a string literal.

# Creating Applications using Python:
Indentation in Python identifies what code belongs to what section of code.

# Escape Sequences:
Backslash character (): e.g \
New line feed: \n
Tab: \t
Vertical tab: \v
Backspace: \b
Carriage return: \r
Single quote (useful in strings enclosed in single quotes: ‘hello \ ‘World’): \'
Double quote (useful in strings enclosed in single quotes: “hello \ “World”): \"

# Reserved words in Python:
NB: Cannot be used as ordinary identifiers, must be spelled EXACTLY as wriiten here: False class finally is return None continue for lambda try True def from nonlocal while and del global not with as elif if or yield assert else import pass
Python 3.5 keywords (added 'async', 'await', 'asynchronous', 'contextlib', 'async for', 'async with')
async await async def async for async with asynchronous contextlib

Python 3.6 keywords (added 'f' for formatted string literals)
f False async await True

Python 3.7 keywords (added 'async' and 'await' as non-keyword identifiers, 'contextvars', 'nonlocal', 'dataclasses')
async await contextvars dataclasses nonlocal

Python 3.8 keywords (added 'walrus' operator ':=')
:=

Python 3.9 keywords (added 'match' statement)
match

Anaconda Navigator:
Anaconda is a popular open-source distribution of Python and other data science-related packages. It simplifies the process of installing, managing, and updating Python libraries for data science, machine learning, and scientific computing. Anaconda includes tools such as conda, a powerful package manager, and provides an environment management system, allowing users to create isolated Python environments for different projects, making it easier to manage dependencies and avoid conflicts between packages.

# Day 2:
## Variables:
Variables in programming act as temporary storage spaces in a computer's memory, holding various data values. When a variable's value changes, it affects the program's current state. They serve as containers for different data items, and understanding them is essential for programming. Variables are crucial in all programming languages, allowing data transfer between functions and making programming tasks more manageable. Each variable is created with an initial value. A value can be in THREE states:

Variable creation (Declaration)
Variable assignment (Initialization)
Variable changed (Execution)
NB: Once the code which created the variable has finished executing, the variable is destroyed.

NB: In Python, variables are defined in a standard way, by using the assignment character (=). This changes the value of the variable. Naming conventions specify the way in which variables should be named. This standard is used to make code more readable, and thus easier to understand.

The rules include the start and continuation characters. Variable names may contain any upper or lower case letter (A–Z, a–z), a number, or the underscore character. They may not begin with a number or contain spaces. Continuation characters are any characters except whitespace characters like tab and space.

## Here are a few examples of valid variable names:

1. c
2. ref_number
3. admin
4. aVeryLongName

## Here are a few examples of invalid variable names:

True
$name
12Graph

NB: In Python identifiers are case sensitive!!!

NB: Variables cannot have the same name as Python’s keywords!!!

We can find out what keywords are in Python, by using the function called dir(). If this function is called with the builtins attribute, it returns a list of Python’s built-in attributes.

The builtins module contains all Python’s built-in attributes, which can be used with the dir()function.

# The ones that are returned are identified with the following characteristics:

Python’s built-in exceptions start with a capital letter.

The rest are either functions or data type names.

Identifiers that start and end with one or two underscores are special methods.

NB: All of the methods, exceptions, and functions contained in
dir(builtins), dir(doc), dir(name), and dir(package) cannot be used as variable names.

# Using Variables:
All variables are assigned to a data type, be it a STRING, or an INTEGER.
Values of the same type can be manipulated together.
In Python, automatic type conversion, also known as implicit casting, allows the interpreter to automatically convert compatible data types, such as integers to floats or floats to strings, as needed during operations or assignments, simplifying code and enhancing flexibility.

### Variables are fundamental to programming in Python and are used extensively to store and manipulate data within programs.

## Concatenation and Operations with Variables:
You can concatenate strings and perform various operations with numerical variables.

## Data Types:
Python is dynamically typed, meaning you don't have to explicitly declare the type of a variable. Python will automatically determine the data type based on the value assigned to it. Common data types include:

Integers: Whole numbers (e.g., int_var = 10)
Floats: Decimal numbers (e.g., float_var = 3.14)
Strings: Text (e.g., string_var = "Hello, World!")
Booleans: True or False values (e.g., bool_var = True).

##Variable Naming Rules:
Variable names can consist of letters (both uppercase and lowercase), digits, and underscores.
Variable names cannot start with a digit.
Python variable names are case-sensitive, meaning myVar, MyVar, and myvar would be considered three different variables.
Variable names should be descriptive to indicate the kind of data they store (e.g., age, name, total_score).
Casting:
# Implicit Casting:
In Python, automatic type conversion, also known as implicit casting, allows the interpreter to automatically convert compatible data types, such as integers to floats or floats to strings, as needed during operations or assignments, simplifying code and enhancing flexibility. Also ensures that no data is lost when these conversions occur.

# Explicit Casting:
A value cannot be automatically cast from one data type to another if it will result in data loss. Extra code has to be written to ensure that the value stays the same and only the data type changes; like when casting from a floating-point value to an integer value.
## Example is :
num1 = 15    #num1 variable is automatically assigned
   #as an integer value
num2 = "30"   #num2 variable is automatically assigned
     #as a string value
ans = num1 + num2   #ans is assigned to num1 added to num2
print ("answer:", ans) #ans is printed


# The rules to convert a string to a float are:

The string should only contain numbers.
Other than numbers the following are allowed:
Only one dot (.) character. Indicates the decimal starts after the dot (.) character. A ‘+’ or ‘−‘ character at the beginning of the string. This indicates that the number is either positive or negative.

# Day 3
Three data types have already been used in the examples before. Now we shall have a more detailed look at the data types used in Python. Data types have different functions in a program. One of the most important factors to take into consideration is that the performance of a computer can be severely affected by choosing the wrong data type. a program might only need to use numbers between 1 and 20; it would therefore not make sense to use string variables to store these numbers in, as one will need to convert these strings back to numbers in order to perform calculations on them. This would create extra work for the computer, which means that the performance could degrade in larger programs. Therefore, one should rather define the variables as integers. 
## Data Types to be covered:

1. Integers
2. Booleans
3. Floating point numbers
4. Complex numbers
5. Strings
6. literals

These are the representations of values in code. These values can be of different data types, such as integers, floating-point numbers, characters, strings, and boolean values. Literals are used to directly represent fixed values in the code without requiring computations or additional processing. Literals are fundamental building blocks in programming and are used to define constant values, initialize variables, and provide input data to programs. Literals are values that never change, i.e. they are a constant. Look at the following example:
        #Interpreter
print ("The answer: ", 5 + 2)

The answer: 7

## common types of literals in programming:
1. Integer Literals:
Integer literals represent whole numbers. Examples: 0, 42, -17.

2. Floating-Point Literals:
Floating-point literals represent decimal numbers. Examples: 3.14, 0.1, -0.003.

3. String Literals:
String literals represent sequences of characters. They are usually enclosed in single (') or double (") quotes. Examples: 'hello', "world".

4. Character Literals:
Character literals represent single characters and are enclosed in single quotes. Examples: 'a', '5', '%'.

5. Boolean Literals:
Boolean literals represent the two truth values: True and False.

6. Null or None Literals:
In some programming languages like Python, None represents the absence of a value or a null value.

7. Hexadecimal and Octal Literals:
Some programming languages allow the representation of integers in hexadecimal (base 16) or octal (base 8) notation. For example, in Python, 0x1A represents 26 in hexadecimal, and 0o34 represents 28 in octal.

## Examples in PYTHON
Integer literals
integer_literal = 42

Floating-point literals
float_literal = 3.14

String literals
string_literal = "hello"

Character literals (in Python, characters are represented as strings of length 1)
char_literal = 'a'

Boolean literals
boolean_literal = True

None literal
none_literal = None

## \Data Types Examples Integers: T
hese represent numbers in an unlimited range. This is only limited by a machine’s memory. Booleans: Evaluate to ‘True or False’, 1 or 0 respectively. Floating point numbers: Floating-point numbers represent double-precision numbers. Complex numbers: Complex numbers represent numbers as a pair of double-precision numbers. Strings: A sequence of Unicode characters e.g. a word or a sentence that can be manipulated.

## Itergers
Python has three distinctive numeric types; this means that for every number that you use in your programs there is a suitable data type that you will use to ensure that your programs are truly performance efficient.

Python is a static language because only values of a certain type can be assigned to particular variables, according to their data types assigned.Integers are always whole numbers. Integers include negative and positive numbers. The only factor that determines the range of an integer variable is the amount of memory a machine has available.
The four main operators used when doing calculations, are ‘+’, ‘-’, ‘*’, and ‘/’. There are more, but those will be discussed later in the course. The plus ‘+’ operator can be used universally, which means that you can use it for purposes other than to adding numbers together. The plus operator can also be used to concatenate strings. programs had fixed values that were used to get an output by manipulating the given data. In real life situations, almost all programs require some sort of input from the user to give accurate output. This is done by using the input() command.

## BOOLEANS
The boolean data type has corresponding integer values. There are only two possible values that a Boolean variable can have, True (1) or False (0). When returning Booleans as strings they are seen as “True” and “False”, and never as “1” and “0”. True and False are case-sensitive in Python. Boolean tests whether conditions are valid or not. The three logical operators used to test conditions between two arguments are:

The and-operator
The or operator
The not-operator

## The following variable values are considered False:

False
None
Zero for any numeric data type, 0, 0.0, 0j
An empty sequence or mapping. Like a list or tuple, ' ', ( ), [ ], { }
Instances of user-defined classes, where a class that defines a bool() method returns zero or False.
All values returned otherwise are always considered true. This means that many objects will always return true.

Operators and built-in functions that have a Boolean result always return (False or 0) or (True or 1). The Boolean or and and operations always return only one of the options, either True or False.

## FLOATING POINT NUMBERS
Floating point numbers are better known as floats. Float is the data type that manages numbers with decimal places with very accurate precision. The float data type can be called as a function with zero or 1 argument of any data type.

If no argument is given, then float returns 0.0. If an argument is given, an attempt will then be made to convert the value to a float data type, but this does not mean it is always possible. For example, float("21.765") will be converted to a float, but float("FF909A") will raise an exception. A string value cast to a float must contain only numbers and only one occurrence of the dot (.) character. The following piece of code will clarify the statement.

## Complex numbers
The absolute value of a complex number is its magnitude (or modulus), defined as the theoretical distance between the coordinates (real,imag) of x and (0,0) (applying the Pythagorean theorem). Another way of thinking about it is that it can be used to calculate the distance from 0, if you walk 5 km left and then 10 km up: you will be 11.19 km from where you started, because Banner Complete = 11.185. Complex numbers are two numbers contained in a single variable. The first part of a complex number is the real part (float), and the second part is the imaginary part (float), assigned in this manner: complex(real, image). Imaginary numbers are real multiples of the imaginary unit, written with a suffix of j (J). The imaginary part is the square root of -1. Python has built-in support for complex numbers. The latter notation is written as follows: 4+8j.Complex numbers are used in Python to combine two numbers into one manageable number. The following example shows how complex numbers are used in a simple manner.

a_comp = complex(4, 8) # defines a_comp complex number i1 = 5 i2 = 6 b_comp = complex(i1, i2) # complex(5, 6)

print (a_comp.real) # first number which is 4 print (a_comp.imag) # second number which is 8

print (abs(a_comp)) # sqrt(a_comp.real2 + a_comp.imag2) print (a_comp + 5+6j) # adds a_comp complex number to a prints the total

print (7+5j + 10+4j) # adds 7 + 10 and 5 + 4 separately.

Using the ‘+=‘ operator with strings
The ‘+=‘ operator adds values to an existing variable.
# Strings
Strings are represented by the immutable (unchangeable) str data type. Strings are a sequence of Unicode characters which form a single manageable string. The str data type can be called to create a string; when there is no argument supplied, it returns an empty string. s = str("") is the same as s = str(), when an argument is passed to the string method that is not a string value, it is passed as a string representation of the type supplied: s = str(17.2354), is the same as s = str("17.2354"). The string function is often used to convert other data types to strings.
## Example: 

print ("Please enter your name:")

s_name = input(str())

print ("Please enter your surname:")

s_surname = input(str())

print ("Please enter your current age")

i_age = input(int())

s = str(i_age)


sentence = s_name + " " 

sentence += s_surname + " is currently "

sentence += s + " year(s) old" 


print (sentence)

OUTPUT
Please enter your name:
tshele
Please enter your surname:
molelekoa
Please enter your current age
046
tshele molelekoa is currently 46 year(s) old

## Using the ‘+=‘ operator with strings
The ‘+=‘ operator adds values to an existing variable.
​
# Lambda Expressions
Lambda expressions, also known as anonymous functions or lambda functions, are a concise way to create small, unnamed functions in programming languages. This function returns the sum of its two arguments: lambda a, b: a+b. Lambda functions can be used wherever function objects are required. Lambda expressions are powerful and flexible, but they should be used judiciously(with good judgment or sense.). For complex logic, it's often better to use named functions for the sake of readability and maintainability. Lambda functions are most suitable for simple operations and brief computations.
 Lambda expressions are often used when you need a simple function for a short period of time and don't want to formally define a full function using the def keyword.

## Syntax:
lambda arguments: expression

Here's a breakdown of the components:

lambda keyword: Indicates that you're creating a lambda expression.
arguments: Represents the input parameters of the lambda function. You can have zero or more arguments separated by commas.
expression: Represents the computation that the lambda function performs. The result of this expression is implicitly returned from the lambda function.

Like nested function definitions, lambda functions can reference variables from the containing scope.

# Day 4 Operators

operators are special symbols or keywords used to perform operations on variables and values. There are several types of operators in Python, including arithmetic operators, comparison operators, logical operators, assignment operators, and more. Let's go through each type of operator with examples:
1. Arithmetic Operators:
Arithmetic operators are used to perform mathematical operations.
+ (Addition): Adds two operands.

python

result = 5 + 3  # Result will be 8
- (Subtraction): Subtracts the right operand from the left operand.

python

result = 7 - 2  # Result will be 5
* (Multiplication): Multiplies two operands.

python
result = 4 * 6  # Result will be 24
/ (Division): Divides the left operand by the right operand (always results in a float).

python

result = 10 / 3  # Result will be 3.3333...
// (Floor Division): Divides and rounds down to the nearest integer.

python

result = 10 // 3  # Result will be 3
% (Modulus): Returns the remainder of the division.

python
Copy code
result = 10 % 3  # Result will be 1
** (Exponentiation): Raises the left operand to the power of the right operand.

python

result = 2 ** 3  # Result will be 8
2. Comparison Operators:
Comparison operators are used to compare values.

== (Equal): Checks if the values of two operands are equal.

python

result = 5 == 5  # Result will be True
!= (Not Equal): Checks if the values of two operands are not equal.

python

result = 5 != 3  # Result will be True
> (Greater Than): Checks if the left operand is greater than the right operand.

python

result = 7 > 4  # Result will be True
< (Less Than): Checks if the left operand is less than the right operand.

python

result = 2 < 6  # Result will be True
>= (Greater Than or Equal To): Checks if the left operand is greater than or equal to the right operand.

python

result = 4 >= 4  # Result will be True
<= (Less Than or Equal To): Checks if the left operand is less than or equal to the right operand.

python

result = 3 <= 5  # Result will be True
3. Logical Operators:
Logical operators are used to combine conditional statements.

and: Returns True if both statements are true.

python
Copy code
result = (5 > 3) and (4 < 6)  # Result will be True
or: Returns True if one of the statements is true.

python

result = (5 > 3) or (4 > 6)  # Result will be True
not: Reverse the result, returns False if the result is true.

python

result = not (5 > 3)  # Result will be False
4. Assignment Operators:
Assignment operators are used to assign values to variables.

= (Assignment): Assigns the value of the right operand to the left operand.

python

x = 5  # x is now 5
+= (Add and Assign): Adds the right operand to the left operand and assigns the result to the left operand.

python

x += 3  # Equivalent to x = x + 3, x is now 8
-= (Subtract and Assign): Subtracts the right operand from the left operand and assigns the result to the left operand.

python

x -= 2  # Equivalent to x = x - 2, x is now 6
*= (Multiply and Assign): Multiplies the left operand by the right operand and assigns the result to the left operand.

python
x *= 4  # Equivalent to x = x * 4, x is now 24
/= (Divide and Assign): Divides the left operand by the right operand and assigns the result to the left operand.

python
x /= 3  # Equivalent to x = x / 3, x is now 8.0 (float)
These are the basic types of operators in Python. Understanding and mastering these operators are essential for writing effective and efficient Python programs.

# WEEK 2
# Day 1
## Control flow statements

A program’s control flow is the order in which the program’s code executes.
The control flow of a Python program is regulated by conditional statements, loops, and function calls.
Python has three types of control structures:

·         Sequential - default mode
·         Selection - used for decisions and branching
·         Repetition - used for looping, i.e., repeating a piece of code multiple times.

1    1. Sequential
Sequential statements are a set of statements whose execution process happens in a sequence. The problem with sequential statements is that if the logic has broken in any one of the lines, then the complete source code execution will break.

a=20
b=12
c=a-b
print("Subtraction is:", c)

## 2. Selection/Decision control statements

 In Python, the selection statements are also known as Decision control statements or branching statements.

 The selection statement allows a program to test several conditions and execute instructions based on which condition is true.

Some Decision Control Statements are:

Simple if

if-else

nested if

if-elif-else

Simple if: If statements are control flow statements that help us to run a particular code, but only when a certain condition is met or satisfied. A simple if only has one condition to check.

## 2.   Repetition
 
A repetition statement is used to repeat a group(block) of programming instructions.

In Python, we generally have two loops/repetitive statements:

for loop

while loop

for loop: A for loop is used to iterate over a sequence that is either a list, tuple, dictionary, or a set. We can execute a set of statements once for each item in a list, tuple, or dictionary.

while loop: In Python, while loops are used to execute a block of statements repeatedly until a given condition is satisfied. Then, the expression is checked again and, if it is still true, the body is executed again. This continues until the expression becomes false.

# GRADED ACTIVITY
1.Using two for loops, write a program that produces the following output:

>>>

1 2 3

4 5 6

7 8 9
>>>
# Using two for loops to create the specified pattern
for i in range(1, 10, 3):
    for j in range(i, i + 3):
        print(j, end=" ")
    print()
In the outer loop, the variable i takes values 1, 4, and 7, and in the inner loop, the variable j takes values from i to i + 3, printing the numbers in each row. The end=" " argument in the print function is used to separate the numbers with spaces instead of newlines.
2.   Input in a number representing a car type, until the number 0 is input. There are three types of cars: 1 = luxury, 2 = commercial, 3 = sedan. Count how many of each type there are and print out this total with a message stating what type of car it is.
# Initialize counters for each car type
luxury_count = 0
commercial_count = 0
sedan_count = 0

# Infinite loop to take car type input until 0 is entered
while True:
    car_type = int(input("Enter car type (1 for luxury, 2 for commercial, 3 for sedan, 0 to stop): "))
    
    # Check if input is 0 to break the loop
    if car_type == 0:
        break
    
    # Update counters based on car type
    if car_type == 1:
        luxury_count += 1
    elif car_type == 2:
        commercial_count += 1
    elif car_type == 3:
        sedan_count += 1
    else:
        print("Invalid car type. Please enter 1, 2, 3, or 0.")
        continue

# Print the total counts for each car type
print(f"Total luxury cars: {luxury_count}")
print(f"Total commercial cars: {commercial_count}")
print(f"Total sedan cars: {sedan_count}")

the while True loop continues indefinitely until the user enters 0. Inside the loop, the program asks for car type input, updates the corresponding counters based on the input, and if an invalid input is given, it prompts the user to enter a valid car type. When the user enters 0, the loop breaks, and the program prints the total counts for each car type.

3.  Write a program that contains a while loop. Use a variable to count the number of iterations and print out this value each time. After the fifth iteration, the loop should stop and exit. Use the break statement.
   
# Initialize a variable to count the number of iterations
iteration_count = 0

# Start a while loop
while True:
    # Increment the iteration count
    iteration_count += 1
    
    # Print the current iteration count
    print(f"Iteration {iteration_count}")
    
    # Check if the fifth iteration is reached, then exit the loop
    if iteration_count == 5:
        print("Reached fifth iteration. Exiting the loop.")
        break


The while True loop runs indefinitely until it encounters the break statement inside the loop when iteration_count becomes equal to 5. The program prints the current iteration count at each step. When the fifth iteration is reached, it prints a message and exits the loop.
# Day 2

## Using Functions
We create functions by providing three pieces of information. The name of the function, a list of zero or more parameters, and, optionally, a block of code which provides the return value (a function can return nothing).

We normally define functions in script files for the simple reason that we do not want to type them more than once, we just want to edit a function (if necessary).

We must make a firm distinction between an argument value and a parameter:

·         Argument

The argument is the object used in an application of a function; it may be referenced by other variables or objects.

·         Parameter

The parameter is a variable name that is part of the function and is a local variable within the function body.
We define a function by using the following syntax:

def function_name(parameter <,...>):

# suite
The function_name part is the name used to call a function. The parameter part shows that zero or more parameters can be given to a function. The suite part is where the functionality is coded.
The first line of a function’s suite should always be a comment. This comment must briefly explain what the function does.

When the return statement is included in the function’s suite, it means that the function returns a result, for example a calculated value. The return statement can also be used to break out of a function.
There are three types of functions in Python:
Ordinary functions
Procedure functions
Factory functions

Ordinary functions are functions that follow mathematical procedures. They will receive an argument, perform a specific calculation with the argument, and return a result.
Procedure functions normally do not return a result; they are called to execute a procedure. For example a function can be created to set up a connection to a database.
Factory functions do not take parameters. The function generates values. Some factory functions work by accessing an object encapsulated in a module. For example, you will access the random number generator encapsulated in the random module.

The following is an example of how programs use functions to be more efficient:
Example 1 – Function:

def calculateTax(salary):

  """Calculates and prints a given salary’s tax"""

  if salary > 30000 :

    rate = 0.2

  elif salary > 10000 :

    rate = 0.15

  else:

    rate = 0.1

  tax = salary * rate

  print (tax)
print ("Enter the amount on which you want to calculate tax:")

calculateTax(int(input()));

Notice that the function must be defined before it can be called. The program is divided into two separate programs: the main program and the calculateTax function are separate pieces of code. Each time calculateTax() is called, it will run through the function’s piece of code.
The rate and tax variables are only accessible in the calculateTax function itself; you cannot use or access them outside of calculateTax. The variables rate, tax, and salary are known as local variables, because they are local to the function in which they are declared and cannot be accessed by other functions.
If we want the value of a local variable to be available in another part of the application, one way of doing this is to return the value to the program or function which called it. For example, if we want the value of the tax variable to be available in the main program, we can use a return statement to accomplish this. Remember that it is only the value of the variable that is being returned and not the variable itself.

Example 2 – Default parameters:
1 x = 15
def num(y = x):
"""This function assigns a default value to y"""
return y
7 x = 5             #Reassign 'x' to 5.
print (num())     #Returns 15 (default value not changed)

Using default parameters in functions has one advantage. You would automatically assign a default value to a parameter within a function. The default value would only be used if a function call does not include a specific parameter’s value; the parameter would then take the default value that was specified in the function’s declaration.

The above example assigns 15 to the x variable. A function is then declared called num. The num function has only one parameter (y), which has a default value of 15. Line 7 changes the value of x to 5. This change would not affect the default value of y, because num has already been declared. Line 8 would then thus print 15.

# Day4
Regular expressions, often referred to as “regexes,” are a concise way of specifying patterns in text. They are a powerful tool in Python, thanks to the `re` module, and serve several key purposes:



1.	Parsing: Regular expressions are used to identify and extract specific pieces of text that match certain criteria within a larger text or data.



2.	Searching: They help locate substrings that may have multiple forms, such as finding various image file extensions like ‘pet.png,’ ‘pet.gif,’ and ‘pet.mpg’ while excluding ‘carpet.gif.’





3.	Searching and Replacing: You can find substrings and replace specific words within the matched string or strings, such as replacing a local phone number format like ‘071 234 5678’ with an international format like ‘+2771 234 5678.’



4.	Splitting Strings: Regular expressions are handy for splitting a string at specific delimiters. For example, you can split a comma-separated list into individual items by using a regex that matches ‘,’.





5.	Validation: They are used to check whether a string adheres to certain criteria, like validating whether an email address is in the standard format.

However, regular expressions do have limitations:

-	They are suitable for handling recursive (repeating) structured text only if the maximum number of repetitions is known in advance.

-	Large and complex regex patterns can become challenging to maintain and understand.


As a best practice, when dealing with highly structured data formats like XML, it’s often better to use specialized parsers tailored to that format. In simpler terms, a basic regular expression consists of a character followed by a quantifier, while more complex expressions can involve combinations of quantified expressions to match intricate patterns in text data.

## Regular expression syntax

This section provides an overview of regular expressions (regex) and their syntax. It covers key functions from the Python re module and presents a table of commonly used functions and their descriptions.


1.	**Introduction to Regular Expressions: ** 

-	Regular expressions are a powerful tool for text pattern matching.

-	The section is divided into four subsections:


-	Matching individual characters or character groups.

-	Quantifying matches (e.g., matching zero or more occurrences).


-	Creating and grouping sub-expressions.

-	Using language assertions and flags.


2.	**Table of re Module Functions (commonly used):**

-	`compile`: Compiles a regex pattern.

-	`findall`: Returns a list of all non-overlapping matches in a string.


-	`finditer`: Returns an iterator over all matches.

-	`match`: Tries to apply the pattern at the start of the string.


-	`search`: Scans through a string looking for a match.

-	`split`: Splits a string by pattern occurrences.


-	`sub`: Replaces occurrences of the pattern in the string.

-	`subn`: Returns a 2-tuple with the new string and the number of replacements.


-	`template`: Compiles a template pattern.


3.	 **Regular Expression Syntax:**

-	This part explains various regex syntax elements:

-	`.` (Dot): Matches any character (except newline).


-	`^`: Matches the start of the string.

-	`$`: Matches the end of the string.


-	`*`: Matches zero or more occurrences.

-	`+`: Matches one or more occurrences.


-	`?`: Matches zero or one occurrence.

-	`{m}`: Matches exactly m occurrences.


-	`{m,n}`: Matches from m to n occurrences.

-	`{m,n}?`: Matches as few occurrences as possible.


-	`\`: Escapes special characters or signals a special sequence.

-	`[]`: Indicates a set of characters.


-	`|`: Represents alternation (matches X or Y).

4.	**Raw Strings in Python:**

-	Explains the importance of using raw strings in regex.

-	In raw strings, backslashes are treated as literal characters, making regex patterns cleaner.

6.	**Example – Validating Input Format:**

-	Demonstrates the use of regex to validate input.

-	Shows two equivalent regex patterns: one using a raw string and one without.
-	Validates input in the format of three numbers enclosed in brackets.


The provided code example shows how to validate input in a specific format (three numbers enclosed in brackets) using regular expressions and demonstrates the use of raw strings for cleaner pattern definition.


Overall, this section provides a comprehensive introduction to regular expressions and their syntax, with a focus on Python’s re module and the importance of using raw strings to simplify regex pattern creation.


# Character and character classes:

In this section on regular expressions and escape characters, the following key points are discussed:

1.	Basic Regex Expressions:

-	A single character, like ‘5’ or ‘b’, matches one occurrence by default.

-	Special characters in regex, like ‘+’, ‘*’, and ‘?’, need a backslash (\) as a prefix if they are to be treated as literals.

2.	Escape Characters in Python and Regex:

-	Escape characters in Python include ‘\’, ‘\n’, ‘\t’, and more. They are used to represent special characters or control characters.

-	To use special regex characters as literals, they must be preceded by a backslash (\).


3.	Example – Matching Special Characters:

-	A Python example is given where regular expressions are used to match the presence of a ‘+’ character and a newline character (‘\n’) in a sentence.

-	The ‘^’ symbol matches the start of the text, ‘.*’ matches zero or more characters (including newlines), ‘[\+]+’ matches one or more ‘+’ characters, and ‘$’ matches the end of the line.


4.	Character Classes and Ranges:

-	Character classes, like [ea], match either ‘e’ or ‘a’.

-	Ranges, like [0-9], match any digit from 0 to 9.


-	Negating a character class, like [^0-9], matches any character except digits.

5.	Handling Special Characters within Character Classes:

-	Dashes (-) and some other characters are metacharacters by default. However, if they are the first character within a character class (e.g., [-abc]), they are treated as literals and do not require a backslash.

-	Other metacharacters, like ‘.’, ‘^’, ‘?’, ‘+’, ‘*’, are always treated as literals within character classes.

7.	Shortcuts in Character Classes:

-	Python offers shortcuts for character classes, such as ‘\d’ (matches any digit) and ‘\s’ (matches whitespace).

-	The ASCII flag can modify the behavior of these shortcuts.


8.	Example – Using Shortcuts in Character Classes:

-	A Python example illustrates how to count the number of words in a sentence using shortcuts like ‘\w’ and ‘\W’.

-	The regular expression ‘^[\W]*[\w]*[\W]*’ is used to identify words in a sentence.

In summary, this section covers the basics of regular expressions, escape characters, character classes, and shortcuts within character classes. It provides practical examples to demonstrate the use of these concepts in Python.

#Quantifies and flags:

## Quantifies:

This section explains quantifiers in regular expressions and provides shorthand notations for simplifying the use of quantifiers. The key points covered are as follows:

1.	Quantifiers in Regex:

-	A quantifier in regex has the form {m, n}, specifying the minimum and maximum number of times an expression must match.

-	For example, e{1,1}e{1,1} and e{2,2} both match “feelings” but not “belt.”


2.	Shorthand Notations for Quantifiers:

-	Regex provides shorthand notations to simplify quantifiers.

-	If only one number is supplied, it’s assumed that the minimum and maximum are the same. For example, e{4} is equivalent to e{4, 4}.


-	Different minimum and maximum values can be convenient. For instance, to match both “travelled” and “traveled,” you can use “travel{1,2}ed” or “travell{0,1}ed.”

-	The ‘?’ symbol is used to represent {0,1}, meaning the preceding character is optional.

3.	Examples of Using Quantifiers:

-	An example in Python demonstrates the use of quantifiers to match words like “travelled” and “traveled” with the pattern ‘travell?ed’ (where ‘?’ is a shorthand for {0,1}).

-	This allows for flexibility in matching words with different numbers of ‘l’ characters.


In summary, this section clarifies the concept of quantifiers in regular expressions and shows how shorthand notations like ‘?’ can be used to make regex patterns more concise and flexible. It provides a practical example in Python to illustrate the application of these quantifiers.

# Flags:

Flags are used to tell the regex how to behave when looking for expressions.

This section introduces various regex flags and their functions in Python. The key points covered include:

1.	Regex Flags:

-	Python offers several flags to modify the behavior of regex patterns.

-	Flags, like re.IGNORECASE or re.VERBOSE, can be used to make regex matching more flexible and readable.

2.	Examples of Flags:

-	An example demonstrates the use of the IGNORECASE flag (re.IGNORECASE or re.I) for case-insensitive matching. It removes all vowels (both uppercase and lowercase) from a string.

-	Another example uses the VERBOSE flag (re.VERBOSE or re.X) to make a complex regex pattern more readable. It checks whether a string is a valid octal or hexadecimal number.

3.	IGNORECASE Flag:

-	The IGNORECASE flag is used to make regex matching case-insensitive, reducing the need to specify both uppercase and lowercase characters explicitly.

4.	VERBOSE Flag:

-	The VERBOSE flag allows comments and white spaces to be included in a regex pattern, making complex expressions more readable.

-	It can be especially useful for explaining longer and more intricate regular expressions.

In summary, this section covers the use of regex flags, specifically the IGNORECASE (case-insensitive) and VERBOSE (readable) flags, and provides practical examples to illustrate their application in Python.


# WEEK3 
##day1 
The keyword def introduces a function definition. It must be followed by the function name and the parenthesized list of formal parameters. The statements that form the body of the function start at the next line, and must be indented.

The first statement of the function body can optionally be a string literal; this string literal is the function’s documentation string, or docstring. (More about docstrings can be found in the section Documentation Strings.) There are tools which use docstrings to automatically produce online or printed documentation, or to let the user interactively browse through code; it’s good practice to include docstrings in code that you write, so make a habit of it. 

The execution of a function introduces a new symbol table used for the local variables of the function. More precisely, all variable assignments in a function store the value in the local symbol table; whereas variable references first look in the local symbol table, then in the local symbol tables of enclosing functions, then in the global symbol table, and finally in the table of built-in names. Thus, global variables and variables of enclosing functions cannot be directly assigned a value within a function (unless, for global variables, named in a global statement, or, for variables of enclosing functions, named in a nonlocal statement), although they may be referenced. 

The actual parameters (arguments) to a function call are introduced in the local symbol table of the called function when it is called; thus, arguments are passed using call by value (where the value is always an object reference, not the value of the object). 1 When a function calls another function, a new local symbol table is created for that call. 

A function definition introduces the function name in the current symbol table. The value of the function name has a type that is recognized by the interpreter as a user-defined function. This value can be assigned to another name which can then also be used as a function. This serves as a general renaming mechanism.

# MORE LISTS

 list is a built-in data type used to store multiple items. Lists are mutable, which means you can modify their elements after they have been created.
 ## Creating Lists:
You can create a list by enclosing a sequence of items inside square brackets [], separated by commas. For example: my_list = [1, 2, 3, 4, 5] 

Lists can contain elements of different data types, including numbers, strings, and even other lists.

# Accessing Elements:
You can access elements in a list using indexing. Python uses zero-based indexing, meaning the first element is at index 0, the second element at index 1, and so on. Negative indexing allows you to access elements from the end of the list, with -1 representing the last element:
print(my_list[0])  # Output: 1
print(my_list[-1]) # Output: 5


## Slicing Lists:
You can extract a portion of a list using slicing. Slicing allows you to create a new list containing elements from a specified start index to an end index (exclusive):
subset = my_list[1:4] # Creates a new list: [2, 3, 4]

## Modifying Lists:
Lists are mutable, which means you can change their elements after creation. You can assign new values to specific indices or use methods like append(), insert(), extend(), and remove() to modify lists:

## modifier list.
my_list[2] = 10       # Modifying an element at index 2
my_list.append(6)      # Appending a new element to the end of the list
my_list.insert(2, 7)   # Inserting an element at index 2
my_list.extend([8, 9]) # Extending the list with another list
my_list.remove(3)      # Removing the first occurrence of an element

# List Methods:
Python provides various built-in methods to work with lists. Some commonly used methods include:

len(list): Returns the length of the list.
list.append(element): Adds an element to the end of the list.
list.insert(index, element): Inserts an element at the specified index.
list.extend(iterable): Extends the list by adding elements from an iterable.
list.remove(element): Removes the first occurrence of the specified element.
list.pop(index): Removes and returns the element at the specified index.
list.index(element): Returns the index of the first occurrence of the specified element.
element in list: Returns True if the element is present in the list, False otherwise.

# Day2

# day 3

# Day4

In Python, classes are used to create objects, which are instances of the class. Classes provide a means of bundling data (attributes) and functionality (methods) together. Here's a basic overview of how classes work in Python:

Defining a Class:
To define a class, you use the class keyword, followed by the class name and a colon. Class names in Python are typically written in CamelCase.
Class Constructor and Instance Variables:
The __init__ method is a special method in Python classes and is used as a constructor. It is called when a new object of the class is instantiated. Instance variables are variables that belong to the object and are defined within the __init__ method using the self keyword.

class MyClass:
    def __init__(self, var1, var2):
        self.var1 = var1
        self.var2 = var2
        
## Class Methods:
Methods are functions defined within a class. They can perform operations on the class's data or provide some functionality related to the class.

class MyClass:
    def __init__(self, var1, var2):
        self.var1 = var1
        self.var2 = var2
    
    def display_vars(self):
        print("Var1:", self.var1)
        print("Var2:", self.var2)

# Creating an object of the class
obj = MyClass(10, 20)
obj.display_vars()

## Inheritance:
Inheritance allows one class to inherit properties and methods from another class. The derived class (subclass) inherits attributes and behaviors from the base class (superclass).
class ParentClass:
    def __init__(self, var1, var2):
        self.var1 = var1
        self.var2 = var2

class ChildClass(ParentClass):
    def __init__(self, var1, var2, var3):
        super().__init__(var1, var2)
        self.var3 = var3

ChildClass inherits from ParentClass. The super() function is used to call the constructor of the parent class within the child class.

# Three important principles of object-oriented programming (OOP):

1. Encapsulation:
Encapsulation is the bundling of data (attributes) and methods (functions) that operate on the data into a single unit known as a class. The data within a class is often kept private to prevent direct access from outside the class. Instead, access to the data is controlled through public methods, also known as getters and setters.

In Python, encapsulation is achieved by using private and public access specifiers. By convention, attributes prefixed with a single underscore (e.g., _variable) are considered protected, and attributes prefixed with double underscores (e.g., __variable) are considered private.

class MyClass:
    def __init__(self):
        self._protected_var = 10  # protected variable
        self.__private_var = 20    # private variable

    def get_private_var(self):
        return self.__private_var

obj = MyClass()
print(obj._protected_var)  # Accessing protected variable (not recommended)
   #print(obj.__private_var)  # This will raise an error (private variable)
print(obj.get_private_var())  # Accessing private variable through a public method

# 2. Abstraction:
Abstraction is the process of hiding the complex implementation details and showing only the necessary features of an object. In Python, abstraction is achieved through abstract classes and interfaces. Abstract classes are classes that cannot be instantiated and are meant to be subclassed by other classes. Abstract methods defined in abstract classes must be implemented by their subclasses.

from abc import ABC, abstractmethod

class Shape(ABC):
    @abstractmethod
    def area(self):
        pass

class Square(Shape):
    def __init__(self, side):
        self.side = side

    def area(self):
        return self.side * self.side

square_obj = Square(5)
print(square_obj.area())  # Output: 25
   #shape_obj = Shape()  # This will raise an error (abstract class cannot be instantiated)

# 3. Polymorphism:
Polymorphism allows objects of different classes to be treated as objects of a common superclass. It enables flexibility and interchangeability of objects, making the code more modular and easier to maintain. Polymorphism is often achieved through method overriding and duck typing in Python.
Method overriding occurs when a subclass provides a specific implementation for a method that is already defined in its superclass. This allows objects of different classes to be used interchangeably based on their common interface.

class Animal:
    def sound(self):
        pass

class Dog(Animal):
    def sound(self):
        return "Woof!"

class Cat(Animal):
    def sound(self):
        return "Meow!"

def print_animal_sound(animal):
    print(animal.sound())

dog = Dog()
cat = Cat()

print_animal_sound(dog)  # Output: Woof!
print_animal_sound(cat)  # Output: Meow!

In the example above, print_animal_sound() function can accept objects of different classes (Dog and Cat) because they share a common interface (the sound() method). This is an example of polymorphism in action.

These principles of object-oriented programming help in creating more organized, efficient, and maintainable code in Python and many other object-oriented programming languages.

# Python Scopes and Namespaces
A namespace is a container that holds a set of identifiers (variable names, function names, class names, etc.) and their corresponding objects (values). A scope is a region of the program where a namespace is directly accessible. Understanding scopes and namespaces is crucial for writing Python code that behaves as expected, especially when dealing with variables and functions.

There are several types of namespaces and scopes in Python:

# 1. Local Namespace/Scope:
A local namespace is the namespace inside a function.
It contains local variables, function arguments, and the function's name.
This namespace is created when the function is called and is destroyed when the function exits.
Local variables cannot be accessed from outside the function.
 examples:

def my_function():
    local_var = 10  # This is a local variable
    print(local_var)

my_function()
  # print(local_var)  # This will raise an error because local_var is not accessible here
  
# 2. Enclosing Namespace/Scope (Closure):
An enclosing namespace is the namespace of the containing (enclosing) function.
It is accessible from nested functions.
This allows inner functions to access variables from the outer (enclosing) function.

def outer_function():
    outer_var = 20

    def inner_function():
        print(outer_var)  # Accessing outer_var from the enclosing scope

    inner_function()

outer_function()  # Output: 20


# 3. Global Namespace/Scope:
The global namespace contains variables defined at the top level of the script or module.
Global variables can be accessed from any part of the module or script.
To modify a global variable inside a function, you need to use the global keyword


global_var = 30  # This is a global variable

def my_function():
    global global_var
    global_var += 1
    print(global_var)


# 4. Built-in Namespace/Scope:
The built-in namespace contains functions and names pre-defined in Python.
Functions like print(), len(), and built-in types like list, dict are part of the built-in namespace.

my_function()  # Output: 31
print(len([1, 2, 3]))  # Output: 3


# Classes and Variables

In object-oriented programming, class variables and instance variables are used to store data within classes. They serve different purposes and have different scopes.

Class Variables:
Class variables are shared by all instances (objects) of a class. They are defined within a class but outside of any methods. Class variables are common to all instances of the class and are used to store data that is shared among all objects of that class.


 class MyClass:
    class_variable = 0  # This is a class variable

    def __init__(self, instance_variable):
        self.instance_variable = instance_variable  # This is an instance variable

# Accessing the class variable
print(MyClass.class_variable)  # Output: 0

# Modifying the class variable
MyClass.class_variable = 10
print(MyClass.class_variable)  # Output: 10

# Creating instances of the class
obj1 = MyClass(5)
obj2 = MyClass(8)

# Accessing instance variables
print(obj1.instance_variable)  # Output: 5
print(obj2.instance_variable)  # Output: 8

above, class_variable is a class variable shared by all instances of MyClass. Changes made to the class variable are reflected in all instances.

# Instance Variables:
Instance variables are specific to each instance of a class. They are defined inside the class methods, particularly within the class's constructor method (__init__). Instance variables are used to store data that is unique to each object created from the class.

In the example above, instance_variable is an instance variable. Each instance of MyClass can have a different value for instance_variable.

Instance variables are accessed and modified using the self keyword within class methods. Each instance of the class has its own copy of instance variables.
   class MyClass:
    def __init__(self, instance_variable):
        self.instance_variable = instance_variable  # This is an instance variable

# Creating instances of the class
obj1 = MyClass(5)
obj2 = MyClass(8)

# Accessing instance variables
print(obj1.instance_variable)  # Output: 5
print(obj2.instance_variable)  # Output: 8


class variables are shared among all instances of a class and are defined outside any methods, while instance variables are specific to each object and are defined within methods, usually in the constructor. Understanding the distinction between these types of variables is essential for effective object-oriented programming in Python.


# RANDOM REMARKS

Data attributes override method attributes with the same name; to avoid accidental name conflicts, which may cause hard-to-find bugs in large programs, it is wise to use some kind of convention that minimizes the chance of conflicts. Possible conventions include capitalizing method names, prefixing data attribute names with a small unique string (perhaps just an underscore), or using verbs for methods and nouns for data attributes.

Data attributes may be referenced by methods as well as by ordinary users (“clients”) of an object. In other words, classes are not usable to implement pure abstract data types. In fact, nothing in Python makes it possible to enforce data hiding — it is all based upon convention. (On the other hand, the Python implementation, written in C, can completely hide implementation details and control access to an object if necessary; this can be used by extensions to Python written in C.) 


random remarks and tips related to programming in Python and general software development:

Python's Readability:
Python emphasizes readability and simplicity, making it a great language for beginners and experienced developers alike. The use of indentation to define blocks of code enhances code readability.

Use of Libraries:
Python has a rich ecosystem of libraries and modules that can significantly speed up development. Whether you're working on web development, data analysis, machine learning, or any other domain, there's likely a Python library that can assist you.

Virtual Environments:
It's good practice to use virtual environments (e.g., virtualenv or venv) for each of your Python projects. Virtual environments allow you to manage project-specific dependencies without interfering with system-wide Python packages.

Error Handling:
Python provides robust error handling mechanisms using try, except, finally, and raise keywords. Proper error handling can make your code more reliable and user-friendly.

List Comprehensions:
Python's list comprehensions provide a concise way to create lists. They can often replace traditional loops, making your code more compact and expressive.

example:
       # Traditional loop
squares = []
for i in range(1, 6):
    squares.append(i**2)

# Using list comprehension
squares = [i**2 for i in range(1, 6)]


   ##Week 4 

## Objects and classes  

### Inheritance and private variables. 

In Python, inheritance is a fundamental object-oriented programming (OOP) concept that allows a new class (subclass or derived class) to inherit attributes and methods from an existing class (base class or superclass).  

This promotes code reuse, extensibility, and the creation of a hierarchy of classes. 

To declare private variables we use double underscore__ infront of your variable name. 

A private variable means its private to the class 

 

#### Here are key points about inheritance in Python: 

 

1. Syntax: 

To create a subclass that inherits from a superclass, you define the subclass using the `class` keyword, followed by the subclass name and the superclass name in parentheses.  

 

For example: 

   class Superclass: 

   # Superclass attributes and methods 

 

  class Subclass(Superclass): 

  # Subclass attributes and methods 

 

2. Access to Superclass Methods: 

 The subclass can access the methods and attributes of the superclass. 

 This allows you to reuse code and extend the functionality of the superclass.  

 You can call the superclass methods using the `super()` function. 

 

3. Overriding Methods: 

 If a method in the subclass has the same name as a method in the superclass, the method in the subclass will override the method in the superclass. 

 This is known as method overriding, and it allows the subclass to provide a specific implementation. 

 

4. Multiple Inheritance: 

Python supports multiple inheritance, where a class can inherit from more than one superclass.  

This is done by listing multiple superclass names in the parentheses after the subclass name. However, multiple inheritance can lead to complexities, and it's essential to use it carefully. 

 

5. Inheritance Hierarchy: 

Classes can form an inheritance hierarchy, where a class inherits from another class, and then another class inherits from it, creating a chain of inheritance. 

This helps in organizing and structuring code. 

Here's a simple example: 

class Animal: 

 def speak(self): 

 print("Animal speaks") 

 

class Dog(Animal): 

 def bark(self): 

 print("Dog barks") 

 

# Creating an instance of Dog 

my_dog = Dog() 

 

# Accessing methods from the superclass 

my_dog.speak()  # Output: Animal speaks 

my_dog.bark()   # Output: Dog barks 

In this example, the `Dog` class inherits from the `Animal` class, and the `Dog` instance can use both the `speak` method from the `Animal` class and the `bark` method from the `Dog` class. 

 

### For presentation  

 

fundamental concept in Python programming - Inheritance. It's a powerful feature in object-oriented programming that allows us to create a hierarchy of classes, promoting code reuse and organization. 

Slide 1: What is Inheritance? 

 

At its core, inheritance is a way for a new class to inherit attributes and methods from an existing class. Think of it as a way of passing down characteristics from a parent to a child. 

Slide 2: Syntax of Inheritance 

 

In Python, we use the class keyword to define classes. To create a subclass that inherits from a superclass, we simply include the superclass name in parentheses after the subclass name. 

python 

Copy code 

class Superclass: 

    # Superclass attributes and methods 

 

class Subclass(Superclass): 

    # Subclass attributes and methods 

Slide 3: Accessing Superclass Methods 

 

Once we have a subclass, we can access the methods and attributes of the superclass. This is done using the super() function. It allows us to reuse code and extend the functionality of the superclass. 

python 

Copy code 

class Animal: 

    def speak(self): 

        print("Animal speaks") 

 

class Dog(Animal): 

    def bark(self): 

        super().speak()  # Accessing superclass method 

        print("Dog barks") 

Slide 4: Overriding Methods 

 

Inheritance allows us to override methods in the subclass. If a method in the subclass has the same name as a method in the superclass, the subclass method will override it. This enables us to provide a specific implementation. 

python 

Copy code 

class Animal: 

    def speak(self): 

        print("Animal speaks") 

 

class Dog(Animal): 

    def speak(self): 

        print("Dog barks")  # Overriding the speak method 

Slide 5: Multiple Inheritance 

 

Python supports multiple inheritance, where a class can inherit from more than one superclass. This can be useful but needs to be used carefully to avoid complexities. 

python 

Copy code 

class A: 

    pass 

 

class B: 

    pass 

 

class C(A, B):  # Multiple inheritance 

    pass 

Conclusion: 

 

Inheritance is a powerful tool that makes our code more modular, readable, and scalable. It encourages a structured approach to coding and helps in creating well-organized class hierarchies. 

 

As you work on your projects, consider how inheritance can be applied to make your code more efficient and maintainable. 

 

Q&A: 

 

Now, I'd like to open the floor for any questions you may have about inheritance. Feel free to share your thoughts or ask for clarification. 

Feel free to customize the presentation based on your audience and the specific examples you want to showcase. Adding practical examples and engaging with the audience can enhance the learning experience. 

 

 

 

 

 

Private variables 

 

private variables are a way to restrict access to certain class attributes or variables from outside the class itself. 

 This encapsulation is achieved using a naming convention rather than a strict access control mechanism. 

 

Variables designated as private in Python conventionally start with an underscore (_) as a prefix in their names (e.g., _variable_name). 

 

 However, this is more of a convention and less of a strict rule, as Python does not have a strong notion of access control like some other languages do. 

 

Although these variables are not truly private in the sense that they cannot be accessed at all from outside the class, their naming convention serves as a signal to other developers that these attributes are intended for internal use within the class, and they should not be accessed or modified directly from outside the class. 

Python follows the principle of "we are all consenting adults here," which means that it trusts developers to use private variables responsibly and doesn't strictly enforce access restrictions. However, developers are encouraged to respect the convention and avoid direct manipulation of private variables from outside the class, accessing them instead through class methods known as getters and setters to maintain encapsulation and data integrity. 

 

 

 

 

 

 

 

 

Example  

 

 

 

## Day 2 

### Iterators and Generators 

 

Iterators and generators are essential features in Python that facilitate efficient handling of sequences and data streams, providing a way to iterate through elements without storing them entirely in memory. 

 

 Iterators: 

 

Definition: An iterator is an object that allows sequential access to elements within a collection or sequence, one element at a time, without the need to load the entire collection into memory. 

   

Usage: Iterators are used with iterable objects like lists, tuples, dictionaries, strings, etc., and they enable iteration using the `iter()` function and fetching elements using the `next()` function. 

   

Characteristics: 

    Iterators maintain their internal state and remember the current position during iteration. 

    - They implement two methods: `__iter__()` (to obtain the iterator object itself) and `__next__()` (to retrieve the next element in the sequence). 

    - When all elements are exhausted, the `StopIteration` exception is raised. 

 

####Generators: 

 

Definition: Generators are a type of iterable that generate values on-the-fly and produce a sequence of values using the `yield` statement, allowing iteration without the need to construct an entire list or collection in memory. 

   

Usage: Generators can be created using generator functions (functions containing `yield` statements) or generator expressions (similar to list comprehensions but using round brackets `()`). 

   

Characteristics: 

    - Generator functions use the `yield` keyword to produce a series of values, suspending the function's state between each `yield` call and resuming execution from where it left off when `next()` is called again. 

    - They are memory efficient as they produce values on demand, reducing memory overhead. 

    - Generator expressions are concise and create generators without the need for defining a separate function. 

 

 Summary: 

 

Iterators provide a way to access elements sequentially, remembering their state, and allowing iteration over a sequence using `iter()` and `next()` functions. 

   

Generators are a specific type of iterator that generates values lazily using `yield`, making them memory-efficient and suitable for handling large datasets or infinite sequences. 

 

Both iterators and generators play a crucial role in Python programming, offering flexibility, efficiency, and a convenient way to handle and process data in a memory-efficient manner. 

 

###Generator Expressions 

 

Generator expressions in Python are concise and memory-efficient constructs for creating generators. They are similar to list comprehensions but use round brackets `()` instead of square brackets `[]`. Generator expressions generate values on-the-fly, allowing iteration over large or potentially infinite sequences without constructing the entire sequence in memory. 

 

### Key points about Generator Expressions: 

 

1. Syntax: Generator expressions follow a similar syntax to list comprehensions but use round brackets instead of square brackets: 

 

    ```python 

    # List comprehension 

    list_comp = [x for x in range(10)]  # Generates a list 

 

    # Generator expression 

    gen_exp = (x for x in range(10))    # Generates a generator object 

    ``` 

 

2. Lazy Evaluation: Generator expressions produce values one at a time as they are needed. They do not create the entire sequence in memory at once, making them memory-efficient. 

 

3. Iterative Access: You can iterate over the values produced by a generator expression using a `for` loop or by passing it to functions that accept iterables. 

 

    ```python 

    gen_exp = (x for x in range(10)) 

    for value in gen_exp: 

        print(value) 

    ``` 

 

4. Use Cases: Generator expressions are suitable for situations where you need to iterate over large datasets, process elements on-the-fly, or generate an infinite sequence without storing all the elements in memory. 

 

5. Efficiency: They are especially useful when dealing with large collections of data, as they avoid the memory overhead associated with creating a full list or sequence. 

 

6.Combining with Functions: Generator expressions can be used with functions that consume iterables, like `sum()`, `min()`, `max()`, `filter()`, `any()`, `all()`, etc., enabling efficient processing of data without loading it entirely into memory. 

 

```python 

# Example: Finding the sum of squares of even numbers using generator expression 

even_squares_sum = sum(x**2 for x in range(10) if x % 2 == 0) 

print(even_squares_sum)  # Output: 120 

``` 

 

generator expressions provide a concise and memory-efficient way to create generators in Python, allowing for the efficient processing of large or potentially infinite sequences of data. 

 

 

### Error Output Redirection and Program Termination 

 

Error output redirection and program termination involve managing how errors are handled, displayed, and the program's response to such errors. 

 

#### Error Output Redirection: 

 

1. Standard Error Stream (stderr): Python distinguishes between standard output (`stdout`) and standard error (`stderr`). Errors and exceptional situations are typically printed to `stderr` rather than `stdout`.

# Day 4 

Logging, Managing packages with pip, and Floating point Arithmetic. 

Logging: 

Logging is a process of recording events, messages, or information about the execution of a program. It's a valuable tool for debugging and understanding the flow of a program. In Python, the logging module provides a flexible framework for emitting log messages from Python programs. You can use it to output messages to different places (console, files) at different levels (debug, info, warning, error, critical). 

Managing Packages with pip: 

 pip is the package installer for Python. Inside a virtual environment, you can use pip to install, upgrade, and uninstall packages. You can install, upgrade, and remove packages using a program called pip. By default pip will install packages from the Python Package Index, <https://pypi.org>. You can browse the Python Package Index by going to it in your web browser, or you can use pip’s limited search feature. 

Virtual Environments: 

 A virtual environment is an isolated Python environment where you can install packages and dependencies without affecting the global Python installation. This is useful to manage project-specific dependencies and versions. Different applications can then use different virtual environments. To resolve the earlier example of conflicting requirements, application A can have its own virtual environment with version 1.0 installed while application B has another virtual 

environment with version 2.0. If application B requires a library be upgraded to version 3.0, this will not affect application A’s environment. 

  

 Creating Virtual Environments: 

 To create a virtual environment, you can use the venv module (available in Python 3.3 and newer) or virtualenv (a third-party tool). Here's an example using venv. To create a virtual environment in Python, you can use the venv module, which is included in Python 3.3 and newer versions. 

  

 Floating Point Arithmetic: 

Floating-point arithmetic is a way to represent and perform arithmetic with real numbers (those that have a fractional part). In Python, floating-point numbers are represented as float data type. Floating-point numbers are represented in computer hardware as base 2 (binary) fractions. For example, the decimal fraction 0.125 has value 1/10 + 2/100 + 5/1000, and in the same way the binary fraction 0.001 has value 0/2 + 0/4 + 1/8. These two fractions have identical values, the only real difference being that the first is written in base 10 fractional notation, and the second in base 2. 

PyPI · The Python Package Index 

The Python Package Index (PyPI) is a repository of software for the Python programming language. 

 

3. Redirection: Python provides ways to redirect error output (`stderr`) to different destinations. This can be useful for logging errors, saving error messages to a file, or suppressing error output. 

 

    ```python 

    import sys 

 

    # Redirect stderr to a file 

    with open('error_log.txt', 'w') as f: 

        sys.stderr = f 

        # Your code generating errors 

    ``` 

 

4. Error Handling: Python also allows programmers to catch and handle errors using `try`, `except`, `finally` blocks to handle exceptions gracefully without the program terminating abruptly. 

 

### Program Termination: 

 

1. **Exceptions:** Errors or exceptional situations in Python trigger exceptions. If unhandled, exceptions can cause the program to terminate abruptly, displaying error messages to the console. 

 

2. Exception Handling: Python provides mechanisms like `try`, `except`, `finally` blocks to catch exceptions and execute specific code when an error occurs. This allows for graceful handling of errors without causing the program to crash. 

 

    ```python 

    try: 

        # Code that might raise an exception 

        result = 10 / 0 

    except ZeroDivisionError as e: 

        print(f"Error: {e}") 

        # Handle the exception gracefully 

    ``` 

 

3. Program Exit: The `sys.exit()` function can be used to terminate a Python program explicitly with an exit status code. A non-zero exit status typically indicates that an error occurred. 

 

    ```python 

    import sys 

 

    # Terminate program with an exit status 

    sys.exit(1)  # Exit with status code 1 (indicating an error) 

    ``` 

 

Python provides ways to manage error output redirection, allowing control over where error messages are displayed or logged. Additionally, handling exceptions gracefully using `try` and `except` blocks helps prevent abrupt program termination due to errors, enabling better control and response to exceptional situations. When necessary, the `sys.exit()` function can be used to terminate a program explicitly with an exit status code. 

 

 

 

How to Match Any Pattern of Text 

 

Matching any pattern of text in Python involves using regular expressions (regex) via the `re` module. Regular expressions allow you to define flexible patterns to search for and manipulate text data. 

 

#### Basic Steps to Match Any Pattern of Text using Regular Expressions: 

 

1. Import the `re` Module: Start by importing the `re` module, which provides functions and methods for working with regular expressions. 

 

    ```python 

    import re 

    ``` 

 

2. **Create a Regular Expression Pattern:** Define a regex pattern that represents the text pattern you want to match. Regular expressions use special characters and syntax to define patterns. 

 

    ```python 

    pattern = r'your_pattern_here' 

    ``` 

 

   - `r` before the string indicates a raw string literal in Python, which is often used with regex patterns to handle backslashes and special characters properly. 

 

3. **Use Functions/Methods for Pattern Matching:** 

 

   - **`re.search()`**: Searches for a pattern in a string and returns the first match found. 

 

        ```python 

        text = "Your text here" 

        match = re.search(pattern, text) 

        if match: 

            print("Pattern found:", match.group()) 

        else: 

            print("Pattern not found") 

        ``` 

 

   - **`re.findall()`**: Finds all occurrences of a pattern in a string and returns them as a list. 

 

        ```python 

        matches = re.findall(pattern, text) 

        if matches: 

            print("Pattern found:", matches) 

        else: 

            print("Pattern not found") 

        ``` 

 

   - **`re.match()`**: Checks if the pattern matches at the beginning of the string and returns a match object if found. 

 

        ```python 

        match = re.match(pattern, text) 

        if match: 

            print("Pattern found at the beginning:", match.group()) 

        else: 

            print("Pattern not found at the beginning") 

        ``` 

 

   - **`re.fullmatch()`**: Checks if the entire string matches the pattern and returns a match object if found. 

 

        ```python 

        match = re.fullmatch(pattern, text) 

        if match: 

            print("Entire string matches the pattern:", match.group()) 

        else: 

            print("Entire string does not match the pattern") 

        ``` 

 

4. **Regular Expression Patterns:** 

 

   - Regular expressions use special characters like `.` (matches any character), `*` (matches zero or more occurrences), `+` (matches one or more occurrences), `[]` (matches a character set), `^` (matches the start of a string), `$` (matches the end of a string), etc. 

 

   - You can combine these special characters and construct complex patterns to match specific text formats or structures. 

 

Regular expressions offer powerful text matching capabilities, allowing you to find patterns, validate data, extract information, and perform text manipulation tasks efficiently. Understanding regex syntax and experimenting with different patterns is key to effectively matching various text patterns in Python. 

 

## Day 3  

###Dates and Times, Data Compression, Performance Measurement, and Quality Control 

  

### Dates and Times in Python: 

Python provides the `datetime` module to handle dates and times.  

It offers classes like `datetime`, `date`, `time`, `timedelta`, etc., allowing manipulation, formatting, and arithmetic operations on dates and times.  

The `datetime` module also supports timezone handling, parsing, and formatting of date/time strings. 

  

### Data Compression in Python: 

Data compression refers to reducing the size of data to save storage space or transmission bandwidth.  

Python has libraries such as `zlib`, `gzip`, `bz2`, `lzma`, and `zipfile` that provide functionalities for compressing and decompressing data using various compression algorithms like DEFLATE, BZIP2, LZMA, and ZIP formats.  

These libraries enable reading and writing compressed files and streams. 

  

### Performance Measurement in Python: 

Python offers several modules and techniques for measuring the performance of code.  

The `timeit` module is commonly used to measure the execution time of small code snippets. 

 Profiling tools like `cProfile` or external profilers (e.g., `line_profiler`, `memory_profiler`) help identify performance bottlenecks, analyze memory usage, and optimize code for better performance. 

  

### Quality Control in Python: 

Quality control involves ensuring the reliability, correctness, and maintainability of software. 

 Python supports various testing frameworks like `unittest`, `pytest`, and `doctest` to automate testing and verify code functionality. Tools such as `flake8`, `pylint`, and `black` assist in code linting, style checking, and formatting adherence, promoting code consistency and readability. 

These topics are crucial in software development and data manipulation tasks in Python, providing functionalities to manage dates and times efficiently, compress and decompress data, measure code performance, and ensure code quality through testing and adherence to coding standards. 

 

 

Output formatting  

Python refers to the process of presenting data in a specific structure or style to enhance readability and convey information effectively.  

Python provides various methods and techniques for output formatting, including: 

  

### 1. String Formatting: 

   - **`str.format()` method:** This method allows inserting values into a string by specifying placeholders `{}` that are replaced with corresponding variables or values. 

   - **`f-strings` (formatted string literals):** Introduced in Python 3.6, f-strings provide a concise and readable way to embed expressions and variables directly within string literals using curly braces `{}`. 

  

### 2. `format()` Function: 

   - The `format()` function enables formatting data with more flexibility. It supports specifying formatting options for numbers, strings, and other data types, controlling precision, alignment, and padding. 

  

### 3. C-style String Formatting: 

   - Python also supports C-style string formatting using the `%` operator. However, this method is considered less preferred compared to the `str.format()` method or f-strings. 

  

### 4. Formatting Options: 

   - Formatting options allow controlling the appearance of output, such as specifying decimal places for floating-point numbers, aligning text, adding padding, converting values to different representations (e.g., hexadecimal, octal), and applying width and precision. 

  

### Example: 

```python 

name = "Alice" 

age = 30 

height = 5.8 

  

# Using f-strings 

print(f"Name: {name}, Age: {age}, Height: {height:.2f}") 

  

# Using str.format() method 

print("Name: {}, Age: {}, Height: {:.2f}".format(name, age, height)) 

  

# Using format() function 

print("Name: {0}, Age: {1}, Height: {2:.2f}".format(name, age, height)) 

  

# C-style string formatting 

print("Name: %s, Age: %d, Height: %.2f" % (name, age, height)) 

```  

Output formatting in Python offers flexibility and readability, allowing developers to present data in a structured and easily understandable manner according to specific requirements.  

The choice of formatting method often depends on personal preference, code readability, and compatibility with Python versions. 


