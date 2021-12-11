# **Module 1:**
## **File I/O**
***

### **Reading Text Files**
* Since a file lives outside of the Python interpreter, we must ask the operating system to go and find the specified file.
    * Ex)
```python
my_file = open("testfile.txt)

for line in my_file:
    print(line, end = " ")

myfile.close()
```
> NOTE: 'end = " "' just tells the print statement what to end each print statement with, as the default is '\n', a newline character.
* If you try to open a file that does not exist, then you will receive an I/O error.
* In Python, the basics of processing a file looks like this:
    1. Open the file.
    2. For each line in the file:
        Do something.
    3. Close the file.
        * the file is not actually altered until it has been closed.
* To ensure entries in files are uniform, we often use CSV files:
    * Comma-separated-value (CSV) format
    * Ex)
        * Hermione, Granger, 10, 10, 10, 10, 10
        * Fred, Weasley, 4, , 5, , 3
        * Harry, Potter, 8, 6, 7, 8, 7
        * Rip, Van Winkle, 1, 2, 3, 4, 5
* To split a String using commas as a delimiter, use:
    * s.split(",")
* To check if a String is a digit, use:
    * s.isdigit()
* To read the lines of a file and store them as a list of Strings, use:
    * lines = my_file.readlines()
***

###  **Writing Text Files**
* There is a second parameter when opening a file to dictate whether or not you want to read, write, or append to the specified file.
    * Ex)
```python
f = open(filename) # open the file to read from it
f = open(filename, 'r') # same as above, open the file to read from it
f = open(filename, 'w') # open the file to write to it as a new file, this creates a new file entirely. IF A FILE WITH THE SAME NAME ALREADY EXISTS, THEN ITS CONTENTS WILL BE DESTROYED.
f = open(filename, 'a') # open the file to append, or add, to it
```
* To write to a file that has been opened in write or append mode, use:
    * myfile.write("Hello!")
> NOTE: if you want to create a new line in a file, '.write(String)' does not do it automatically - you must actually write the newline character.
> NOTE: the parameter for the write function must be a SINGLE String.
* To write a newline to a file, you must manually do so:
    * myfile.write("\n")
* To protect important files from being overwritten, simply set certain user-restrictions or make the file 'Read-Only'.
***

### **File Paths and Command Shells**
* While many 'complete', or advanced, programs use a GUI, many scripts are used through the command shell, such as Mac OS's Terminal, or Windows' Command Prompt.
    * Window's Command Shell Cursor: '>'.
        * 'dir' - lists the current directory and its sub-directories.
        * 'cd \' - return to the root directory.
        * 'type fileName.txt' - prints the contents of the specified text file in the Command Prompt.
    * Mac's Command Shell Cursor: '$'.
        * ~ - the abbreviation for the 'home directory'.
        * 'pwd' - print working directory (displays the full path of the current directory).
        * 'ls' - prints the names of the current directory's sub-directories.
        * 'ls -l' - prints the names AND extensions of the files and folders inside of the current directoy.
            * if the entry begins with a 'd', then we know that it is a folder / sub-directory.
        * 'cd /' - return to the root directory.
        * 'cat fileName.txt' - prints the contents of the specified text file in the Terminal.
* Navigating through the file system:
    * Every file has an absolute path, and a relative path.
        * Absolute path - the sequence of directories that is the unique address for any file or folder.
            * root -> Users -> username.
                * the 'username' directory is your 'home directory'.
        * Relative path - the sequence of directories starting from the current working directory.
* Windows: C:\Users\username\cs104\chapter21\testfile.txt
    * C:\ - root directory
* Mac: \Users\username\cs104\chapter21\testfile.txt
    * \ - root directory
* 'cd' - change directory
* 'cd ..' - go up one level in the directory (the current directory's parent directory).
* Use the up-arrow to cycle through previos commands.
* Use the 'TAB' button to auto-fill commands.
* On Windows, drives are named using letters.
* On Mac, drives are named using actual names.
* To run the Python interpreter through the Command Prompt on Windows, you must first provide the absolute path of the Python executable. 
    * To quit, enter: 'quit()'.
* To run the Python interpreter through the Terminal on Mac, you only need to type 'python', since the Mac OS Terminal already has the Python interpreter installed.
    * To quit, enter: 'quit()'.
> To run a Python script which is contained in the working directory, simply write 'python scriptName.py'. However, if the script is not contained in the working directory, use the relative or absolute path of the script.
***