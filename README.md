# Getting Started With Python (basic syntax & data types)

<a href="http://creativecommons.org/licenses/by-nc/4.0/" rel="license"><img style="border-width: 0;" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" alt="Creative Commons License" /></a>This tutorial was written by Katherine Walden and is licensed under a <a href="http://creativecommons.org/licenses/by-nc/4.0/" rel="license">Creative Commons Attribution-NonCommercial 4.0 International License</a>.

## Lab Overview & Goals

This lab provides an overview of foundational programming concepts, with a focus on Python syntax. Topics covered include:
- Variables & assignment operators
- Basic data types & comments
- Arithmetic operators
- Concatenation
- Input/Output
- Relational or comparison operators
- Boolean logic & logical operators

## Acknowledgements

Portions of this lab are adapted from the ["Lab: Programming in Python"](https://www.cs.grinnell.edu/~davisjan/csc/105/2012S/labs/python1.html) and ["Lab: Numbers in Python"](https://www.cs.grinnell.edu/~davisjan/csc/105/2012S/labs/python2.html) lab materials developed by [Janet Davis](https://cs.whitman.edu/~davisj/) for the the [CSC 105 "The Digital Age" course](https://www.cs.grinnell.edu/~davisjan/csc/105/2012S/). 

This lab also incorporates elements of [Corey Pennycuff's](https://www3.nd.edu/~cpennycu/) ["Intro to Python/Jupyter" Jupyter notebook](https://www3.nd.edu/~cpennycu/2019/assets/fall/EOC/19.08.29.ipynb) from [CSE 10101 Elements of Computing (Fall 2019)](https://www3.nd.edu/~cpennycu/2019/fa-CSE10101-CDT30010.html).

Definitions and explanations in this lab are adapted from:
- W3Schools, [Python tutorials and documentation](https://www.w3schools.com/python/)
- Kenneth Leroy Busbee and Dave Braunschweig, *[Programming Fundamentals: A Modular Structured Approach, 2nd Edition](https://press.rebus.community/programmingfundamentals/)* (Rebus Press, 2018)

# Table of Contents
- [Key Concepts](#key-concepts)
- [Lab Notebook Template](#lab-notebook-template)
- [Your First Program](#your-first-program)
  * [Data Types](#data-types)
  * [Comments](#comments)
  * [Running Your Program](#running-your-program)
- [Variables & Assignment Operators](#variables--assignment-operators)
- [Arithmetic Operators](#arithmetic-operators)
- [Concatenation](#concatenation)
- [Input & Output (I/O)](#input--output-io)
- [Converting Data Types](#converting-data-types)
- [Comparison Operators](#comparison-operators)
- [How to submit this lab (and show your work)](#how-to-submit-this-lab-and-show-your-work)
- [Lab Notebook Questions](#lab-notebook-questions)

[Click here](https://colab.research.google.com/drive/1HYwPZ6MkpYDe4QIXVVzXM4M13hA26ufL?usp=sharing) to access this lab procedure as a Jupyter Notebook.

## Key Concepts

[Click here](https://github.com/kwaldenphd/python-intro/blob/main/key-concepts.md) for a full list of key concepts and definitions for this lab.

## Lab Notebook Template

[Click here](https://replit.com/team/eoc-f23/Python-Fundamentals) to make a copy of the Replit template for this lab.

Alternatives:
- `.py placeholder
- `ipynb` placeholder

## How to submit this lab (and show your work)

Moving forward, we'll submit lab notebooks as `.py` files. 

One option is to have a `.py` file that you use to run code and test programs while working through the lab. When ready to submit the lab notebook, you add comments and remove extraneous materials.

Another option is to have an "official" `.py` file that you are using as a lab notebook (separate from your working/testing file). Use comments in Python to note when you are starting a new question (as well as answering a question).
  * Example: `Lab_Notebook_Walden.py`

What gets submitted as the lab notebook is the `Lab_Notebook_Walden.py` file.
- When in doubt, use comments
- Be sure you are using comments to note what question you're responding to

# Your First Program

## Data Types

"A data type is a classification of data which tells the compiler or interpreter how the programmer intends to use the data. Most programming languages support various types of data, including integer, real, character or string, and Boolean" (Kenneth Leroy Busbee and Dave Braunschweig, "[Data Types](https://press.rebus.community/programmingfundamentals/chapter/data-types/)" in *Programming Fundamentals*)

How a programming language recognizes or understands the type of information shapes how it executes specific commands or operations.

Commonly-used data types (with Python examples) include:

<table><tr><th>Name</th><th>Python Syntax</th><th>Example</th><th>Description</th></tr>
  <tr><td>String</td><td><code>str()</code><td><code>"Hello World!"</code></td><td>String of characters</td></tr>
  <tr><td>Integer</td><td><code>int()</code><td><code>7</code></td><td>Whole number</td></tr>
  <tr><td>Float</td><td><code>float()</code><td><code>1.5</code></td><td>Decimal number, or number with floating point values</td></tr>
  <tr><td>Boolean</td><td><code>bool()</code><td><code>True</code></td><td>Two-state system that typically represents true/false values</td></tr>
  <tr><td>Nothing/Null/NoneType</td><td><code>NoneType</code><td><code>None</code></td><td>No value</td></tr> 
  </table>
  
More on data types, from Busbee and Braunschweig's *[Coding Fundamentals](https://press.rebus.community/programmingfundamentals)*:
- [Integer](https://press.rebus.community/programmingfundamentals/chapter/integer-data-type/)
- [Floating Point](https://press.rebus.community/programmingfundamentals/chapter/floating-point-data-type/)
- [String](https://press.rebus.community/programmingfundamentals/chapter/string-data-type/)
- [Boolean](https://press.rebus.community/programmingfundamentals/chapter/boolean-data-type/)
- [Nothing](https://press.rebus.community/programmingfundamentals/chapter/nothing-data-type/)

For more on data types in Python:
- [W3Schools, Python Data Types](https://www.w3schools.com/python/python_datatypes.asp)

We can use the `type()` function in Python to check an object or value's data type.
- `type` is the function name
- The value or information we are passing to the function goes inside the parenthesis

```Python
# a type example
type("Hello world!")
```

## Comments

Comments mark instructions or information in the code that will not run as part of the program. Comments are useful for testing, documenting, and describing what your code is doing. 

In Python, single line comments begin with a pound `#` symbol and multi-line comments are marked by three sets of double quotation marks `"""`.

```Python
# This is an example of a single line comment in Python

"""
This is an example of a multi-line comment in Python
"""
```

For more on comments in Python:
- [W3Schools, Python Comments](https://www.w3schools.com/python/python_comments.asp)

## Running Your Program

Earlier in the semester, we wrote an assembly language program that ran when we pressed the `Execute` button.

In most programming languages, there are a few common options for how you run or execute specific lines of code, sections of code, or an entire program.

<p align="center"><img src="https://github.com/kwaldenphd/python-intro/blob/main/images/Replit_Python_Screenshot.png?raw=true" width="1000"></p>

Most integrated development environments (IDEs) include two locations where you can execute code:
- We can type commands and run programs in the **console**, but those instructions are not saved and aren't available outside the current working session.
- We can also type commands and run programs in a **script**. This is a file that is saved as part of the project/workspace. It's available outside the current working session and can be reopened, modified, or executed (as an entire program).

A couple other notes on consoles and scripts:
- When we run a piece of code in our script, the output or result will be shown in the console.
- We can also run an entire script at the command line (i.e. `python main.py`)

## Comprehension Check

<table>
 <tr><td>
<img src="https://github.com/kwaldenphd/internet/blob/main/images/clipboard.png?raw=true" alt="Clipboard icon" width="50"/></td>
  <td><a href="https://docs.google.com/forms/d/e/1FAIpQLSdhdGEhhGB1wcx4BSRS7xGRG3yV8jKy3YXaISk1FEjCA4-W9w/viewform?usp=sf_link">Data Types & the IDE Comprehension Check</a></td>
  </tr>
  </table>

# Variables & Assignment Operators

In most programming languages, variables work as "containers for storing data values" ([W3Schools, Python Variables](https://www.w3schools.com/python/python_variables.asp))

We create a variable by assigning a value to that variable name using an **assignment operator**.

"An assignment statement sets and/or re-sets the value stored in the storage location(s) denoted by a variable name; in other words, it copies a value into the variable...The assignment operator has two operands. The one to the left of the operator is usually an identifier name for a variable. The one to the right of the operator is a value" (Kenneth Leroy Busbee and Dave Braunschweig, "[Assignment](https://press.rebus.community/programmingfundamentals/chapter/assignment/)" in *Programming Fundamentals*)

```
[identifier] [assignment symbol] [value]
```

In Python, the equals sign `=` is the assignment symbol. The underlying syntax for creating a variable in Python using an assignment statement:

```Python
# general syntax
identifier = value

# simple variable example
x = 7

# composite variable example
y = 5 + 7
```

Python has a few restrictions and best practices around variable identifiers or names:

#1- They have to start with a letter character or an underscore (no symbols or numeric characters)

```Python
# example of a valid identifier
x = 7

# example of an invalid identifier
$x = 7
```

#2: Terms that have other meaning or function in Python can't be used as variable identifiers. For example the name of a built-in function (`type`) can't be used as a variable identifier.

Reserved keywords in Python include: `and, except, lambda, with, as, finally, nonlocal, while, assert, fale, None, yield, break, for, not, class, from, or, continue, global, pass, def, if, raise, del, import, return, elif, in, True, else, is, try`

#3: Best practice is any programming language is to use meaningful variable identifiers. Just calling something `x` or `y` won't be particularly helpful to someone else reading or interacting with your code. That said, overly-complex variable identifiers are prone to user error.

We can show the value for a variable using Python's `print()` function.

```Python
# assignment statement
x = 7

# show variable value
print(x)
```

We can also show a variable's data type using the `type()` function.

```Python
# assignment statement
y = "Hello world!"

# show type
type(y)
```

## Comprehension Check

<table>
 <tr><td>
<img src="https://github.com/kwaldenphd/internet/blob/main/images/clipboard.png?raw=true" alt="Clipboard icon" width="50"/></td>
  <td><a href="https://docs.google.com/forms/d/e/1FAIpQLScZ06JksFcjjrgt1IdbPD1IS38ZLItdonFwg6G-vL-fCUflPg/viewform?usp=sf_link">Variables & Assignment Operators Comprehension Check</a></td>
  </tr>
  </table>

## Application

Q1: Create a named variable for each of the following data types.
- Integer
- Float
- String
- Boolean

Show the value of each variable using `print()` and check the type of each variable using `type()`.

Answer to this question includes program + comments that document process and explain your code.

# Arithmetic Operators

Most programming languages allow you to perform arithmetic operations and mathematical calculations using **arithmetic operators**.

Common arithmetic operations (with Python examples) include:

<table><tr><th>Name</th><th>Python Syntax</th><th>Python Example</th><th>Description</th></tr>
  <tr><td>Addition</td><td><code>+</code><td><code>5 + 6</code></td><td>Adds values</td></tr>
  <tr><td>Subtraction</td><td><code>-</code><td><code>5 - 6</code></td><td>Subtracts values</td></tr>
  <tr><td>Multiplication</td><td><code>*</code><td><code>5 * 6</code></td><td>Multiples values</td></tr>
  <tr><td>Integer division</td><td><code>//</code><td><code>5 // 6</code></td><td>Divides values, integers (whole numbers)</td></tr> 
  <tr><td>Float division</td><td><code>/</code><td><code>5 / 6</code></td><td>Divides values, floating point numbers (decimal values)</td></tr>
  <tr><td>Modulo</td><td><code>%</code><td><code>5 % 6</code></td><td>Returns or retrieves remainder (whole number) from division operation</td></tr>  
  <tr><td>Exponent</td><td><code>**</code><td><code>5 ** 6</code></td><td>Calculates exponent</td></tr>
  </table>
  
More on arithmetic operators (in general): "[Arithmetic Operators](https://press.rebus.community/programmingfundamentals/chapter/arithmetic-operators/)" from Busbee and Braunschweig's *[Coding Fundamentals](https://press.rebus.community/programmingfundamentals)*:

For more on arithmetic operators in Python:
- [W3Schools, Python Arithmetic Operators](https://www.w3schools.com/python/gloss_python_arithmetic_operators.asp)

We can run arithmetic operations directly in the console or in a script.

```Python
# sample arithmetic operation
5 + 7
```

But we can also assign the output of an arithmetic operation to a variable.

```Python
# sample arithmetic operation where output is assigned to variable
x = 5 + 7

# show variable value
print(x)
```

<p align="center"><img src="https://github.com/kwaldenphd/python-intro/blob/main/images/PEDMAS.png?raw=true" width="500"></p>

Python follows the PEDMAS order of operations: parenthesis, exponents, multiplication, division, addition, subtraction. 
- *When in doubt, use parenthesis!*

## Comprehension Check

<table>
 <tr><td>
<img src="https://github.com/kwaldenphd/internet/blob/main/images/clipboard.png?raw=true" alt="Clipboard icon" width="50"/></td>
  <td><a href="https://docs.google.com/forms/d/e/1FAIpQLSel1Y3UC27V97ChdRtXeWIUXBsQ0SR8vW9w2R5IqQE7yXBhww/viewform?usp=sf_link">Arithmetic Operators Comprehension Check</a></td>
  </tr>
  </table>

## Application

Q2: Write programs (or a single program) that use each of the following arithmetic operators.
- Addition
- Subtraction
- Multiplication
- Division
- Modulus
- Exponents

You can write separate calculations with single operators, or calculations that use multiple operators.

Answer to this question includes program + comments that document process and explain your code.

Q3: Write a program that uses arithmetic operators to convert a specific Farenheit temperature value and output its Celsius representation. Answer to this question includes program + comments that document process and explain your code.

<blockquote>The conversion equation is: <code>celsius = (fahrenheit - 32.0) * 5.0 / 9.0</code></blockquote>

# Concatenation

In most programming languages, **concatenation** involves adding or joining character strings.

For example, we could concatenate the strings `Hello` and `world` to create a `Hello world` message.

In Python, we use the plus sign `+` to concatenate strings.

One option is to use concatenation as part of a `print()` statement:

```Python
# concatenation in a print statement
print("Hello " + "World!")
```

We can also use concatenation with string variables.

```Python
# concatenation with string variables
x = "Hello"
y = "World"

# concatenation with a print statement
print(x + y)

# conatenation with variable assignment
z = x + y
print(z)
```

We can compare string concatenation to how the addition operator (`+`) interacts with numeric values.

```Python
# numeric 'concatenation' in a print statement
print(5 + 7)

# numeric 'concatenation' with variable assignment
x = 5
y = 7
z = x + y
print(z)
```

NOTE: In Python, concatenation operations or the `+` operator will only work on variables or values of a common type.

```Python
# trying concatenation with an integer and string
year = 2023
school = "Notre Dame"

print(school + ", Class of " + year)
```

Later in this lab, we'll talk about how to convert data types to address this issue.

## Comprehension Check

<table>
 <tr><td>
<img src="https://github.com/kwaldenphd/internet/blob/main/images/clipboard.png?raw=true" alt="Clipboard icon" width="50"/></td>
  <td><a href="https://docs.google.com/forms/d/e/1FAIpQLScFQQp8Hb0H3j-obJSPVjQf_wpdaYXOUBmoIlbrN4wDtaBBRQ/viewform?usp=sf_link">Concatenation Comprehension Check</a></td>
  </tr>
  </table>

## Application

Q5: Write a program that creates `first_name` and `last_name` variables, and then uses concatenation to create (and then print) a `full_name` variable. Answer to this question includes program + comments that document process and explain your code.

Q6: Create variables for each of the discrete pieces of information in "the standard Notre Dame introduction."
- Name
- Class year
- Home state/country
- Major(s) / minor(s)
- Residence hall

Use concatenation in combination with a `print()` statement to output a narrative introduction using the named variables.

Answer to this question includes program + comments that document process and explain your code.

Sample output for this program:
```
I'm Knute Rockne, class of 1914. I'm majoring in pharmacy and originally from Norway but grew up in Chicago. I live in Sorin Hall.
```

# Input & Output (I/O)

In programming languages and computing more broadly, `I/O` stands for `Input` and `Output`.

We've seen `I/O` at work in previous labs, where we provided inputs to the computer (using a CPU simulator or working at the terminal), a task or operation was performed, and there was an endpoint or output for that process.

A concrete example would be the assembly language program we wrote for Lab #2: How Comptuters Work (Hardware). We wrote assembly language instructions which served as inputs for the fetch-execute cycle, and the final output for the program was a data value stored in main memory.

Similarly, programming languages can take a variety of inputs (user-provided values, data, files, etc) and return outputs in a variety of formats (data stored in memory, output that shows up in the console, newly-created or -modified files, etc).

In future labs, we'll do more with with aspects of `I/O` that have to do with reading and writing files. But for now, we've already seen `I/O` in action in Python via `print()` statements.

One way Python accepts input is via the `input()` function, which accepts a user input and assigns that to a variable.

A sample program that asks a user to enter their name:

```Python
# initial prompt
print("Enter your name: ")

# input function
name = input()

# output statement
print("Hello, " + name)
```

We can modify that program to include the initial prompt as part of the `input()` statement.

```Python
# initial prompt with input function
name = input("Enter your name: ")

# output
print("Hello, " + name)
```

NOTE: The default data type for a variable created using the `input()` function is a string object. We can change data types using the functions we'll cover later in this lab.

More on Python's `input()` function:
- [W3Schools, Python input() Function](https://www.w3schools.com/python/ref_func_input.asp)

## Comprehension Check

<table>
 <tr><td>
<img src="https://github.com/kwaldenphd/internet/blob/main/images/clipboard.png?raw=true" alt="Clipboard icon" width="50"/></td>
  <td><a href="https://docs.google.com/forms/d/e/1FAIpQLSe83StYhYCVwUUt3kSSNImGjP8sHS9JfKDjlfSUrGFQNUn3AA/viewform?usp=sf_link">I/O Comprehension Check</a></td>
  </tr>
  </table>

## Application

Q7: Write a program that asks the user to enter their favorite color, and then prints a `"Your favorite color is..."` message. Answer to this question includes program + comments that document process and explain your code.

Q8: Write a program that accepts user input for the discrete pieces of information in "the standard Notre Dame introduction."
- Name
- Class year
- Home state/country
- Major(s) / minor(s)
- Residence hall

Use concatenation in combination with a `print()` statement to output a narrative introduction using the named variables.

Answer to this question includes program + comments that document process and explain your code.

Sample output for this program:
```
Knute Rockne, class of 1918, is majoring in pharmacy. He is originally from Norway but grew up in Chicago. He lives in Sorin Hall.
```

# Converting Data Types

Earlier in this lab we used arithmetic operators to develop a Fahrenheit - Celsius temperature conversion formula. Imagine a scenario in which we want to convert a user-provided temperature.

We could use the `input()` function and then pass that input value to our conversion formula. Let's try it.

```Python
temp = input("Enter a temperature in Fahrenheit: ")

# conversion formula
celsius = (temp - 32) * (5/9)

# show celsius output
print(temp + " degrees in Fahrenheit is " + celsius + " degrees in Celsius")
```

Except this program results in a `TypeError`. In Python, this is a data type error indicating we're trying to perform an operation that's not compatible with the data types we're using.

Python includes built-in functions that let us convert specific data types.

<table><tr><th>Name</th><th>Python Syntax</th><th>Example</th><th>Description</th></tr>
  <tr><td>String</td><td><code>str()</code><td><code>"Hello World!"</code></td><td>String of character</td></tr>
  <tr><td>Integer</td><td><code>int()</code><td><code>7</code></td><td>Whole number</td></tr>
  <tr><td>Float</td><td><code>float()</code><td><code>1.5</code></td><td>Decimal number, or number with floating point values</td></tr>
  <tr><td></td>Boolean<td><code>bool()</code><td><code>True</code></td><td>Two-state system that typically represents true/false values</td></tr>
  <tr><td>Nothing/Null/NoneType</td><td><code>NoneType</code><td><code>None</code></td><td>No value</td></tr> 
  </table>

Remember our program from the [Concatenation](#concatenation) section of the lab:

```Python
# trying concatenation with an integer and string
year = 2023
school = "Notre Dame"

print(school + ", Class of " + year)
```

We can use the `str()` function to convert `year` from an integer to a string object. That will allow the final `print()` statement to run.

```Python
# assign year variable
year = 2023

# convert to string
year = str(year)

# assign school variable
school = "Notre Dame"

# output
print(school + ", Class of " + year)
```

We could combine the first two lines of this program to convert the data type when we create the variable.

```Python
# assign year variable and convert to string
year = str(2023)

# assign school variable
school = "Notre Dame"

# output
print(school + ", Class of " + year)
```

An alternate workflow for instructing Python to treat `2023` as a string of characters:

```Python
# assign year variable as string
year = "2023"

# assign school variable
school = "Notre Dame"

# output
print(school + ", Class of " + year)
```

## Comprehension Check

<table>
 <tr><td>
<img src="https://github.com/kwaldenphd/internet/blob/main/images/clipboard.png?raw=true" alt="Clipboard icon" width="50"/></td>
  <td><a href="https://docs.google.com/forms/d/e/1FAIpQLSd-ZmsE0NYbCz3pLsuAx0f5a9E2rWeC8FryIhI6KBS_KJjP-Q/viewform?usp=sf_link">Converting Data Types Comprehension Check</a></td>
  </tr>
  </table>

## Application

Q9: Write a program that prompts the user to enter two numbers, converts the input values to integers, adds them, and reports the result. Answer to this question includes program + comments that document process and explain your code.

Q10: Write a program that asks the user to think of a month and then enter the number of days in that month. Your program should then compute the number of minutes in the month, and report the result. Answer to this question includes program + comments that document process and explain your code.

Q11: Write a program that prompts the user to enter a temperature in Fahrenheit, and reports the equivalent temperature in Celsius. Answer to this question includes program + comments that document process and explain your code.

# Comparison Operators

"The relational operators are often used to create a test expression that controls program flow. This type of expression is also known as a Boolean expression because they create a Boolean answer or value when evaluated. There are six common relational operators that give a Boolean value by comparing (showing the relationship) between two operands. If the operands are of different data types, implicit promotion occurs to convert the operands to the same data type" (Busbee, "[Relational Operators](https://press.rebus.community/programmingfundamentals/chapter/relational-operators/)", in *Programming Fundamentals*)

Relational operators, also called comparison operators, allow us to run `True/False` tests on specific conditions, focusing on the relationship(s) between two or more values.

Relational operators or comparison operators in Python: 

<table><tr><th>Name</th><th>Syntax</th><th>Example</th><th>Description</th></tr>
  <tr><td>Equal</td><td><code>==</code><td><code>x == y</code></td><td>Tests if values are equal</td></tr>
  <tr><td>Not equal</td><td><code>!=</code><td><code>x != y</code></td><td>Tests if values are not equal</td></tr>
  <tr><td>Greater than</td><td><code>></code><td><code>x > y</code></td><td>Tests is a value is greater than another</td></tr>
  <tr><td>Less than</td><td><code><</code><td><code>x < y</code></td><td>Tests is a value is less than another</td></tr> 
  <tr><td>Greater than or equal to</td><td><code>>=</code><td><code>x >= y</code></td><td>Tests if a value is greater than or equal to another</td></tr>
  <tr><td>Less than or equal to</td><td><code><=</code><td><code>x <= y</code></td><td>Tests if a value is less than or equal to another</td></tr>  
  </table>
    
For more on comparison operators in Python: [W3Schools, Python Comparison Operators](https://www.w3schools.com/python/gloss_python_comparison_operators.asp)

## Boolean Logic

- "In mathematics and mathematical logic, Boolean algebra is the branch of algebra in which the values of the variables are the truth values true and false, usually denoted 1 and 0" ([Wikipedia](https://en.wikipedia.org/wiki/Boolean_algebra))

We've talked previously about the Boolean data type. The underlying `True`/`False` logic lets us test for specific conditions and then specify how our code will execute based on the truth value for those conditional statements.

- "You can evaluate any expression in Python, and get one of two answers, `True` or `False`. When you compare two values, the expression is evaluated and Python returns the Boolean answer" ([W3Schools, Python Booleans](https://www.w3schools.com/python/python_booleans.asp))

## Boolean Logic & Comparison Operators
   
We can use comparison operators with a `print()` statement to test whether a particular statement is `True` or `False`.
   
A couple Python examples:

```Python
print(4 == 5) # returns false
print(6 < 10) # returns true
```

```Python
# comparison operator using variables
x = 5
y = 6

print(x > y) # returns false
```

## Comparison Operators & String Objects

We can probably make intuitive sense of how these comparison operators would work for numeric values. But what about text characters or string objects?
   
Most programming languages treat the 26 characters in the English-language alphabet (`a-z`) as sequential values, where `a` is less than `b`, which is less than `c`, etc.

When working with string objects that represent words or characters, comparison operators indicate positionality in the English-language alphabet.

A few examples in Python:
```
print("apple" > "banana") # returns false

print("Ohio State" > "Notre Dame") # returns true
```   

## Comprehension Check

<table>
 <tr><td>
<img src="https://github.com/kwaldenphd/internet/blob/main/images/clipboard.png?raw=true" alt="Clipboard icon" width="50"/></td>
  <td><a href="https://docs.google.com/forms/d/e/1FAIpQLSd20NlXelKfF3hS5ftvjJAPG_Db7uMbnODfIT8dGZ39fP5EaA/viewform?usp=sf_link">Comparison Operators Comprehension Check</a></td>
  </tr>
  </table>

## Application

Q12: Write a program that uses each of Python's comparison operators (`==, !=, >, <, >=, <=`) to compare two numeric values. Answer to this question includes program + comments that document process and explain your code.

Outline for this program:
```
# first numeric value

# second numeric value

# equal

# not equal

# greater than

# less than

# greater than or equal to

# less than or equal to

```

Q13: Write a program that uses each of Python's comparison operators (`==, !=, >, <, >=, <=`) to compare two string objects. Answer to this question includes program + comments that document process and explain your code.

Outline for this program:
```
# first string object

# second string object

# equal

# not equal

# greater than

# less than

# greater than or equal to

# less than or equal to

```

Q14: Write a program that asks a user to enter their age and returns an output message comparing that value with your age. This program will use a combination of the `input()` function, comparison operators, and `if-then-else` logic. Answer to this question includes program + comments that document process and explain your code.

Sample output for this program:
```
Your age: 10

My age: 12

I am older!
```

# How to submit this lab (and show your work)

Moving forward, lab notebooks will be submitted as `.py` files. 

One option is to have a `.py` file that you use to run code and test programs while working through the lab. When ready to submit the lab notebook, you add comments and remove extraneous materials.

Another option is to have an "official" `.py` file that you are using as a lab notebook (separate from your working/testing file). Use comments in Python to note when you are starting a new question (as well as answering a question).
- Example: `Lab5_Notebook_Walden.py`

What gets submitted as the lab notebook is the `Lab5_Notebook_Walden.py` file.
- When in doubt, use comments
- Be sure you are using comments to note what question you're responding to

# Lab Notebook Questions

[Click here](https://replit.com/team/eoc-f22/Introduction-to-Python) to make a copy of the Replit template for this lab.

Alternatives:
- [`.py` template](https://drive.google.com/file/d/1usNaA299oB63ruoruBXlhtIT78Ie6D1j/view?usp=sharing) (Google Drive, ND users)
- [Jupyter Notebook, `.ipynb`](https://colab.research.google.com/drive/1yiBlBqUlWLjX4MisZCJFRmatdBAsbWb5?usp=sharing) (Google Colab, ND users)

Q1: Create a named variable for each of the following data types.
- Integer
- Float
- String
- Boolean

Show the value of each variable using `print()` and check the type of each variable using `type()`.

Answer to this question includes program + comments that document process and explain your code.

Q2: Write programs (or a single program) that use each of the following arithmetic operators.
- Addition
- Subtraction
- Multiplication
- Division
- Modulus
- Exponents

You can write separate calculations with single operators, or calculations that use multiple operators.

Answer to this question includes program + comments that document process and explain your code.

Q3: Write a program that uses arithmetic operators to convert a specific Farenheit temperature value and output its Celsius representation. Answer to this question includes program + comments that document process and explain your code.

<blockquote>The conversion equation is: <code>celsius = (fahrenheit - 32.0) * 5.0 / 9.0</code></blockquote>

Q4: Write a program that calculates the fewest number of U.S. coins needed to make change for a 73 cent remainder. To put that another way- write a program that determines the smallest number of coins in each U.S. denomination needed to make up 73 cents. Answer to this question includes program + comments that document process and explain your code.

In U.S. currency, one dollar ($1.00) equals one hundred (100) cents. The coins used to make change have a face value in cents.

- Quarter = 25 cents
- Dime = 10 cents
- Nickel = 5 cents
- Penny = 1 cent

Q5: Create variables for each of the discrete pieces of information in "the standard Notre Dame introduction."
- Name
- Class year
- Home state/country
- Major(s) / minor(s)
- Residence hall

Use concatenation in combination with a `print()` statement to output a narrative introduction using the named variables.

Answer to this question includes program + comments that document process and explain your code.

Sample output for this program:
```
I'm Knute Rockne, class of 1914. I'm majoring in pharmacy and originally from Norway but grew up in Chicago. I live in Sorin Hall.
```

Q6: Write a program that creates `first_name` and `last_name` variables, and then uses concatenation to output a `full_name` variable. Answer to this question includes program + comments that document process and explain your code.

Q7: Write a program that asks the user to enter their favorite color, and then prints a `"Your favorite color is..."` message. Answer to this question includes program + comments that document process and explain your code.

Q8: Write a program that accepts user input for the discrete pieces of information in "the standard Notre Dame introduction."
- Name
- Class year
- Home state/country
- Major(s) / minor(s)
- Residence hall

Use concatenation in combination with a `print()` statement to output a narrative introduction using the named variables.

Answer to this question includes program + comments that document process and explain your code.

Sample output for this program:
```
Knute Rockne, class of 1918, is majoring in pharmacy. He is originally from Norway but grew up in Chicago. He lives in Sorin Hall.
```

Q9: Write a program that prompts the user to enter two numbers, converts the input values to integers, adds them, and reports the result. Answer to this question includes program + comments that document process and explain your code.

Q10: Write a program that asks the user to think of a month and then enter the number of days in that month. Your program should then compute the number of minutes in the month, and report the result. Answer to this question includes program + comments that document process and explain your code.

Q11: Write a program that prompts the user to enter a temperature in Fahrenheit, and reports the equivalent temperature in Celsius. Answer to this question includes program + comments that document process and explain your code.
