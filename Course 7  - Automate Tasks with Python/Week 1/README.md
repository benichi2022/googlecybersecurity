# Week 1
# Introduction to Python
# Introduction to python programming in cybersecurity

Lines of code are used to communicate with a computer, similar to a sentence, telling it how to perform a task. Programming is used to create a specific set of instructions for a computer to execute tasks. Python is considered to be a general-purpose language. This means that it can create a variety of different programs, and it isn't a specialized in any particular problem in fields such as web development and artificial intelligence. Python is typically used to build websites and perform data analysis. In security, the main reason we use Python is to automate our tasks. Automation is the use of technology to reduce human and manual effort to perform common and repetitive tasks.
In addition to automating individual tasks, Python can combine separate tasks into one workstream. So why exactly might a security professional choose Python for these tasks? There are several advantages Python has as a programming language. For one, Python is user-friendly because it resembles human language, it requires less code, and it's easy to read. Python programmers also have the benefit of following standard guidelines to ensure consistency with the design and readability of code. Another great reason for learning Python is that there's a large amount of online support. Python also has an extensive collection of built-in code that we can import and use to perform many different tasks.

 When we work in Python, we refer to what we write as a "script" or a "program." In Python, it's good practice to start with a comment. A comment is a note programmers make about the intention behind their code.

Simple python script used for printing message:

