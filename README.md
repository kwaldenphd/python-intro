# Getting Started With Python (basic syntax & data types)

<a href="http://creativecommons.org/licenses/by-nc/4.0/" rel="license"><img style="border-width: 0;" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" alt="Creative Commons License" /></a>This tutorial was written by Katherine Walden and is licensed under a <a href="http://creativecommons.org/licenses/by-nc/4.0/" rel="license">Creative Commons Attribution-NonCommercial 4.0 International License</a>.

## Lab Overview & Goals


<table>
 <tr><td>
<img src="https://elearn.southampton.ac.uk/wp-content/blogs.dir/sites/64/2021/04/PanPan.png" alt="Panopto logo" width="50"/></td>
<td><a href="https://notredame.hosted.panopto.com/Panopto/Pages/Viewer.aspx?pid=ff776195-c52e-4083-b903-aef40171360f">Lecture/Live Coding Playlist</a></td>
  </tr>
  </table>

## Acknowledgements

Severance Python For Everyone

W3Schools Python tutorials

Portions of this lab are adapted from the ["Lab: Programming in Python"](https://www.cs.grinnell.edu/~davisjan/csc/105/2012S/labs/python1.html) and ["Lab: Numbers in Python"](https://www.cs.grinnell.edu/~davisjan/csc/105/2012S/labs/python2.html) lab materials developed by [Janet Davis](https://cs.whitman.edu/~davisj/) for the the [CSC 105 "The Digital Age" course](https://www.cs.grinnell.edu/~davisjan/csc/105/2012S/). 

This lab also incorporates elements of [Corey Pennycuff's](https://www3.nd.edu/~cpennycu/) ["Intro to Python/Jupyter" Jupyter notebook](https://www3.nd.edu/~cpennycu/2019/assets/fall/EOC/19.08.29.ipynb) from [CSE 10101 Elements of Computing (Fall 2019)](https://www3.nd.edu/~cpennycu/2019/fa-CSE10101-CDT30010.html).

(Kenneth Leroy Busbee and Dave Braunschweig, "[Data Types](https://press.rebus.community/programmingfundamentals/chapter/data-types/)" in *Programming Fundamentals*)

# Table of Contents
- [Lecture & Live Coding](#lecture--live-coding)
- [Key Concepts](#key-concepts)
- [Lab Notebook Template](#lab-notebook-template)

## Lecture & Live Coding

Throughout this lab, you will see a Panopto icon at the start of select sections.

This icon indicates there is lecture/live coding asynchronous content that accompanies this section of the lab. 

You can click the link in the figure caption to access these materials (ND users only).

Example:

<table>
 <tr><td>
<img src="https://elearn.southampton.ac.uk/wp-content/blogs.dir/sites/64/2021/04/PanPan.png" alt="Panopto logo" width="50"/></td>
<td><a href="https://notredame.hosted.panopto.com/Panopto/Pages/Viewer.aspx?pid=ff776195-c52e-4083-b903-aef40171360f">Lecture/Live Coding Playlist</a></td>
  </tr>
  </table>

## Key Concepts

[Click here](https://github.com/kwaldenphd/python-intro/blob/draft/key-concepts.md) for a full list of key concepts and definitions for this lab.

## Lab Notebook Template

[Click here]() to make a copy of the Replit template for this lab.

Alternatives:
- [`.py` template]()
- [Jupyter Notebook, `.ipynb`]()

## How to submit this lab (and show your work)

Moving forward, we'll submit lab notebooks as `.py` files. 

One option is to have a `.py` file that you use to run code and test programs while working through the lab. When ready to submit the lab notebook, you add comments and remove extraneous materials.

Another option is to have an "official" `.py` file that you are using as a lab notebook (separate from your working/testing file). Use comments in Python to note when you are starting a new question (as well as answering a question).
  * Example: `Lab_Notebook_Walden.py`

What gets submitted as the lab notebook is the `Lab_Notebook_Walden.py` file.
- When in doubt, use comments
- Be sure you are using comments to note what question you're responding to

# How We Got to Python / Why Programming Languages

<table>
<tr><td><img src="https://elearn.southampton.ac.uk/wp-content/blogs.dir/sites/64/2021/04/PanPan.png" alt="Panopto logo" width="50"/></td></tr>
<tr><td><a href="https://notredame.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=6b873ef6-c961-4ac1-a493-ae5801666f17">Your First Program</a></td></tr></table>

## Key Terms


## Comprehension Check

# Your First Program

## Data Types

"A data type is a classification of data which tells the compiler or interpreter how the programmer intends to use the data. Most programming languages support various types of data, including integer, real, character or string, and Boolean" (Kenneth Leroy Busbee and Dave Braunschweig, "[Data Types](https://press.rebus.community/programmingfundamentals/chapter/data-types/)" in *Programming Fundamentals*)

How a programming language recognizes or understands the type of information shapes how it executes specific commands or operations.

Commonly-used data types (with Python examples) include:

<table><tr><th>Name</th><th>Python Syntax</th><th>Example</th><th>Description</th></tr>
  <tr><td>String</td><td><code>str()</code><td><code>"Hello World!"</code></td><td>String of character</td></tr>
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

REPLIT SCREENSHOT

Most integrated development environments (IDEs) include two locations where you can execute code:
- We can type commands and run programs in the **console**, but those instructions are not saved and aren't available outside the current working session.
- We can also type commands and run programs in a **script**. This is a file that is saved as part of the project/workspace. It's available outside the current working session and can be reopened, modified, or executed (as an entire program).

A couple other notes on consoles and scripts:
- When we run a piece of code in our script, the output or result will be shown in the console.
- We can also run an entire script at the command line (i.e. `python main.py`)

## Comprehension Check

Console vs shell vs script

Int vs float

String vs Boolean

Specific examples:
- is `"7"` different than `7` (how)
- is `"True"` different than `True` (and how)

# Variables & Assignment Operators

In most programming languages, variables work as "countainers for storing data values" ([W3Schools, Python Variables](https://www.w3schools.com/python/python_variables.asp))

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

What are variables, what do they do

How do we create variables in Python, assignment statement

Rules for variable names

## Application

QX: Create named variable for each data type in Python using assignment operator

Check using `print` and `type`

Answers need to include assignment statement and print/type for each data type
- Int
- Float
- String object
- Boolean T/F

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

PEDMAS FIGURE

Python follows the PEDMAS order of operations: parenthesis, exponents, multiplication, division, addition, subtraction. 
- *When in doubt, use parenthesis!*

## Comprehension Check

Sample math problems, what would be correct output for....
- Modulus operator
- Exponent operator
- Integer/floor division
- Example that involves order of operations

Show example of arithmetic operator and assignment statement, what terms/concepts/statements apply to this
- Example of simple vs composite
- Expression/assignment/statement language
- Something about data type

## Application

Explain each / show example
- Addition
- Subtraction
- Multiplication
- Division
- Modulus
- Exponents

QX: Write a program that uses arithmetic operators to convert a specific Farenheit temperature value and output its Celsius representation. Answer to this question includes program + comments that document process and explain your code.

<blockquote>The conversion equation is: <code>celsius = (fahrenheit - 32.0) * 5.0 / 9.0</code></blockquote>

QX: Write a program that calculates the fewest number of U.S. coins needed to make change for a 73 cent remainder. To put that another way- write a program that determines the smallest number of coins in each U.S. denomination needed to make up 73 cents. Answer to this question includes program + comments that document process and explain your code.

In U.S. currency, one dollar ($1.00) equals one hundred (100) cents. The coins used to make change have a face value in cents.

- Quarter = 25 cents
- Dime = 10 cents
- Nickel = 5 cents
- Penny = 1 cent

<blockquote>This workflow mirrors how store clerks give change to their customers. To be considerate, they always try to give the exact change using the fewest coins possible. It turns out that this can always be done (in U.S. currency) by giving as many quarters as possible, followed by as many dimes as possible, and so on down to pennies.</blockquote>

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

In the last section of this lab, we'll talk about how to convert data types to address this issue.

## Comprehension Check

Describe concatenation in your own words

Difference between addition and concatenation
- Show example with different data types, what would be the output

## Application

QX: Variables for each of the pieces of a standard ND intro (name, year, majors/minors, hall), use concatenation to create the full introduction using any of the syntax options above

QX: Write a program that creates `first_name` and `last_name` variables, and then uses concatenation to output a `full_name` variable. Answer to this question includes program + comments that document process and explain your code.

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

NOTE: The default data type for a variable created using the `input()` function is a string object. We can change data types using the functions we'll cover in the last section of this lab.

More on Python's `input()` function:
- [W3Schools, Python input() Function](https://www.w3schools.com/python/ref_func_input.asp)

## Comprehension Check

What does I/O stand for

What are some examples in a programming context

Programs that use input- what would we expect to have happen
- Addition and a string object (concatenation)
- Division and a string object (error)

## Application

QX: Write a program that asks the user to enter their favorite color, and then prints a `"You favorite color is..."` message. Answer to this question includes program + comments that document process and explain your code.

QX: Standard ND intro with user inputs.

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

Programs that change data type- what would we expect to have happen
- Convert string input to number, arithmetic operation
- Try to convert string input (that's not a number) to a number, error message
- Concatenation with string number input and convert to number, concatenation

## Application

QX: Write a program that prompts the user to enter two numbers, converts the input values to integers, adds them, and reports the result. Answer to this question includes program + comments that document process and explain your code.

QX:  Write a program that asks the user to think of a month and then enter the number of days in that month. Your program should then compute the number of minutes in the month, and report the result. Answer to this question includes program + comments that document process and explain your code.

QX: Write a program that prompts the user to enter a temperature in Fahrenheit, and reports the equivalent temperature in Celsius. Answer to this question includes program + comments that document process and explain your code.

# How to submit this lab (and show your work)

Moving forward, lab notebooks will be submitted as `.py` files. 

One option is to have a `.py` file that you use to run code and test programs while working through the lab. When ready to submit the lab notebook, you add comments and remove extraneous materials.

Another option is to have an "official" `.py` file that you are using as a lab notebook (separate from your working/testing file). Use comments in Python to note when you are starting a new question (as well as answering a question).
- Example: `Lab5_Notebook_Walden.py`

What gets submitted as the lab notebook is the `Lab5_Notebook_Walden.py` file.
- When in doubt, use comments
- Be sure you are using comments to note what question you're responding to

## Final Application Questions

### ASCII Art

"ASCII art is a graphic design technique that uses computers for presentation and consists of pictures pieced together from the 95 printable (from a total of 128) characters defined by the ASCII Standard" ([Wikipedia, "ASCII art"](https://en.wikipedia.org/wiki/ASCII_art))

An example of ASCII art output:

```
           * *
          *   *
           * *
            *
          * * *
         *  *  *
        *   *   *
            *
          *   *
         *     *
        *       *
       *         *
      *           *
```

One option to create this output in Python is to use multiple print statements:

```Python
print("     * *")
print("    *   *")
print("     * *")
print("      *")
print("    * * *")
print("   *  *  *")
print("  *   *   *")
print("      *")
print("    *   *")
print("   *     *")
print("  *       *")
print(" *         *")
print("*           *")
```

Another option would be to use regular expression special characters to note when we want to mark line breaks and tabs.

What are regular expressions? Generally, regular expressions (or regex) are special characters or character sequences that form a search pattern.
- More on regular expressions in Python: [W3Schools, Python Regex](https://www.w3schools.com/python/python_regex.asp)

A couple special characters that might be useful for ASCII art:
- `\n` (new line)
- `\r` (carriage return)
- `\t` (tab)

How we might create the same stick figure ASCII art using regular expressions:

```Python


QX: Write a program that creates your own ASCII art. You're welcome to consult the [ASCII Art Archive](https://www.asciiart.eu/) for inspiration. Answer to this question includes program + comments that document process and explain your code.

### Calculating Change

QX: Write a program that asks the user to input the amount of change your program is to make, and then compute the number of quarters, dimes, nickels, and pennies that produces the correct change with the fewest coins possible. Answer to this question includes program + comments that document process and explain your code.

In U.S. currency, one dollar ($1.00) equals one hundred (100) cents. The coins used to make change have a face value in cents.

- Quarter = 25 cents
- Dime = 10 cents
- Nickel = 5 cents
- Penny = 1 cent


# Lab Notebook Questions

TEMPLATE LINK

ALL THE QUESTIONS
