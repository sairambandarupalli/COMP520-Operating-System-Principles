# COMP520-Operating-System-Principles

# Explaination of ProjectA
The code initializes variables for video memory and a string. It uses a loop to write each character and a white color attribute to consecutive video memory locations. The program then enters an infinite loop, keeping the message on the screen. However, the putInMemory function, responsible for writing to memory, is not provided in the snippet.

To verify the code, run the commands in terminal chmod + x compileOS.sh and ./compileOS.sh If the code run successfully, then run java -jar simulator.jar

# Explanation of ProjectB
The main function takes a sector from the disc, reads user input, and sets up interrupt handling.Using BIOS video interrupts, the printString and printChar functions output characters and strings to the screen.The function readString receives input from the user and manages backspace for editing.The handleInterrupt21 function uses BIOS interrupts to carry out various activities, routing them according to the value of the 'ax' register. 

To verify the code, run the commands in terminal chmod + x compileOS.sh and ./compileOS.sh If the code run successfully, then run java -jar simulator.jar
