# Week 1
# Introduction to Operating Systems

Operating systems are essential components found in devices like computers, smartphones, and tablets. When using a desktop or laptop computer, you may have encountered operating systems such as Windows or MacOS. Mobile devices like smartphones and tablets rely on mobile operating systems like Android and iOS. Another widely used operating system is Linux, especially in the security industry. As a security professional, it's highly likely that you will engage with the Linux OS.

The operating system serves as the interface connecting computer hardware and users. Commonly referred to as the OS, it plays a crucial role in optimizing computer performance and ensuring user-friendly interactions. Hardware, on the other hand, refers to the physical components of a computer.

In the past, early computers faced a major challenge: the significant time required to run computer programs. Unlike modern systems, those computers couldn't handle multiple programs simultaneously. Users had to patiently wait for one program to finish running, then reset the computer and load the next program. Imagine turning your computer on and off every time you needed to open a new application! Simple tasks like sending emails would take an eternity. Thankfully, operating systems have evolved, eliminating such time-consuming processes. Today's computers efficiently run multiple applications and seamlessly connect with external devices like printers, keyboards, and mice.

Operating systems also play a crucial role in enabling communication between humans and computers. Computers communicate using binary language, comprising 0s and 1s. The OS acts as an interface that bridges the communication gap, allowing users to interact with computers in more complex ways.

Given the importance of operating systems, securing them becomes paramount for overall computer security. This involves safeguarding files, controlling data access, and implementing user authentication to protect against threats like viruses, worms, and malware. Understanding how operating systems function is essential for performing various security-related tasks. As a security analyst, you may be responsible for configuring and maintaining system security, managing access, setting up firewalls, enforcing security policies, enabling virus protection, and detecting unusual behavior through auditing, accounting, and logging. All these responsibilities demand a comprehensive understanding of operating systems, which we will explore further in this course.

# The Operating System at Work

Consider the scenario of driving a car. When someone presses the gas pedal, the car moves forward effortlessly. They don't need to concern themselves with the intricate mechanics behind the car's movement. Similarly, just as a car cannot function without its engine, a computer cannot operate without its operating system.

The purpose of an operating system (OS) is to facilitate the efficient execution of other computer programs. It accomplishes this by managing all the intricate details involved in controlling the computer's hardware, relieving users of that burden.

When you power on your computer, a sequence of events takes place. Pressing the power button initiates a direct interaction with the hardware, booting up the computer and activating the operating system. This booting process involves a specialized microchip known as the BIOS or, in more recent computers, the UEFI. Both contain instructions responsible for loading the bootloader, a program tasked with initiating the operating system. Just like that, your computer springs to life.

Understanding these processes is particularly valuable for security analysts. Vulnerabilities can arise during the booting process, as the BIOS is often not scanned by antivirus software, making it susceptible to malware infection. Now that you comprehend the booting process, let's explore how you and other users communicate with the system to accomplish tasks.

The process begins with you, the user, utilizing applications on your computer to complete specific tasks. An application is a program designed for a particular purpose. When you make a request through the application, it communicates with the operating system. The operating system then interprets and directs this request to the appropriate hardware component of the computer.

In our previous video, we discovered that hardware encompasses all the physical components of the computer. The hardware also relays information back to the operating system, which, in turn, communicates with the application.

To illustrate, let's take a simple example of using the calculator application on your computer. You click on the calculator using your mouse. As you input the desired number for calculation, the application communicates this to the operating system. Subsequently, the operating system dispatches the calculation to a hardware component known as the central processing unit (CPU). Once the hardware completes the calculations and determines the final number, it transmits the answer back to the operating system, which then displays it in your calculator application.

Having a grasp of this process proves invaluable when investigating security events. Security analysts should be capable of retracing this flow to analyze where a security incident may have occurred.

The operating system (OS) not nly interacts with various components of the computer but also manages its resources. Similar to how a person needs energy for different tasks, the OS ensures efficient utilization of the computer's resources. For example, running an antivirus scan requires more resources than using a calculator application.

In the analogy of an orchestra, the OS acts as the conductor. It handles resource and memory management to optimize the limited capacity of the computer system. Different programs, tasks, and processes compete for the resources of the central processing unit (CPU), and the OS allocates and de-allocates resources accordingly. This orchestration occurs simultaneously, enabling the efficient functioning of the system.

While much of this resource management is hidden from users, tools like a browser's task manager reveal the tasks being processed and their resource usage. As an analyst, understanding resource usage helps in incident response and troubleshooting. For instance, a slow-running computer could be allocating resources to malware. Grasping the basics of operating systems enhances comprehension of the security skills to be learned later in the program.

# The User Interface

The operating system can be interacted with through user interfaces, such as the graphical user interface (GUI) and the command-line interface (CLI). The GUI utilizes icons and graphics on the screen to manage tasks, commonly seen in personal computers and cell phones. It includes components like a start menu, taskbar, and desktop icons. On the other hand, the CLI is a text-based interface that relies on commands to interact with the computer. It lacks graphical elements but offers greater flexibility and power, allowing for simultaneous execution of multiple tasks. Security analysts often employ the CLI for tasks like log analysis and user authentication. Understanding both interfaces is important, and the program will provide practical experience using the CLI in Linux.

# Glossary terms from week 1
Terms and definitions from Course 4, Week 1
Application: A program that performs a specific task

Basic Input/Output System (BIOS): A microchip that contains loading instructions for the computer and is prevalent in older systems 

Bootloader: A software program that boots the operating system

Command-line interface (CLI): A text-based user interface that uses commands to interact with the computer

Graphical user interface (GUI): A user interface that uses icons on the screen to manage different tasks on the computer

Hardware: The physical components of a computer

Legacy operating system: An operating system that is outdated but still being used

Operating system (OS): The interface between computer hardware and the user

Unified Extensible Firmware Interface (UEFI): A microchip that contains loading instructions for the computer and replaces BIOS on more modern systems

User interface: A program that allows the user to control the functions of the operating system