![image](https://github.com/benichi2022/googlecybersecurityprofessionalcertificate/assets/113864743/79c42b19-fe18-414d-9c79-f4f6f62c3702)

we want to output the string "Hello Python!" We must place string data in quotation marks. These quotation marks are just one example of syntax that you will encounter in Python. Syntax refers to the rules that determine what is correctly structured in a computing language. 

# Core Python Components
Data types in python
A data type is a category for a particular type of data item. String data is data consisting of an ordered sequence of characters. These characters could be letters, symbols, spaces, and even numbers.
Strings must be placed within qoutes. Otherwise, python will return an error.

![image](https://github.com/benichi2022/googlecybersecurityprofessionalcertificate/assets/113864743/63a63cbd-4948-4028-8612-51707e28a0bc)

Python also supports numeric data types as well. When working with numeric data, we don't put quotation marks around the data. Numeric data includes floats and integers. Float data is data consisting of a number with a decimal point. This includes fractions like 2.1 or 10.5. It also includes whole numbers with a decimal point like 2.0 or 10.0.
Integer data is data consisting of a number that does not include a decimal point. Numbers such as 0, -9, and 5,000 are valid integers. The third data type in Python is called a Boolean. Boolean data is data that can only be one of two values: either "True" or "False." Booleans are useful for logic in our programs. For example, let's compare numbers and determine the Boolean values of these comparisons. 

![image](https://github.com/benichi2022/googlecybersecurityprofessionalcertificate/assets/113864743/0c0aebff-d54d-4420-adb9-24a041893855)

List data is a data structure that consists of a collection of data in sequential form. We'll create and print a list that prints all the usernames of the three individuals that have access to a confidential file. 

![image](https://github.com/benichi2022/googlecybersecurityprofessionalcertificate/assets/113864743/aa3f82f9-b7eb-4158-a1a5-8bcc5cba43ab)

A variable is a container that stores data. To create a variable, you need a name for it. Then, you add an equals sign and then an object to store in it. Creating a variable is often called assignment. The best practice for naming variables is to make the names relevant to what they're being used for. 

String Data Type:

![image](https://github.com/benichi2022/googlecybersecurityprofessionalcertificate/assets/113864743/d480bffe-65d2-428a-b406-e927e50cb2fe)

"Calling" the variable 

![image](https://github.com/benichi2022/googlecybersecurityprofessionalcertificate/assets/113864743/c0dce2cc-7451-45f4-b1e1-aec6bcd5a7b6)

Data type of a variable is the same as the data type of the data it stores.

![image](https://github.com/benichi2022/googlecybersecurityprofessionalcertificate/assets/113864743/d500c493-1236-4aa0-97a0-b41a9aa88332)

and type function to check the data type.

After we define a variable, we can always change the object inside of it. This is called reassignment. Reassigning a variable is very similar to assigning it in the first place. Let's try this out and reassign a variable. 

# Conditional statements in Python
Automation is the use of technology to reduce human and manual effort to perform common and repetitive tasks. Conditional statements are important for automation. A conditional statement is a statement that evaluates code to determine if it meets a specified set of conditions. The keyword if is important in conditional statements. if starts a conditional statement. After this keyword, we then specify the condition that must be met and what will happen if it is.
Python always evaluates if the condition is True or False, and if it's True, it performs the specific action.
Example, checking the number of failed attempts.

![image](https://github.com/benichi2022/googlecybersecurityprofessionalcertificate/assets/113864743/b328ecd2-16f9-4ddd-8333-000f3adb7592)

In this case, when the user has more than five failed log-in attempts, it prints a message that the account is locked. In Python, this message should always be indented at least one space in order to execute only when the condition is true.

We can also use conditional operators.

![image](https://github.com/benichi2022/googlecybersecurityprofessionalcertificate/assets/113864743/0efc5026-a265-4e22-a841-0e0091fe289d)

# For Loops
An iterative statement is code that repeatedly executes a set of instructions. Iterative statements are also referred to as "loops." There are two types of loops we'll explore: for loops and while loops. The loop header is the line that contains the for keyword and ends with a colon. It tells Python to start a loop. It consists of the for keyword, a loop variable, and the sequence the loop will iterate through. The loop variable is a variable that is used to control the iterations of a loop. The loop variable comes directly after for.

![image](https://github.com/benichi2022/googlecybersecurityprofessionalcertificate/assets/113864743/45e91efb-4fd4-4435-8c94-d4be34013989)

Another important use of for loops is to repeat a specific process a set number of times. This is done through combining it with the range function. 

![image](https://github.com/benichi2022/googlecybersecurityprofessionalcertificate/assets/113864743/dddc934f-d5f3-44d8-8547-ac26194af33e)

# While Loops

While loops still repeatedly execute, but this repetition is based on a condition. As long as the condition is true, the loop continues to execute. But when it becomes false, the while loop stops. It consists of the keyword while, the condition, and a colon. The while loop starts with the keyword while. The keyword while signals the beginning of a while loop and is followed by the condition that evaluates to a Boolean value of either True or False. The condition contains the loop variable. This variable is used to control the number of loop iterations.

![image](https://github.com/benichi2022/googlecybersecurityprofessionalcertificate/assets/113864743/5d993a9d-1e85-44df-ae52-831ff40fecb6)

Since while loops do not include a sequence to iterate through, we have to explicitly define how the loop variable changes in the body of the while loop. For example, in this while loop, we increase the loop variable time by two every iteration.

![image](https://github.com/benichi2022/googlecybersecurityprofessionalcertificate/assets/113864743/c7f7dc1b-be5e-40c7-b10d-fef9bc074744)

Glossary terms from week 1
Terms and definitions from Course 7, Week 1
Automation: The use of technology to reduce human and manual effort to perform common and repetitive tasks

Boolean data: Data that can only be one of two values: either True or False

Command-line interface: A text-based user interface that uses commands to interact with the computer

Comment: A note programmers make about the intention behind their code

Conditional statement: A statement that evaluates code to determine if it meets a specified set of conditions

Data type: A category for a particular type of data item

Dictionary data: Data that consists of one or more key-value pairs

Float data: Data consisting of a number with a decimal point

Integer data: Data consisting of a number that does not include a decimal point

Integrated development environment (IDE): A software application for writing code that provides editing assistance and error correction tools

Interpreter: A computer program that translates Python code into runnable instructions line by line 

Iterative statement: Code that repeatedly executes a set of instructions

List data: Data structure that consists of a collection of data in sequential form

Loop variable: A variable that is used to control the iterations of a loop

Notebook: An online interface for writing, storing, and running code 

Programming: A process that can be used to create a specific set of instructions for a computer to execute tasks

Set data: Data that consists of an unordered collection of unique values

String data: Data consisting of an ordered sequence of characters

Syntax: The rules that determine what is correctly structured in a computing language

Tuple data: Data that consists of a collection of data that cannot be changed 

Type error: An error that results from using the wrong data type

Variable: A container that stores data






































