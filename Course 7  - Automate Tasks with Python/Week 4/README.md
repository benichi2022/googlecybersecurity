# Week 4
# Python In Practice

# Python For Automation

# Work with files in python

Security professionals often have the responsibility of reviewing log files, which can contain a vast number of entries. Automating this process can be beneficial, and that's where Python comes in handy. To begin, let's import a simple text file containing a few words and convert it into a string using Python.

To accomplish this task, we utilize the "with" statement in Python. The "with" keyword handles errors and manages external resources. By employing the "with" statement, Python automatically releases resources that would otherwise keep our system occupied until the program finishes executing. This is particularly useful in file handling scenarios, ensuring that a file is closed after reading it. To open and read files, we start by using a statement that begins with the "with" keyword, followed by the open() function.

The open() function in Python allows us to open a file. Its first parameter specifies the name of the text file on our computer or provides a link to it on the internet. Depending on the Python environment, we may also need to include the file's path. It's important to include the .txt extension in the file name.

Now let's delve into the second parameter of the open() function. This parameter dictates the intended action on the file. In our case, we aim to read the file, so we utilize the letter "r" enclosed in quotation marks. If we wanted to write to a file, we would replace the "r" with a "w". However, for now, our focus is on reading.

The "file" variable within the with statement holds the file information as long as we remain within the context of the with statement. Similar to other types of statements, we conclude our with statement with a colon. The code following the colon informs Python how to process the file's content.

With our understanding of the concepts, let's put them into practice within Python. We begin by opening a text file using Python.

To accomplish this, we construct our with statement.

Subsequently, we employ Python's built-in read method. This method converts files into strings. Returning to our with statement, similar to a for loop, we begin an indent on the next line to indicate that this code belongs within the with statement. Inside the statement, we utilize the read() function to convert the file into a string and store it in a new variable.

This new variable can be utilized outside the with statement. To exit the with statement, we remove the indentation and proceed to print the variable.

Excellent! The string from the text file is successfully printed.

In summary, security professionals often encounter the task of reviewing log files, which may contain a multitude of entries. Automating this process using Python can be highly advantageous. By employing the "with" statement and the open() function, we can efficiently handle file operations. Furthermore, utilizing the read() method allows us to convert files into strings, providing us with convenient access to their contents.

Now that you have gained the knowledge of importing text files into Python, we can take it a step further and explore how to structure them to facilitate easier analysis. This process is commonly known as parsing, which involves converting data into a more readable format. To achieve this, we will combine our understanding of lists and strings and introduce another method for manipulating strings in Python.

The method we need for parsing is called the split method. By using the split method, we can convert a string into a list. This is accomplished by specifying a character as the delimiter to separate the string. If no argument is provided, the split method automatically splits the string whenever it encounters a whitespace. For instance, the string "We are learning about parsing!" would be converted into the following list.

In our case, we will employ the split method to break down the strings into smaller chunks, allowing for easier analysis compared to dealing with a single large block of text. In the context of this video, we will work with an example of a security log where each line represents a new data point. To store these data points in a list, we will use the split method without passing any arguments since Python treats a new line as a type of whitespace.

Let's begin with the code we used in the previous video, where we opened a file and read its contents into a string. Now, we will utilize the split method to convert that string into a list, and then we will print the output. Upon running the code, Python will generate a list of usernames instead of a single string. If we wish to save this list, we can assign it to another variable, such as "usernames". After assigning the list, we can use it in other parts of our code.

In summary, having the ability to import text files into Python is useful, but structuring them through parsing enhances their readability and ease of analysis. By utilizing the split method, we can convert strings into lists, dividing them based on specified delimiters or whitespace. This approach allows us to break down text into smaller, more manageable components. By applying this knowledge to a security log example, we can extract individual data points and store them in a list, enabling further analysis and utilization within our code

To begin, let's examine the structure of our inputs and devise a plan for developing our program. We possess a log file stored in .txt format, with each line representing a username corresponding to a failed login attempt. Our objective is to create a program that checks for a given username and counts the number of times it appears in the log file. If the username occurs three or more times, the program will generate an alert.

We will commence by importing the file containing the login attempts, splitting its contents, and storing them in a variable called "usernames." To verify the contents of this variable, we will print it. Running the code confirms that the variable "usernames" accurately captures the expected information and is ready for implementation in our algorithm.

Next, we will devise a strategy to count the occurrences of a username within the list. Initially, let's consider the first eight elements of the "usernames" list. We observe two instances of the username "eraab." How can we instruct Python to count these occurrences? We will utilize a for loop that iterates through each element, represented by an arrow. Additionally, we will define a counter variable initialized to 0. The for loop starts with the username "elarson," and at each element, Python checks if it is equal to the string "eraab." If the condition is true, the counter increments by one; otherwise, it remains the same. This process continues for the entire list.

