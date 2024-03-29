# Key Concepts

Specific code commands that show up in this lab:

<table><tr><th>Name</th><th>Syntax</th><th>Example></th><th>Description</th></tr>
  <tr><td>Type function</td><td><code>type()</code></td><td><code>type("Hello world!")</code></td><td>Returns data type</td></tr>
  <tr><td>Print function</td><td><code>print()</code></td><td><code>print("Hello world!")</code></td><td>Shows specific output in console or shell</td></tr>
  <tr><td>Concatenation</td><td><code>+</code></td><td><code>print("Hello" + " " + "World!")</code></td><td>Adds strings together</td></tr>
  <tr><td>Assignment operator</td><td><code>=</code></td><td><code>x = 3</code></td><td>Assigns value(s) to variable</td></tr>
  </table>

Comparison operators:

<table><tr><th>Name</th><th>Syntax</th><th>Example</th><th>Description</th></tr>
  <tr><td>Equal</td><td><code>==</code><td><code>x == y</code></td><td>Tests if values are equal</td></tr>
  <tr><td>Not equal</td><td><code>!=</code><td><code>x != y</code></td><td>Tests if values are not equal</td></tr>
  <tr><td>Greater than</td><td><code>></code><td><code>x > y</code></td><td>Tests is a value is greater than another</td></tr>
  <tr><td>Less than</td><td><code><</code><td><code>x < y</code></td><td>Tests is a value is less than another</td></tr> 
  <tr><td>Greater than or equal to</td><td><code>>=</code><td><code>x >= y</code></td><td>Tests if a value is greater than or equal to another</td></tr>
  <tr><td>Less than or equal to</td><td><code><=</code><td><code>x <= y</code></td><td>Tests if a value is less than or equal to another</td></tr>  
  </table>

