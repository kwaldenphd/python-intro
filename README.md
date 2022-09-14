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
  <tr><td></td>Boolean<td><code>bool()</code><td><code>True</code></td><td>Two-state system that typically represents true/false values</td></tr>
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

## Application

QX: Describe each data type in your own words and show an example (using type)

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

[Click here]() for a list of reserved keywords in Python.

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

Create named variable for each data type in Python using assignment operator

Check using `print` and `type`

Answers need to include assignment statement and print/type for each data type
- Int
- Float
- String object
- Boolean T/F

# Arithmetic Operators

Table of arithmetic operators (define them, show examples)
- Addition
- Subtraction
- Multiplication
- Division
- Modulus
- Exponents
- Floor division

https://www.w3schools.com/python/gloss_python_arithmetic_operators.asp

Try stuff in console (raw output, using Python as a calculator)

Then connect into variables/assignment
- INTRODUCE LANGUAGE OF EXPRESSIONS

ALSO MENTION ORDER OF OPERATIONS (PEDMAS)

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
- Floor division


Check comprehension text on `/` vs `//` with example

TEMPERATURE CONVERSION EQUATION (word problem)

Making change (from set amount)

# Concatenation

Introduce concept:
- Connect to assignment (simple vs composite)
- Reference the underlying logic
- Show the syntax
- Show how it works with different data types

Emphasize underlying logic- arithmetic operation (addition) vs concatenation

Syntax options for concatenation:
- `+` plus sign
- `,` comma
- Curly bracket syntax
- f/s syntax

## Comprehension Check

Difference between addition and concatenation
- Show example with different data types, what would be the output

Different syntax options
- Show example, what would be the output

## Application

QX: Variables for each of the pieces of a standard ND intro (name, year, majors/minors, hall), use concatenation to create the full introduction using any of the syntax options above

QX: Same prompt, but alternate workflow that creates sentences and prints concatenated sentences

# Input & Output (I/O)

Introduce concept:
- Connect with work we've done previously with CPU/memory simulators, and overarching principle of what computers "do" (take an input, do something with it, return that to user)
- Big picture all the different ways we see the concept at work in programming re inputs (user inputs, data, files, etc) and outputs (stored in program memory, show output in console/shell, create/save/modify files, other more complex tasks that can be part of output)

How we're thinking about I/O at this point
- A lot more to come with reading/writing files, but for now...
- `input()` and `print()`
- `print()` we've already seen
- Big picture what `input()` does (takes input, stores in program by assigning to variable)
  * `input()` quirks- STORES AS STRING
  * IF WE WANT TO CHANGE THIS.....introduce concept of converting data types, we'll come back to this

Example of putting it all together:
- Sample program where user inputs favorite color (string) and program outputs "Your favorite color" message

Different ways we can interact with variables and output:
- Concatenation
- Curly bracket syntax
- f/s syntax

## Comprehension Check

What does I/O stand for

What are some examples in a programming context

Programs that use input- what would we expect to have happen
- Addition and a string object (concatenation)
- Division and a string object (error)

## Application

QX: Favorite color message from user input "Your favorite color is")

QX: Standard ND intro with user inputs.

# Converting Data Types

EXAMPLE of trying to perform arithmetic operation on a string object

Describe this as a data type issue

As mentioned previously, default for input is string...We might want to change that

We might also run into data type errors 
- SHOW EXAMPLE OF DATA TYPE ERROR (message or specific example)

So also other scenarios where we need to change how Python is understanding a value/object

We can do that using specific functions:
- `int()`
- `str()`

Show a couple examples of both in action

## Comprehension Check

Programs that change data type- what would we expect to have happen
- Convert string input to number, arithmetic operation
- Try to convert string input (that's not a number) to a number, error message
- Concatenation with string number input and convert to number, concatenation

## Application

QX: Temperature conversion formula using user input

QX: Month/days/something time unit conversion

# Putting It All Together

DOCUMENTING VIA COMMENTS- single vs. multi-line, best practices

How they'll be expected to document in future lab notebooks

## Final Application Questions

FINAL APPLICATION QUESTIONS / PUTTING IT ALL TOGETHER

Pull from existing synthesis notebook questions

ASCII art (mention new line regular expression characters, or multiple print statements)

Calculating change



# Lab Notebook Questions

TEMPLATE LINK

ALL THE QUESTIONS
