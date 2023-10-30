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

2. Selection/Decision control statements

 In Python, the selection statements are also known as Decision control statements or branching statements.

 The selection statement allows a program to test several conditions and execute instructions based on which condition is true.

Some Decision Control Statements are:

Simple if

if-else

nested if

if-elif-else

Simple if: If statements are control flow statements that help us to run a particular code, but only when a certain condition is met or satisfied. A simple if only has one condition to check.

