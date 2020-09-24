# Lab #5: Getting Started With Python (basic syntax & data types)

<a href="http://creativecommons.org/licenses/by-nc/4.0/" rel="license"><img style="border-width: 0;" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" alt="Creative Commons License" /></a>
This tutorial is licensed under a <a href="http://creativecommons.org/licenses/by-nc/4.0/" rel="license">Creative Commons Attribution-NonCommercial 4.0 International License</a>.

## Lab Objectives

By the end of this lab you will be able to:
-	Describe the differences between a high-level programming language and machine language
-	Use Repl.it (or another IDE) to write and execute Python programs
-	Understand and be able to use core elements of Python syntax (including the `print` command, character strings, and variables)

Python is an object-oriented programming language. It’s comparable to a number of other programming languages, such as Perl, Ruby, or Java. Python is a high-level programming language.

## Acknowledgements

This lab is based on the ["Lab: Programming in Python"](https://www.cs.grinnell.edu/~davisjan/csc/105/2012S/labs/python1.html) and ["Lab: Numbers in Python"](https://www.cs.grinnell.edu/~davisjan/csc/105/2012S/labs/python2.html) lab materials developed by [Janet Davis](https://cs.whitman.edu/~davisj/) for the the [CSC 105 "The Digital Age" course](https://www.cs.grinnell.edu/~davisjan/csc/105/2012S/). 

### Programming in Python

- Written: Marge M. Coahran, February 2008
- Revised: Jerod Weinman, 2 January 2009
- Revised: Jerod Weinman, 24 February 2011
- Revised: Janet Davis, 6 March 2012
- Adopted from: [CSC105: Programming in Python](http://www.cs.grinnell.edu/%7Ecoahranm/csc105/labs/python1.html)
- Copyright © 2009-2012 Marge Coahran, Jerod Weinman, and Janet Davis.
- This work is licensed under a [Creative Commons Attribution-Noncommercial-Share Alike 3.0 United States License](http://creativecommons.org/licenses/by-nc-sa/3.0/us/).

### Numbers in Python
- Written: Marge M. Coahran, February 2008
- Revised: Jerod Weinman, 2 January 2009
- Revised: Jerod Weinman, 25 February 2011
- Revised: Janet Davis, 9 March 2012
- Adopted from: [CSC105: Programming in Python (Numbers)](http://www.cs.grinnell.edu/%7Ecoahranm/csc105/labs/python2.html)
- Copyright © 2009-2012 Marge Coahran, Jerod Weinman, and Janet Davis.
- This work is licensed under a [Creative Commons Attribution-Noncommercial-Share Alike 3.0 United States License](http://creativecommons.org/licenses/by-nc-sa/3.0/us/).

This lab also incorporates elements of [Corey Pennycuff's](https://www3.nd.edu/~cpennycu/) ["Intro to Python/Jupyter" Jupyter notebook](https://www3.nd.edu/~cpennycu/2019/assets/fall/EOC/19.08.29.ipynb) from [CSE 10101 Elements of Computing (Fall 2019)](https://www3.nd.edu/~cpennycu/2019/fa-CSE10101-CDT30010.html).

# Table of Contents
- [How to submit this lab (and show your work)](#how-to-submit-this-lab-and-show-your-work)
- [Your First Program](#your-first-program)
- [Print Statements & ASCII Art](#print-statements--ascii-art)
- [Data Types](#data-types)
  * [Comments](#comments)
  * [Variables and Types](#variables-and-types)
  * [Numbers](#numbers)
  * [Strings](#strings)
  * [Boolean Operators](#boolean-operators)
  * [Arithmetic Operators](#arithmetic-operators)
- [Character Strings and Variables](#character-strings-and-variables)
  * [User-defined inputs](#user-defined-inputs)
  * [Additional exercises](#additional-exercises)
- [Lab Notebook Questions](#lab-notebook-questions)

# How to submit this lab (and show your work)

Moving forward, we'll submit lab notebooks as `.py` files. 

One option is to have a `.py` file that you use to run code and test programs while working through the lab. When ready to submit the lab notebook, you add comments and remove extraneous materials.

Another option is to have an "official" `.py` file that you are using as a lab notebook (separate from your working/testing file). Use comments in Python to note when you are starting a new question (as well as answering a question).
  * Example: `Lab5_Notebook_Walden.py`

What gets submitted as the lab notebook is the `Lab5_Notebook_Walden.py` file.
- When in doubt, use comments
- Be sure you are using comments to note what question you're responding to

# Your First Program

1. Your first program will contain a single Python statement. Enter the following statement into a new `.py` file. 

<blockquote>Watch out for quotation marks!</blockquote>

```python
print ("Welcome to the wild world of computer programming!")
```
2. Save your work as part of the `main.py`. 

<blockquote>When adding new files in Repl.it or writing a Python program from scratch either in a text editor or in a desktop Python IDE, be sure to include the <code>.py</code> file extension, which specifies your file is a Python program.</blockquote>

3. As in the Lab #4 and Midterm Project work in HTML/CSS, one of the features of an IDE is that syntax highlighting, which recognizes the language you are writing in and uses color/font highlighting to visually help you write and understand programs.

4. Run your first program in the Replit terminal window, using the following command: `python main.py`. You can also run the program using "Run"

5. The `print()` function will output the value passed to it, including a string. 

<blockquote>NOTE: If you've previously worked in Python 2, the way Python 3 deals with strings is very different. Consult <a href="https://docs.python.org/3.7/library/string.html#format-string-syntax">Python documentation</a> if needed.</blockquote>

<blockquote>Q1: What do you expect to see when you run the <code>first.py</code> program? How does that compare to what happened when you ran the program?</blockquote>

# Print Statements & ASCII Art

5. Add a second print statement to your `main.py` program:
```python
print "Are we having fun yet?"
```
6. Save your program, and run it in the terminal window.

7. Modify your program to include additional lines of text in your output. Note that you can use any punctuation or printable symbol on the keyboard.

8. Start a new file in your repl (remember the `.py` file extension!) to start writing a new program `figure.py`.

9. In your new file, write a program that draws a figure similar to the one below, using a set of `print` commands.
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
<blockquote>This kind of drawing is called "ASCII Art" since it is made solely with characters in the ASCII character set.</blockquote>

10. Run the `figure.py` program in the terminal.

11. Create a new file (`ascii.py`) and write a program in which you draw your own ASCII art using Python `print` statements. 

<blockquote>Consult the <a href="https://www.asciiart.eu/">ASCII Art Archive</a> for inspiration.</blockquote>

<blockquote>Q2: Describe your experience and process building your own ASCII art. How did you approach the design process? What challenges did you encounter? Include your code as part of this answer.</blockquote>

# Data Types 

11. Python includes a number of different data types, which can be stored as variables.

12. We'll do more with variables later, but for now...

## Comments

```python
# From Professor Walden: The text of this comment about comments is taken from one of Corey Penneycuff's Elements of Computing I Jupyter notebooks

# I am a comment

"""
I am a multi-line comment.
I'm not really a "comment" per-se, but Python does not support
multi-line comments, so I'm the best that you get.
If I'm not really a comment, then what am I?  Well, I'm actually
a multi-line string that Python evaluates, and then ignores,
because nothing is being done with the string.
"""

# The only alternative is to put a pound at the beginning of each line.
# This is a pound sign --> #
# No, it's not a "hashtag".
# It was called "pound" LONG before "hashtag" was even though about...
# by about a century!
```

## Variables and Types

13. What are variables in Python?
- Variables are a "storage location" for holding some value which can be used by a Python script
- A variable's contents are referred to as its "data"
- All data has some "type" associated with it
- We're focusing on a few key data types, but there are <bold>many</bold> different types of data in Python.
  * Consult the [Python.org documentation on data types](https://docs.python.org/3/library/datatypes.html) to learn more.
  
14. For each of these examples, copy/paste or retype the code into a new `.py` file to run each mini program (and learn more about Python's functionality and documentation). Experiment, adapt, or modify these samples as you work through the lab procedure.

## Numbers

15. An integer is a whole number that does not include any decimal (or fractional) values. A float data type includes decimal (or fractional) values.
```python
# Numbers: Int and Float
i = 3
print("i is of type: ", type(i))
j = 3.0
print("j is of type: ", type(j))
```
<blockquote>It may seem odd at first, but in Python, the "equals sign" here does not denote equality. Rather, it is an instruction telling Python to assign the value on its right into the variable on its left.</blockquote>

16. But Python variables can also change their type...
```python
# variable type...can vary
i = 3
print("i is of type: ", type(i))
i = i + .5
print("i is of type: ", type(i))
```

## Strings

17. A string is a sequence of characters (letters, numbers, symbols, etc.)
```python
s = "Hello world!"
print(s)
```

18. Another example of strings at work, this time using concatenation to join strings.
```python
myFirstName = "Katherine"
myLastName = "Walden"
myName = myFirstName + " " + myLastName
print(myName)
```
<blockquote>Concatenation: adding or joining together. For strings, Python will concatenate using the <code>+</code> symbol.</blockquote>

## Boolean Operators

19. Boolean operators are logical values (think true/false, yes/no, 0/1).

20. We can use Boolean operators in a variety of ways when programming in Python.

21. `<`, `<=`, `>`, `>=`, `==`, `!=` compare two values and return `True` or `False`.

22. `and`, `or`, and `not` can combine or modify `True` and `False` values.

23. A few examples. Remember for each of these examples, copy/paste or retype the code into a new `.py` file to run each mini program (and learn more about Python's functionality and documentation)

```python
print(type(x == 4))
print(x==4)
```

```python
# Logic operators can be chained.
print(1 < 2 < 3)
print(10 < 2 < 3)
```

```python
x = 3
y = 18
z = 10
print (x < y < z)
```

```python
# a complex sample program that uses Boolean operators
print("\"True\" is of type: ", type(True))
myLogicalVariable = True

print(myLogicalVariable)
print('with a not:', not myLogicalVariable)
print('with a not not:', not not myLogicalVariable)
print('True and True:', True and True)
print('True and False:', True and False)
print('True or True:', True or True)
print('True or False:', True or False)
print("3: ", bool(3))
print("0: ", bool(0))
print("-1:", bool(-1))
```

<blockquote>Q3: Describe a scenario or situation in which being able to use Boolean operators when programming in Python would be valuable. What kinds of tasks or programs would require Boolean operators? What would Boolean operators enable you to do?</blockquote>  
  
## Arithmetic Operators

24. A few standard operators we can use in Python to perform arithmetic operations.
- `+` (plus, sum)
- `-` (minus, subtraction)
- `*` (times, multiplication)
- `//` (divide, integer division)
- `/` (divide, float division)
- `%` (modulo operator, used to return/retrieve remainder after division)
- `**` (exponent)

25. Python follows the PEDMAS order of operations. When in doubt, use parenthesis!

<blockquote>PEDMAS order of operations: parenthesis, exponents, multiplication, division, addition, subtraction</blockquote>

```python
# sample program that uses float and integer division, as well as the modulo operator
print ("3 / 2 = %f" % (3 / 2))
print ("3 // 2 = %f" % (3 // 2))
```

```python
# sample program that uses order of operations, addition and subtraction, plus the modulo operator
print ("3 + 2 = %d" % (3 + 2))
print ("7 - 13 = %d" % (7 - 13))
```

```python
# sample program that uses order of operations, multiplication, and the modulo operator
# notice the difference between %d and %f
print ("8 * .4 = %d" % (8 * .4))
print ("8 * .4 = %f" % (8 * .4))
```

```python
# sample program that uses integer division, order of operations, and the modulo operator
print ("8 // 3 = %d" % (8 // 3))
# % is the "modulus" (e.g., the "remainder")
print ("278 %% 13 = %d" % (278 % 13))
```

```python
# sample program that includes exponentiation, as well as multiplication and order of operations
print("4 ** 3.8 = %f" % (4 ** 3.8))
```

```python
# sample program that uses the print command to show a variety of number output formats
# this program requires we import the math library
import math
print ("This number (%f) is pi." % math.pi)
print ("This number (%.3f) is pi." % math.pi)
print ("This number (%10.3f) is pi." % math.pi)
print ("This number (%010.3f) is pi." % math.pi)
print ("This number (%+010.3f) is pi." % math.pi)
print ("%+010.3f" % -math.pi)
print ("%e" % 8675309)
```

<blockquote>Q4: Experiment with a range of basic arithmetic operations in Python. Write a program that involves arithmetic operation. Describe the process of writing this program. What did you want to do in Python? What were the program outputs? What challenges or unexpected results did you encounter? Include your program as part of the answer to this question.</blockquote>

# Character Strings and Variables

## User-defined inputs

26. Earlier in this lab, we used the `+` sign to concatenate two strings. 

27. Now we're going to write a program that allows the user (i.e. the person running the program) to input a value for the program to use.

28. To allow the user to input a value, we'll use the `raw_input` function.
```python
# sample code that uses the raw_input function to create a new str variable and assign the user-provided value to that variable
str = raw_input("Please enter a word: ")
print "You typed " + str
```
<blockquote>Q5: Write a program that asks the user to enter two words, and then prints the words concatenated together. Answer to this question includes program + comments that document process and explain your code.</blockquote>

29. Now try entering numbers (such as 5, not "five") into your Q5 program. 

30. This result is less than useful. But how can Python know when we ask for user input whether we want the program to treat numbers as numbers or as strings?

31. The issue here is that Python (like other programming languages) makes a distinction between numbers and strings of characters that contain numeric digits. To see the difference, think of your zip code. It makes no sense to add or multiply zip codes; thus, at heart a zip code isn't really a number, it is really a character string that happens to contain numeric digits. Indeed, many countries use postal codes that include both digits and letters. 

32. The `raw_input` function will always return a character string.

33. We want to convert that string into an integer using the `int()` function.
```python
data = raw_input("Enter a number: ")
num = int(data)
```

34. At this point, `data` contains a string of digits, but `num` contains a number (specifically an integer).

35. Try modifying your Q5 program to include the `int()` function. 

<blockquote>Q6: Write a new program called <code>addition.py</code> that prompts the user to enter two numbers, converts the input values to integers, adds them, and reports the result. Answer to this question includes program + comments that document process and explain your code. </blockquote>

36. An alternative way to handle this situation would be to use a different function to read input from the user. While `raw_input()` always returns a string of characters, the `input()` function always returns a number.

37. The user inputs from the `input()` function can be added to other numbers (and do not need to be converted to an integer first).
```python
number = input("Please enter a number: ")
```

## Additional exercises

Q7:  Write a program that asks the user to think of a month and then enter the number of days in that month. Your program should then compute the number of minutes in the month, and report the result. Answer to this question includes program + comments that document process and explain your code.
  
Q8: Write a program that prompts the user to enter a temperature in Fahrenheit, and reports the equivalent temperature in Celsius. Answer to this question includes program + comments that document process and explain your code.

<blockquote>The conversion equation is: <code>celsius = (fahrenheit - 32.0) * 5.0 / 9.0</code></blockquote>

Q9: Write a program called `change.py` that asks the user to input the amount of change your program is to make, and then compute the number of quarters, dimes, nickels, and pennies that produces the correct change with the fewest coins possible. Answer to this question includes program + comments that document process and explain your code.

<blockquote>Note: Consider how store clerks give change to their customers. To be considerate, they always try to give the exact change using the fewest coins possible. It turns out that this can always be done (in U.S. currency) by giving as many quarters as possible, followed by as many dimes as possible, and so on down to pennies.</blockquote>

# How to submit this lab (and show your work)

38. Moving forward, lab notebooks will be submitted as `.py` files. 

39. One option is to have a `.py` file that you use to run code and test programs while working through the lab. When ready to submit the lab notebook, you add comments and remove extraneous materials.

40. Another option is to have an "official" `.py` file that you are using as a lab notebook (separate from your working/testing file). Use comments in Python to note when you are starting a new question (as well as answering a question).
  * Example: `Lab5_Notebook_Walden.py`

41. What gets submitted as the lab notebook is the `Lab5_Notebook_Walden.py` file.
- When in doubt, use comments
- Be sure you are using comments to note what question you're responding to

# Lab Notebook Questions

Q1: What do you expect to see when you run the <code>first.py</code> program? How does that compare to what happened when you ran the program?

Q2: Describe your experience and process building your own ASCII art. How did you approach the design process? What challenges did you encounter? Include your code as part of this answer.

Q3: Describe a scenario or situation in which being able to use Boolean operators when programming in Python would be valuable. What kinds of tasks or programs would require Boolean operators? What would Boolean operators enable you to do?

Q4: Experiment with a range of basic arithmetic operations in Python. Write a program that involves arithmetic operation. Describe the process of writing this program. What did you want to do in Python? What were the program outputs? What challenges or unexpected results did you encounter? Include your program as part of the answer to this question.

Q5: Write a program that asks the user to enter two words, and then prints the words concatenated together. Include your program as part of the answer to this question.

Q6: Write a new program called <code>addition.py</code> that prompts the user to enter two numbers, converts the input values to integers, adds them, and reports the result. Answer to this question includes program + comments that document process and explain your code.

Q7:  Write a program that asks the user to think of a month and then enter the number of days in that month. Your program should then compute the number of minutes in the month, and report the result. Answer to this question includes program + comments that document process and explain your code.
  
Q8: Write a program that prompts the user to enter a temperature in Fahrenheit, and reports the equivalent temperature in Celsius. Answer to this question includes program + comments that document process and explain your code.

Q9: Write a program called `change.py` that asks the user to input the amount of change your program is to make, and then compute the number of quarters, dimes, nickels, and pennies that produces the correct change with the fewest coins possible. Answer to this question includes program + comments that document process and explain your code.