Having grasped the solution, let's discuss its implementation in Python. Solving the problem entails utilizing a for loop, a counter variable, and an if statement. Let's proceed with our code.

We will create a function named "login_check()" that counts the number of failed login attempts for a given user. The function takes two parameters: "login_list" represents the list of failed login attempts, and "current_user" denotes the user for whom we are checking the login attempts. Inside the function, we begin by defining the counter variable and setting its value to 0. Subsequently, we initiate the for loop, using "i" as the loop variable, to iterate through the "login_list." Within the for loop, we introduce an if statement that checks if the loop variable is equal to the "current_user" we are searching for. If the condition is true, we increment the counter by 1.

To complete our algorithm, we add a final if-else statement to print the alert. If the counter reaches or exceeds 3, we notify the user that their account is locked, preventing further login attempts. Additionally, we incorporate an else statement to indicate that users with fewer than three failed login attempts can log in. Our algorithm is now complete!

Let's test our new function with an example username. We can select a few usernames from the list and apply our function to them. For instance, we can begin with the first username in the list. Running the code reveals that this user can log in since they have fewer than three failed login attempts.

Now let's revisit the username "eraab." Recall that there were two occurrences of this username within the first eight entries of our failed login attempts. Do you believe they will be able to log in? Upon executing the code, we receive a message stating that their account is locked, indicating they had three or more failed login attempts.

# Debug Python

There are three distinct types of errors that can occur in Python programming: syntax errors, logic errors, and exceptions. Syntax errors involve improper usage of the Python language, such as forgetting to include a colon after a function header. Let's delve into this particular error type. When executing the code, a message appears indicating the presence of a syntax error. Additional details may also be displayed, depending on the Python environment. These errors are usually easy to rectify since they pinpoint the exact location of the problem. They are akin to correcting simple grammatical errors in an email. Since the error message specifies that the issue lies in the line defining the function, we can address it by adding a colon to the header. Upon rerunning the code, the error message disappears. This represents just one example of a syntax error. Other instances include omitting parentheses after a function, misspelling a Python keyword, or failing to properly close quotation marks in a string.

Moving on, logic errors differ from syntax errors in that they do not generate error messages, but instead yield unintended outcomes. A logic error could be as trivial as inserting incorrect text within a print statement or as significant as mistakenly using a less than symbol instead of a less than or equal to symbol. Such a change in the operator would exclude a necessary value, preventing the code from functioning as intended. For instance, suppose you alert a response team when the priority level of an issue is "less than three" instead of "less than or equal to three." This means all events categorized as priority level 3 might go unnoticed and unresolved.

To diagnose elusive logic errors, one effective strategy is to employ print statements. These statements need to be inserted throughout the code, describing their respective locations, such as "print line 20" or "print line 55: inside the conditional." The aim is to use these print statements to identify sections of the code that are functioning correctly. When a print statement does not yield the expected output, it helps identify problematic areas in the code.

Another option for identifying logic errors is utilizing a debugger. Debuggers allow the insertion of breakpoints into the code, enabling the execution of one segment at a time. Similar to print statements, running these segments independently helps isolate code issues.

Lastly, we encounter exceptions, which arise when the program encounters code that it does not know how to execute, despite having no syntax problems. Exceptions can occur for various reasons, such as attempting a mathematically impossible operation like dividing by zero, accessing non-existent index values, or using unrecognized variable or function names. Exceptions may also arise from utilizing an incorrect data type. To illustrate an exception, let's consider the following scenario.

Suppose there is a variable called "my_string" containing the word "security," which consists of eight characters. Consequently, we can successfully print any index value less than 8. For instance, index 0 holds "s," index 1 contains "e," and index 2 represents "c." However, if we try to access the character at index 100, an error occurs. Let's execute this code and explore the outcome. After successfully printing the initial three statements, an error message emerges: "string index out of range." When encountering exception errors, debuggers and print statements can also be employed to identify potential sources of the error.

# Glossary terms from week 4
Terms and definitions from Course 7, Week 4
Automation: The use of technology to reduce human and manual effort to perform common and repetitive tasks

Conditional statement: A statement that evaluates code to determine if it meets a specified set of conditions

Debugger: A software tool that helps to locate the source of an error and assess its causes

Debugging: The practice of identifying and fixing errors in code

Exception: An error that involves code that cannot be executed even though it is syntactically correct

File path: The location of a file or directory 

Function: A section of code that can be reused in a program

Integrated development environment (IDE): A software application for writing code that provides editing assistance and error correction tools

Iterative statement: Code that repeatedly executes a set of instructions

Log: A record of events that occur within an organization's systems 

Logic error: An error that results when the logic used in code produces unintended results

Parsing: The process of converting data into a more readable format

Syntax error: An error that involves invalid usage of a programming language

Variable: A container that stores data