**Arithmetic operators**
- Used with numeric values for mathmetical operations
  * More info: [W3Schools](https://www.w3schools.com/python/gloss_python_arithmetic_operators.asp)

<table><tr><th>Name</th><th>Syntax</th><th>Example</th><th>Description</th></tr>
  <tr><td>Addition</td><td><code>+</code><td><code>5 + 6</code></td><td>Adds values</td></tr>
  <tr><td>Subtraction</td><td><code>-</code><td><code>5 - 6</code></td><td>Subtracts values</td></tr>
  <tr><td>Multiplication</td><td><code>*</code><td><code>5 * 6</code></td><td>Multiples values</td></tr>
  <tr><td>Integer division</td><td><code>//</code><td><code>5 // 6</code></td><td>Divides values, integers (whole numbers)</td></tr> 
  <tr><td>Float division</td><td><code>/</code><td><code>5 / 6</code></td><td>Divides values, floating point numbers (decimal values)</td></tr>
  <tr><td>Modulo</td><td><code>%</code><td><code>5 % 6</code></td><td>Returns or retrieves remainder (whole number) from division operation</td></tr>  
  <tr><td>Exponent</td><td><code>**</code><td><code>5 ** 6</code></td><td>Calculates exponent</td></tr>
  </table>

**ASCII Art**
- "ASCII art is a graphic design technique that uses computers for presentation and consists of pictures pieced together from the 95 printable (from a total of 128) characters defined by the ASCII Standard from 1963" ([Wikipedia](https://en.wikipedia.org/wiki/ASCII_art))
- [ASCII Art Archive](https://www.asciiart.eu/)

**Assignment, Assignment Operator**
- "An assignment statement sets and/or re-sets the value stored in the storage location(s) denoted by a variable name; in other words, it copies a value into the variable...The assignment operator has two operands. The one to the left of the operator is usually an identifier name for a variable. The one to the right of the operator is a value" (Kenneth Leroy Busbee and Dave Braunschweig, "[Assignment](https://press.rebus.community/programmingfundamentals/chapter/assignment/)" in *Programming Fundamentals*)
- We create a variable by assigning a value to that variable name using an assignment operator. In Python, the equals sign `=` is the assignment symbol. The underlying syntax for creating a variable in Python using an assignment statement:

```
[identifier] [assignment symbol] [value]
```

**Boolean Logic**
- "In mathematics and mathematical logic, Boolean algebra is the branch of algebra in which the values of the variables are the truth values true and false, usually denoted 1 and 0" ([Wikipedia](https://en.wikipedia.org/wiki/Boolean_algebra))
- "You can evaluate any expression in Python, and get one of two answers, `True` or `False`. When you compare two values, the expression is evaluated and Python returns the Boolean answer" ([W3Schools, Python Booleans](https://www.w3schools.com/python/python_booleans.asp))

Python example:

```Python
print(4 == 5) # returns false
print(6 < 10) # returns true

# boolean logic with variables
x = 5
y = 6
print(x > y) # returns false
```

**Comments** (in a programming language)
- Comments mark instructions or information in the code that will not run as part of the program. Comments are useful for testing, documenting, and describing what your code is doing. 
-In Python, single line comments begin with a pound `#` symbol and multi-line comments are marked by three sets of double quotation marks `"""`.

```Python
# This is an example of a single line comment in Python

"""
This is an example of a multi-line comment in Python
"""
```

For more on comments in Python:
- [W3Schools, Python Comments](https://www.w3schools.com/python/python_comments.asp)

**Comparison Operators (or relational operators)**

- "The relational operators are often used to create a test expression that controls program flow. This type of expression is also known as a Boolean expression because they create a Boolean answer or value when evaluated. There are six common relational operators that give a Boolean value by comparing (showing the relationship) between two operands. If the operands are of different data types, implicit promotion occurs to convert the operands to the same data type" (Busbee, "[Relational Operators](https://press.rebus.community/programmingfundamentals/chapter/relational-operators/)")

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

**Complex Conditional Statements**
- Conditional statements that compare more than two values or evaluate multiple comparisons as part of a conditional statement.

Python examples:

```Python
# an example that compares three integers
print(5 < 6 > 7) # returns false because 6 is not greater than 7

# an example that compares three strings
print("apple" > "banana" < "blueberry") # returns false because apple comes before or is less than banana
```

We can also compare or relate multiple conditions using logical operators: `and`, `or`, `not`

```Python
# example using logical operators
print(5 < 6 and 6 < 7) # returns true because both statements are true

print(5 < 6 or 6 > 7) # returns true because at least one statement is true

print(not(5 < 6 and 6 < 7)) # returns false, inverse of initial true
```

**Concatenation**
- In most programming languages, concatenation involves adding or joining character strings. For example, we could concatenate the strings `Hello` and `world` to create a `Hello world` message.
- In Python, we use the plus sign `+` to concatenate strings.
  * [W3Schools, String Concatenation](https://www.w3schools.com/python/gloss_python_string_concatenation.asp)

**Console**
- Part of most IDEs. We can type commands and run programs in the console, but those instructions are not saved and aren't available outside the current working session. Program output is also sometimes displayed in the console.

**Data types**
- "A data type is a classification of data which tells the compiler or interpreter how the programmer intends to use the data. Most programming languages support various types of data, including integer, real, character or string, and Boolean" (Kenneth Leroy Busbee and Dave Braunschweig, "[Data Types](https://press.rebus.community/programmingfundamentals/chapter/data-types/)" in *Programming Fundamentals*)

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

**Input/Output (I/O)**
- In programming languages and computing more broadly, `I/O` stands for `Input` and `Output`. Programming languages can take a variety of inputs (user-provided values, data, files, etc) and return outputs in a variety of formats (data stored in memory, output that shows up in the console, newly-created or -modified files, etc).
- `I/O` examples in Python include the `input()` and `print()` functions.

**Input function**
- One way Python accepts input is via the `input()` function, which accepts a user input and assigns that to a variable. 
- NOTE: The default data type for a variable created using the `input()` function is a string object. We can change data types using the functions we'll cover in the last section of this lab.
- More info: [W3Schools, Python input() Function](https://www.w3schools.com/python/ref_func_input.asp)

```Python
# initial prompt with input function
name = input("Enter your name: ")

# output
print("Hello, " + name)
```

**Logical Operators**
- "A logical operator is a symbol or word used to connect two or more expressions such that the value of the compound expression produced depends only on that of the original expressions and on the meaning of the operator. Common logical operators include AND, OR, and NOT." (Busbee and Braunschweig, "[Logical Operators](https://press.rebus.community/programmingfundamentals/chapter/logical-operators/)")

Logical operators in Python:
    
<table><tr><th>Name</th><th>Syntax</th><th>Example</th><th>Description</th></tr>
  <tr><td>And</td><td><code>and</code><td><code>x == y and y != z</code></td><td>Returns <code>True</code> if both statements are true</td></tr>
  <tr><td>Or</td><td><code>or</code><td><code>x != y or y == z</code></td><td>Returns <code>True</code> if one of the statements is true</td></tr>
  <tr><td>Not</td><td><code>not</code><td><code>not(x == y and y != z)</code></td><td>Reverses the result, returns <code>False</code> if the result is true</td></tr>
  </table>
    
For more on logical operators in Python: [W3Schools, Python Logical Operators](https://www.w3schools.com/python/gloss_python_logical_operators.asp)    

**Order of operations** (PEDMAS)
- Python follows the PEDMAS order of operations: parenthesis, exponents, multiplication, division, addition, subtraction. 
  * *When in doubt, use parenthesis!*

**Print function**
- One way that Python shows output is via the `print()` function.
- More info: [W3Schools, Python print() Function](https://www.w3schools.com/python/ref_func_print.asp)

```Python
print("Hello world!")
```

**Regular Expressions**
- Big concept
- Specific examples
- What we're using in this lab (newline character)
- [W3Schools, Python RegEx](https://www.w3schools.com/python/python_regex.asp)

**Reserved Keywords**
- Terms that have other meaning or function in Python can't be used as variable identifiers. For example the name of a built-in function (`type`) can't be used as a variable identifier. 
- Reserved keywords in Python include: `and, except, lambda, with, as, finally, nonlocal, while, assert, fale, None, yield, break, for, not, class, from, or, continue, global, pass, def, if, raise, del, import, return, elif, in, True, else, is, try`

**Script**
- A script authoring window is also part of most IDEs. We can also type commands and run programs in a script. This is a file that is saved as part of the project/workspace. It's available outside the current working session and can be reopened, modified, or executed (as an entire program).

**Shell**
- Sometimes included in an IDE. Command-line environment for running scripts (i.e. `python main.py`).

**Type function**
- `type()`: Used to check an object or value's data type.

```Python
# a type example
type("Hello world!")
```

**Variables**

In most programming languages, variables work as "countainers for storing data values" ([W3Schools, Python Variables](https://www.w3schools.com/python/python_variables.asp)). We create a variable by assigning a value to that variable name using an **assignment operator**.

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
