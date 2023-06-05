# Week 3
# Strings

It is important to have knowledge about working with string data in the context of security. One scenario where this is relevant is when analyzing login information and looking for patterns in usernames. In this course, we will revisit the string data type and learn how to work with it using Python.

To start, let's have a quick refresher on strings. In Python, strings are defined as ordered sequences of characters enclosed in quotation marks. Both double and single quotation marks are acceptable, but in this course, we have been using double quotation marks. For example, "Hello," "123," and "Number 1!" are strings we have encountered.

Next, let's recap variables. Currently, the variable "my_string" stores the string "security."

You can also create a string from other data types, such as integers or floats. To do this, we introduce a new built-in function called the string function. The string function converts an input object into a string, enabling us to perform string-specific tasks. For example, converting an integer to a string allows us to remove or reorder its elements, which is not possible with an integer data type.

Let's practice converting an integer to a string. We'll apply the string function to the integer 123. The variable "new_string" will now hold a string with three characters: 1, 2, and 3. To confirm the conversion, we'll print its type, and we should see that it is now a string.

Now that we have learned different ways to create and store strings, let's explore some basic string operations.

The first operation we'll discuss is finding the length of a string. The length function returns the number of elements in an object. When applied to a string, it tells us the number of characters it contains. For instance, a security professional might use the length function to check the validity of an IPv4 address. If the length exceeds 15 characters, it indicates an invalid IPv4 address.

Let's use the length function to print the length of the string "Hello." We'll nest the length function within the print function to calculate the length and display it on the screen. Running this code will output 5, which corresponds to the five letters in the word "Hello."

We can also concatenate strings using the addition operator. String concatenation involves joining two strings together. For example, we can concatenate "Hello" and "world" to obtain "Helloworld" with no spaces between them. However, some operators, such as the minus sign, do not work for strings.

Finally, let's discuss string methods. Methods are functions specific to a particular data type. Attempting to use a string method on another data type, like an integer, will result in an error. Two common string methods are "upper" and "lower." The "upper" method returns a copy of the string with all uppercase letters, while the "lower" method returns a copy with all lowercase letters.


"In the context of security, there are various situations where we may need to search within a string. For instance, we might need to locate a specific username in a security log or search for a known malicious IP address within a network log. To accomplish these tasks using Python, it's essential to understand the concept of indexing characters in a string.

In this video, the focus is on strings and their indices. Each character in a string is assigned an index number, starting from 0 in Python. For example, the character 'H' in the string 'HELLO' has an index of 0, 'E' has an index of 1, and so on. By using square brackets after a string and placing an index within them, we can retrieve the character at that particular index.

However, it's not just limited to accessing individual characters. Python allows us to extract a larger portion of a string through a process called slicing. Slicing involves specifying a starting index and an ending index, where the starting index is inclusive, but the ending index is exclusive. This means that the element at the ending index is not included in the slice. For example, to extract the letters 'E-L-L' from the string 'HELLO,' we would use the indices 1 (inclusive) to 4 (exclusive).

To search for a specific character in a string, we can utilize the index method in Python. The index method finds the first occurrence of the specified character within the string and returns its location. By providing the desired character as an argument to the index method, we can retrieve its index value. It's important to note that the index method is case-sensitive, so the character's case must be accurately represented.

If a character appears multiple times in the string, the index method will only identify the first occurrence. It's crucial to be aware of this behavior when working with the index method. As a security analyst, understanding how to work with indices empowers you to locate specific parts within a string efficiently, such as finding the position of the '@' symbol in an email address.

Lastly, it's worth noting that strings in Python are immutable, meaning they cannot be changed after they are created and assigned a value. Attempting to modify a character within a string directly will result in an error. This immutability is an important characteristic of strings in Python.

Let's apply the "upper" method to the string "Hello" and print the result. To use a method, we append a period (dot) to the string, followed by the method we want to use, in this case, "upper()". Running this code will print "HELLO" in all uppercase letters.

Similarly, the "lower" method converts the string to all lowercase letters. Applying the "lower" method to the "Hello" string and printing the result will display the string in all lowercase letters.

# Working with Lists

Previously, we discussed another data type called a list, which is a valuable tool for storing multiple data elements in a single variable. In the field of security, working with lists is essential. For example, you may encounter scenarios where you need a list of IP addresses that have accessed a network or a list containing information about blocked applications on a system.

