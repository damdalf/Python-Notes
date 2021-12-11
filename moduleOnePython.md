# **Module 1:**
## **The Python Programming Language**
***

### **Vocabularly:**

* Python is a high-level language.
> High-level languages are preferred because they allow programs to be written more easily and quickly, they are shorter and easier to read, and they are more likely to be correct. More importantly, they are portable -> they can run on different kinds of computers with few or no modifications.

* Low-level languages - machine languages or assembly languages. 
> Technically, computers can only execute code written in low-level languages, meaning that any high-level code must be translated into machine language before being able to run.

* Interpreter - Python's compiler.

* Python Shell - an interactive user interface to the Python interpreter. 
> The 'shell' word comes from Linux

* '>>>' is called the Python Prompt, and it serves to indicate that the interpreter is ready for more instructions (code). 

* Script - a program that is written in a file in which it uses the interpreter to execute the contents of the file. 
> Scripts have the advantage that they can be saved to disk, printed, and so on. 

* Immediate mode - a style of using Python where we type expressions at the command prompts, and the results are displayed immediately. 

* Object code - the output of the compiler after it translates the program. 

* What separates an IDE from a text editor? 
> A text editor can only edit the code, but an IDE can interact with the Interpreter / Compiler. 

***

This is obvious information, but not having seen it for ages, I think it is something good to remember when you're frusturated with a current project or assignment.

### **What Five Components Build a Program?**

1. input
2. output
3. math
4. conditions execution
5. repetition

***

### **Quick Ideas:**

* A 'runtime error' is also known as an 'exception'.
* Semantic / logic errors - these errors occur when your code runs, but it does not complete the desired results / performance.
* Tokens - the basic elements of a language: words, numbers, parentheses, commas, etc.
* Structure - the way that tokens are arranged. 
* The meaning of a computer program is ambigious and and literal. 
> This is why coding is nice lol. 

***

### **Basic Functions / Syntax:**

* print(String)
* '#' - comment
* Variable Types:
    * str
    * int
    * float

* type(literal) - returns the data type of the literal.

* Strings can be enclosed in double-quotes and single-quotes, and either of the two can appear in Strings themselves. 

* Triple-doubly-quoted strings can span several lines. 

* len(String) - returns the number of characters in a String. 

* The dvision operator always yields a floating-point result. 

* Floor division, in which an int is returned (similar to the modulo operator in Java and C), is used by '//', but essentially takes only the whole number. 

* '%' - works on integers, and gives the remainder when the first number is divided by the second. 

* the int() type converter can take in a str or a float and convert it into an int, but it will ignore the decimals if it contians any. 

* the float() type converter can turn in an integer, a float, or a string and convert it into a float.

* the str() type converter can turn its argument into a str. 

* input(str user_prompt) - built-in function in Python for getting input from the user. 
    * Note that the input always returns a str.
> name = input("Please enter your name: ")


***

### **Python Info:**

* State-snapshot - shows what state each of the variables is, at a particular time. 

* Variables are commonly named using lower-case letters and underscores in Python.

* Statement - an instruction that the compiler (interpreter) can execute.

* Expression - a combination of values, variables, operators, and calls to functions.

***

### **Operator Precedence**

1. Parentheses
2. Exponentiation
3. Multiplication, Division
4. Addition, Subtraction
> Note how multiplication equals division for their orders of precedence, and the same with addition and subtraction.