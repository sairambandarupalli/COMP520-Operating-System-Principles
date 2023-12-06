# COMP520-Operating-System-Principles

# Explanation of ProjectA (The below description is only about kernel.c and it's essential to acknowledge that the given description doesnot include the entire code and might make reference to supplementary functions that are not explicitly outlined.)
The code initializes variables for video memory and a string. It uses a loop to write each character and a white color attribute to consecutive video memory locations. The program then enters an infinite loop, keeping the message on the screen. However, the putInMemory function, responsible for writing to memory, is not provided in the snippet.

To verify the code, run the commands in terminal chmod + x compileOS.sh and ./compileOS.sh. If the code runs successfully, then run java -jar simulator.jar

# Explanation of ProjectB (The below description is only about kernel.c and it's essential to acknowledge that the given description doesnot include the entire code and might make reference to supplementary functions that are not explicitly outlined.)
The main function takes a sector from the disc, reads user input, and sets up interrupt handling. Using BIOS video interrupts, the printString and printChar functions output characters and strings to the screen. The function readString receives input from the user and manages backspace for editing. The handleInterrupt21 function uses BIOS interrupts to carry out various activities, routing them according to the value of the 'ax' register. 

To verify the code, run the commands in terminal chmod + x compileOS.sh and ./compileOS.sh. If the code runs successfully, then run java -jar simulator.jar

# Explanation of ProjectC (The below description is only about kernel.c and shell.c, it's essential to acknowledge that the given description doesnot include the entire code and might make reference to supplementary functions that are not explicitly outlined.)
The kernel is responsible for initializing an interrupt vector table and performing various tasks. One of these tasks involves reading the contents of a file named "message" into a buffer and displaying the content. If the file is not found, the kernel starts a simple shell. This shell provides functions for file system operations, I/O tasks (such as printing strings and characters), and program execution. When the kernel needs to terminate, it executes a program called "shell" to return to the command prompt.

The shell, defined in shell.c, operates in a continuous loop, accepting user input and interpreting commands. It supports commands like "type" to display file contents and "exec" to run programs. If a command is not recognized, the shell handles it by printing appropriate messages. The provided code focuses on interacting with hardware through interrupt calls. The file system and shell components offer essential features for a basic operating system environment, and it is important to note that additional functions, not included in the provided snippet, are relied upon.

To verify the code, run the commands in terminal chmod + x compileOS.sh and ./compileOS.sh. If the code runs successfully, then run java -jar simulator.jar
