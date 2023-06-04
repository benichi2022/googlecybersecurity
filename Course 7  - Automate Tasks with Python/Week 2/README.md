# Week 2
# Write Effective Python Code
# Introduction to Functions

Writing this code multiple times would be time-consuming, but luckily we have a way to manage this. We can use functions. A function is a section of code that can be reused in a program.
They perform repetitive activities within a program and allow it to work effectively. Functions are made to be reused in our programs. They consist of small instructions and can be called upon any number of times and from anywhere in our programs.
Another benefit to functions is that if we ever had to make changes to them, we can make those changes directly in the function, and there'll be applied everywhere we use them. 
The print() function is an example of a built-in function. Built-in functions are functions that exist within Python and can be called directly. They are available to us by default. We can also create our own functions. User-defined functions are functions that programmers design for their specific needs.

When we define a function, we basically tell Python that it exists. The def keyword is needed for this. def is placed before a function name to define a function. Let's create a function that greets employees after they log in.

![image](https://github.com/benichi2022/googlecybersecurityprofessionalcertificate/assets/113864743/08fa898a-6865-45b4-b22f-5126aa507d64)

# Work with Functions

![image](https://github.com/benichi2022/googlecybersecurityprofessionalcertificate/assets/113864743/5025e297-4a0b-41f8-9be8-a08d4ace24ac)

In Python, a parameter is an object that is included in a function definition for use in that function. Parameters are accepted into a function through the parentheses after a function name.

range() function generates a sequence of numbers from a start point to the value before the stop point. Therefore,range() does include parameters for the start and stop indices that each accept an integer value. 

![image](https://github.com/benichi2022/googlecybersecurityprofessionalcertificate/assets/113864743/7955baf6-f0a1-413e-8024-de5830488eab)

Return Statement
A return statement is a Python statement that executes inside a function and sends information back to the function call. This ability to send information back from a function is useful to a security analyst in various ways.
We'll name it calculate fails() and we'll set two parameters related to login attempts: one for total_attempts and one for failed_attempts. Next, we'll tell Python what we want this function to do. We want this function to store the percentage of failed attempts in a variable called fail_percentage.

![image](https://github.com/benichi2022/googlecybersecurityprofessionalcertificate/assets/113864743/0f0dba43-aaec-43dc-8ddd-ec7573b7d575)

let's learn how to return the fail percentage. To do this, we need to use the keyword return. Return is used to return information from a function. In our case, we'll return the percentage we just calculated.

![image](https://github.com/benichi2022/googlecybersecurityprofessionalcertificate/assets/113864743/92071217-a6d0-4b56-b0ae-de535fb851d4)

Explore built-in functions
built-in functions are functions that exist within Python and can be called directly. Our only job is to call them by their name! And we've already described a few throughout the course; for example, Python's print() and type() functions.

# Learn From Python Community

Built-in functions come standard with every version of Python and consist of functions such as print(), type(), max(), and many more. To access additional pre-built functions, you can import a library. A library is a collection of modules that provide code users can access in their programs. All libraries are generally made up of several modules. A module is a Python file that contains additional functions, variables, classes, and any kind of runnable code. The Python Standard Library is an extensive collection of usable Python code that often comes packaged with Python.
One example of a module from the Python Standard Library is the re module. This is a useful module for a security analyst when they're tasked with searching for patterns in log files. Another module is the csv module. It allows you to work efficiently with CSV files. The Python Standard Library also contains glob and os modules for interacting with the command line as well as time and datetime for working with timestamps. These are just a few of the modules in the Python Standard Library.

One of the advantages to programming in Python is that it's a very readable language. It also helps that the Python community shares a set of guidelines that promote clean and neat code. These are called style guides. A style guide is a manual that informs the writing, formatting, and design of documents. As it relates to programming, style guides are intended to help programmers follow similar conventions.

The PEP 8 style guide is a resource that provides stylistic guidelines for programmers working in Python. PEP is short for Python Enhancement Proposals. PEP 8 provides programmers with suggestions related to syntax. 
It's essentially based on the principle that code is read much more often than it's written. This is a great resource for anyone who wants to learn how to style and format their Python code in a manner consistent with other programmers. For example, PEP 8 discusses comments. A comment is a note programmers make about the intention behind their code. They are inserted in computer programs to indicate what the code is doing and why.

# Glossary terms from week 2
Terms and definitions from Course 7, Week 2
Argument (Python): The data brought into a function when it is called

Built-in function: A function that exists within Python and can be called directly

Comment: A note programmers make about the intention behind their code

Function: A section of code that can be reused in a program

Global variable: A variable that is available through the entire program

Indentation: Space added at the beginning of a line of code

Library: A collection of modules that provide code users can access in their programs

Local variable: A variable assigned within a function

Module: A Python file that contains additional functions, variables, classes, and any kind of runnable code

Parameter (Python): An object that is included in a function definition for use in that function

PEP 8 style guide: A resource that provides stylistic guidelines for programmers working in Python 

Python Standard Library: An extensive collection of Python code that often comes packaged with Python

Return statement: A Python statement that executes inside a function and sends information back to the function call 

Style guide: A manual that informs the writing, formatting, and design of documents

User-defined function: A function that programmers design for their specific needs
























































