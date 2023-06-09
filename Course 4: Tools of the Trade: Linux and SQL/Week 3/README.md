# Week 3
# Linux Commands in the Bash Shell


Linux commands are essential for security professionals, particularly security analysts who work with server logs and need to navigate, manage, and analyze files remotely without a graphical user interface. It is crucial for them to know how to verify and configure user and group access, grant authorization, and set file permissions. The command line is a fundamental tool for these tasks. The Bash shell is the default shell in most Linux distributions and will be utilized in this section.

Communicating with the operating system in Linux is like having a conversation. Commands are typed in, and the OS responds with an answer. The prompt, indicated by a dollar sign, indicates that a new command can be entered. Commands can instruct the computer to find files, launch programs, or output specific text strings. The echo command, for example, is used to output text.

Commands often require arguments, which provide specific information needed by the command. Arguments can take various forms, including text strings. It is important to note that Linux commands and arguments are case sensitive, including file and directory names.

Developing proficiency in Linux commands is vital for security analysts in their day-to-day tasks. Understanding the basics of Linux architecture, utilizing the Bash shell, and mastering commands and arguments will enable them to effectively navigate, manage, and secure systems and files.

![image](https://github.com/benichi2022/googlecybersecurityprofessionalcertificate/assets/113864743/17eb25e8-21bd-4592-9dc7-2eac22534ce3)

The Linux architecture is organized by the Filesystem Hierarchy Standard (FHS), which treats everything in Linux as a file within the system's directory structure. The FHS is hierarchical, with the root directory as the highest level, designated by a single slash. Subdirectories branch out from the root, and slashes are used to trace back to the root when describing the directory structure. Navigating the file system is crucial for security analysts to locate and analyze log files and other data.

To navigate the file system, several commands are commonly used. The "pwd" command displays the current working directory, showing the user's location within the file system. The "ls" command lists the files and directories in the current working directory. The "cd" command is used to change directories, allowing users to move between different locations in the file system.

In Bash, the command prompt, executing these commands is straightforward. Typing "pwd" displays the current location, "ls" lists the files and directories, and "cd" is used to change to a different directory. For example, using "cd logs" changes the working directory to the "logs" subdirectory.

As a security analyst, it's important to read file content in Linux. The "cat" command displays the entire content of a file, which can be useful for examining configuration settings or user access reports. If dealing with large files, the "head" command can be used to display only the first few lines of a file, typically ten lines by default.

Practicing these commands, such as using "cat" or "head" followed by the file name, allows security analysts to read and analyze specific file contents, providing insights into potential vulnerabilities or unauthorized access.

By understanding the Linux file system structure and mastering essential commands for navigation and file content reading, security analysts can effectively perform their tasks and analyze critical data in their day-to-day work.

# Manage Files in Bash

Filtering is an essential skill for security analysts, as it allows them to search for specific information within the Linux system to solve complex problems. One powerful command for filtering is "grep," which searches a specified file for lines containing a particular string. For example, using the command "grep OS updates.txt" searches the "updates.txt" file for lines that contain the word "OS," returning the matching lines.

Another useful concept in Linux filtering is piping. Piping involves sending the output of one command as the input for another command using the "|" (pipe) character. It allows for further processing of data. In the context of filtering, piping can be used to combine commands and perform more complex searches. For instance, using the command "ls | grep users" lists the files and directories in the "reports" subdirectory and then filters the output to display only those that contain the word "users."

In Bash, you can practice these filtering techniques. By using the "ls" command with the appropriate directory path, you can list the contents of a specific directory. To further filter the output, you can combine the "ls" command with piping and the "grep" command. For example, running "ls reports/ | grep users" displays only the files in the "reports" directory that contain the word "users."

By mastering commands like "grep" and understanding how to use piping, security analysts can efficiently search for and filter specific information within the Linux system. These techniques enable them to investigate potential security threats, analyze logs, and identify patterns or indicators of compromise.

In this video, we explore how to create, modify, and organize directories and files in Linux. Directories serve as a way to organize information and files within the Linux system. Understanding how to navigate and manipulate directories is crucial for security analysts.

To create a new directory, we use the "mkdir" command, followed by the desired directory name. Conversely, the "rmdir" command allows us to remove or delete a directory, with a built-in warning if the directory is not empty. Similarly, we can create and remove files using the "touch" and "rm" commands, respectively.

Moving and copying files or directories can be done with the "mv" and "cp" commands. The "mv" command moves a file or directory to a new location, while the "cp" command makes a copy of a file or directory.

To demonstrate these commands, we begin by using "pwd" to display the current directory and "ls" to list the files and directories within the current directory. We then proceed to remove a directory called "oldreports" using the "rmdir" command. Afterward, we create a new directory called "drafts" using the "mkdir" command.

Next, we navigate into the "drafts" directory using "cd" and confirm its emptiness with "ls". We create two files, "email_patches.txt" and "OS_patches.txt", using the "touch" command. To delete a file, we employ the "rm" command followed by the file name.

Moving on to moving and copying files, we use the "mv" command to move the file "email_policy.txt" from one directory to another. Similarly, the "cp" command allows us to copy the "vulnerabilities.txt" file into another directory without removing the original.

Additionally, we explore the use of file editors, specifically the "nano" editor. This editor is commonly used for writing and modifying files. We open the "OS_patches.txt" file with "nano", add a title, save the changes using Ctrl+O, and exit the editor with Ctrl+X.

Understanding these commands and concepts empowers security analysts to efficiently manage and organize files and directories within the Linux system. This knowledge is crucial for maintaining a structured and secure environment for data analysis and investigation.

# Authenticate and Authorize Users


In this video, we explore how to create, modify, and organize directories and files in Linux. Directories serve as a way to organize information and files within the Linux system. Understanding how to navigate and manipulate directories is crucial for security analysts.

To create a new directory, we use the "mkdir" command, followed by the desired directory name. Conversely, the "rmdir" command allows us to remove or delete a directory, with a built-in warning if the directory is not empty. Similarly, we can create and remove files using the "touch" and "rm" commands, respectively.

Moving and copying files or directories can be done with the "mv" and "cp" commands. The "mv" command moves a file or directory to a new location, while the "cp" command makes a copy of a file or directory.

To demonstrate these commands, we begin by using "pwd" to display the current directory and "ls" to list the files and directories within the current directory. We then proceed to remove a directory called "oldreports" using the "rmdir" command. Afterward, we create a new directory called "drafts" using the "mkdir" command.

Next, we navigate into the "drafts" directory using "cd" and confirm its emptiness with "ls". We create two files, "email_patches.txt" and "OS_patches.txt", using the "touch" command. To delete a file, we employ the "rm" command followed by the file name.

Moving on to moving and copying files, we use the "mv" command to move the file "email_policy.txt" from one directory to another. Similarly, the "cp" command allows us to copy the "vulnerabilities.txt" file into another directory without removing the original.

Additionally, we explore the use of file editors, specifically the "nano" editor. This editor is commonly used for writing and modifying files. We open the "OS_patches.txt" file with "nano", add a title, save the changes using Ctrl+O, and exit the editor with Ctrl+X.

Understanding these commands and concepts empowers security analysts to efficiently manage and organize files and directories within the Linux system. This knowledge is crucial for maintaining a structured and secure environment for data analysis and investigation.


In this video, we learn about the "chmod" command, which allows security analysts to change permissions for users on files and directories in Linux. Changing permissions is important to protect system files from unintended or deliberate alterations or deletions.

The "chmod" command operates in symbolic mode, and understanding its usage is best demonstrated through an example. The command requires two arguments: the file or directory for which permissions will be adjusted and the mode of the permission change.

To specify the owner types (user, group, and other), we use symbols: "u" for user, "g" for group, and "o" for other. These owner types are separated by commas in the argument.

Mathematical operators indicate whether permissions should be added or removed. The plus sign (+) adds permissions, while the minus sign (-) removes them. The symbols "r" (read), "w" (write), and "x" (execute) represent the type of permission being added or removed.

To demonstrate the command, we start in the "logs" sub-directory and use the "ls -l" command to view the current permissions. We then modify the permissions to grant write permissions to the security group and remove read permissions for others.

Upon running "ls -l" again, we can observe the changes in the permissions for the file. The write permission is added for the group, while the read permission is removed for others.

Understanding and utilizing the "chmod" command empowers security analysts to manage permissions effectively, ensuring appropriate access controls and maintaining system security.


In this video, we explore the concept of authentication and the importance of managing user access in a system. Users need to prove their identity to gain access, just like in a physical building where not all users should be allowed in.

Adding users is necessary when new individuals join an organization or a specific group within it. Conversely, users who leave the organization or change groups need to be deleted to revoke their access privileges.

Additionally, the video introduces the concept of the root user, who has elevated privileges to modify the system. Regular users have limitations compared to the root user. However, logging in as the root user and running commands with root privileges is considered risky due to security risks, potential irreversible mistakes, and lack of accountability.

To address these concerns, the video presents the "sudo" command as an alternative to running commands as the root user. "sudo" allows specific users to temporarily gain elevated permissions, providing a more controlled approach. Users granted sudo access must be configured in the "sudoers" file.

The video demonstrates how to use "sudo" with the "useradd" command to add a new user and the "userdel" command to delete a user. These commands require root or sudo privileges, ensuring that only authorized users can perform these actions.

Managing user access and utilizing commands like "sudo," "useradd," and "userdel" allows for controlled user authentication and enhances system security by granting appropriate access privileges and revoking them when necessary.

Linux Community, google, stackoverflow and man pages within the shell help you learn linux and search for commands and their uses.


# Glossary terms from week 3
Terms and definitions from Course 4, Week 3
Absolute file path: The full file path, which starts from the root

Argument (Linux): Specific information needed by a command

Authentication: The process of verifying who someone is

Authorization: The concept of granting access to specific resources in a system

Bash: The default shell in most Linux distributions

Command: An instruction telling the computer to do something

File path: The location of a file or directory

Filesystem Hierarchy Standard (FHS): The component of the Linux OS that organizes data

Filtering: Selecting data that match a certain condition

nano: A command-line file editor that is available by default in many Linux distributions

Options: Input that modifies the behavior of a command

Permissions: The type of access granted for a file or directory

Principle of least privilege: The concept of granting only the minimal access and authorization required to complete a task or function

Relative file path: A file path that starts from the user's current directory

Root directory: The highest-level directory in Linux

Root user (or superuser): A user with elevated privileges to modify the system

Standard input: Information received by the OS via the command line

Standard output: Information returned by the OS through the shell


