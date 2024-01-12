# Lab 1 Report
---
This lab focuses on the "cd", "ls" and "cat" terminal commands and how they work with different types of arguments: no arguments, directory path, and file path.

* cd
1. No arguments: The command changes the working directory back to the root directory.
2. A path to a directory as an argument: The command changes the working directory to the directory specified in the path.
3. A path to a file as an argument: Error: The command fails to change directories since the specified path points to a file, not a directory.
* ls
1. No arguments: The command prints to console the names of the files and folders in the current directory.
2. A path to a directory as an argument: The command prints to console the names of the files and folders in the directory specified in the path.
3. A path to a file as an argument: The command prints the filename with the entire specified file path.
* cat
1. No arguments: The console waits for additional input from the user and then proceeds to print whatever you type in until you stop the process with Ctrl+C. 
2. A path to a directory as an argument: Error: The command fails to print anything since the specified path points to a directory, not a file.
3. A path to a file as an argument: The command prints the contents of the specified file in the filepath.