To create a list in Python, you use square brackets to enclose the items, separating them with commas. You can also assign the list to a variable for easier access. For instance, by defining a variable called my_list and enclosing the items 'A' through 'E' within square brackets.

Similar to strings, you can access specific elements from a list using index values within square brackets. In Python, indexing starts from 0, so the index of the first element is 0, the second element is 1, and so on. By placing the desired index after the variable name and enclosing it within square brackets, you can retrieve the corresponding element from the list.

To extract elements from a list, you can use slicing, concatenation, and other list-specific operations. Slicing allows you to specify a range of indices to extract a subset of the list. You can concatenate lists using the plus sign, combining the elements of one list with another.

While strings are immutable in Python, meaning they cannot be changed after creation, lists do not share this limitation. Lists are mutable, enabling you to modify, add, or remove values freely. For example, if you have a list of malicious IP addresses, you can easily add new addresses to the list when they are identified.

To change a specific element within a list, you can use variable assignment. By combining bracket notation with variable assignment, you can reassign an element to a new value. Additionally, Python provides methods for inserting and removing elements from a list. The insert method allows you to add an element at a specified position, while the remove method deletes the first occurrence of a specific element in the list.

Understanding the differences between lists and strings is important. While strings are immutable, lists offer flexibility for modifying and managing data. By leveraging these list operations, you can efficiently handle and manipulate collections of information within your security analysis tasks.


In our daily lives, we often follow a set of rules to solve problems. Let's take a simple example of making a cup of coffee. If you have experience making coffee, you likely have a process that you follow. First, you grab your favorite mug. Then, you add water to the coffee maker and put in the coffee grounds. After pressing the start button, you wait a few minutes. Finally, you can enjoy your freshly brewed cup of coffee.

Even if you have a different approach to making coffee or don't drink coffee at all, you probably have a set of rules or steps that you follow when completing similar everyday tasks. When you follow these routine tasks, you're essentially following an algorithm. An algorithm is a set of rules that solves a problem. It consists of a series of steps that take an input, perform tasks based on that input, and provide a solution as an output. In the context of this course, we will explore how algorithms can be utilized to solve problems using Python.

Let's consider a scenario where you, as a security analyst, have a list of IP addresses. Your objective is to extract the first three digits from each IP address, as this information can provide insights about the corresponding networks. To achieve this, we'll develop an algorithm that incorporates various Python concepts we've covered so far, including loops, lists, and strings.

We have a list of IP addresses stored as strings. For privacy reasons, we won't display the complete IP addresses in our example. Our goal is to extract the first three numbers from each address and store them in a new list. Before diving into the Python code, let's outline an algorithmic approach to solving this problem. Imagine you had just one IP address instead of a list. In that case, the problem becomes simpler. The first step would involve using string slicing to extract the first three digits from that IP address. Now, let's consider how to apply this approach to the entire list. As the second step, we'll use a loop to apply the same solution to every IP address in the list. As you've previously learned about string slicing, let's write some Python code to solve this problem for a single IP address.

In our example, we start with an IP address that begins with "198.567." We'll write a few lines of code to extract the first three characters. By using bracket notation, we can slice the string. Inside the print statement, the "address" variable holds the IP address we want to slice. Keep in mind that Python starts counting at 0. To obtain the first three characters, we start our slice at index 0 and continue until index 3. Remember, Python excludes the final index. In other words, Python will return the characters at index 0, 1, and 2. Running this code will display the first three digits of the address: "198." Once we solve the problem for a single IP address, we can encapsulate the code within a loop and apply it to all IP addresses in the original list. Before proceeding, let's introduce one more method that we'll utilize in this code: the "append" method.

The "append" method adds an input to the end of a list. For instance, if our list contains 1, 2, and 3, we can use the "append" method to add 4 to the list. Now that we have our IP list, we can proceed to extract the first three characters from each element and store them in a new list. Let's create an empty list called "networks" to store the first three characters of each IP from the list. With the "for" loop, we can iterate through each element in the IP list.

Inside the loop, the keyword "for" signals the start of the loop in Python. We specify "address" as the variable that temporarily holds each element from the IP list, and "IP" represents the iterable list. As the loop executes, each IP address will be stored in the "address" variable one at a time. Within the loop, we include a line of code that appends the sliced portion of the "address" to the "networks" list.

To break it down further, we reuse the code we previously wrote to extract the first three characters of an IP address. By utilizing the "append" method, we add the extracted portion to the "networks" list. Finally, we print the "networks" list and run the code. The variable "networks" now contains a list with the first three digits of each IP address from the original list.

# Regular Expressions


"We will explore the concept of searching for patterns in strings using regular expressions. Regular expressions, also known as regex, are sequences of characters that form patterns. These patterns are useful when searching through log files, as they allow us to find specific patterns within the text. For example, we can search for strings that start with a particular prefix or strings of a certain length. In a security context, regular expressions can be applied in various ways. For instance, we can efficiently search for IP addresses with a specific network ID, thanks to regular expressions.

Let's consider an example mentioned in the video. Suppose we want to extract all the email addresses from a log. If we were to use the index method for this task, we would need to know the exact email addresses we are searching for. However, as security analysts, we often don't have that level of specific information. By using regular expressions, we can define the structure of an email address, and Python will return all the strings that match that structure. This means that even if we have a log file with thousands of lines and entries, we can extract all the email addresses by searching for the email address structure using a regular expression, without needing to know the actual emails beforehand.

To achieve this, we need to understand the symbols used in regular expressions. Let's start by discussing the plus sign (+). In regular expressions, the plus sign represents one or more occurrences of a specific character. For example, the pattern "a+" matches a string of any length where the character 'a' is repeated. It can be a single 'a', three consecutive 'a's, or even a thousand consecutive 'a's. We can apply this pattern to extract specific strings.

In the video, a string of device IDs was used as an example. Each instance contains one or more consecutive occurrences of the letter 'a'. By using the regular expression pattern "a+", Python would return a list of all the 'a's in these strings, including those with varying numbers of occurrences.

Another symbol we discussed is "\w", which matches any alphanumeric character but excludes symbols. For example, it matches characters like "1", "k", and "i".

Regular expressions become even more powerful when we combine symbols. By combining "\w" with the plus sign (+), we can create more complex patterns. "\w+" matches an alphanumeric string of any length. The "\w" provides flexibility in the alphanumeric characters that can be matched, and the plus sign allows for varying string lengths. This pattern can match strings like "192", "abc123", and "security".

Now, let's apply these concepts to extracting email addresses from a log. An email address typically consists of text separated by specific symbols like "@" and ".". We can represent this as a regular expression.

The first segment of an email address usually contains alphanumeric characters, and the length can vary. We can use the regular expression pattern "\w+" to match an alphanumeric string of any length. The "@" symbol follows this segment, and it is always present in an email address. We include it directly in the regular expression to ensure proper identification of email addresses. The next segment is the domain name, which also contains alphanumeric characters. Again, we use "\w+" to match this segment, allowing for variations in length.

The final part is the period (".") symbol, which is always present in an email address. However, in regular expressions, the period has a special meaning, so we need to use a backslash before it ("."). This lets Python know that we want to match the actual period symbol.

By combining these pieces, we create a regular expression pattern that matches email addresses and excludes everything else in the string. It follows the structure of an email address by including the "@" symbol and the period where they appear.

To implement this in Python, we need to import the 're' module, which provides regular expression functionality. We start by importing this module. Then, assuming we have a log stored as a multi-line string variable named 'email_log', we can apply the 'findall()' function from the 're' module to search for matches based on our regular expression pattern. The 'findall()' function returns a list of all matches found in the string.

In our case, we use the regular expression pattern for email addresses as the first argument of 'findall()', enclosed in quotation marks. The second argument is the string variable 'email_log', which is the text we want to search through. Running this code will provide us with a list of all the email addresses found in the string. This approach can be scaled to handle logs with thousands of entries."

Note: The timestamps provided in the original text refer to specific points in a video, and without the accompanying visual content, it may be challenging to follow them precisely. However, the information from the transcript is explained comprehensively above.

# Glossary terms from week 3
Terms and definitions from Course 7, Week 3
Algorithm: A set of rules that solve a problem

Bracket notation: The indices placed in square brackets 

Debugging: The practice of identifying and fixing errors in code

Immutable: An object that cannot be changed after it is created and assigned a value

Index: A number assigned to every element in a sequence that indicates its position

List concatenation: The concept of combining two lists into one by placing the elements of the second list directly after the elements of the first list

List data: Data structure that consists of a collection of data in sequential form

Method: A function that belongs to a specific data type

Regular expression (regex): A sequence of characters that forms a pattern

String concatenation: The process of joining two strings together

String data: Data consisting of an ordered sequence of characters

Substring: A continuous sequence of characters within a string
