# **Python Module 4:**
## **Unit Testing, Incremental Development, Debugging, Binary Arithmetic, and Data Encoding.**
***

### **Unit Testing & Incremental Development:**
* Unit test - a script that calls a certain function several times and prints the following: the input being tested, the result we expect to get, and the result from the actual function call. 
    * a script that checks whether a function works correctly or not
* Incremental development - breaking your program down into several components that can be developed independently of each other, and testing each component.
***
### **Debugging**
* Syntax errors - code doesn't run at all
* Runtime errors - code starts to run but fails with an error
    * read errors from bottom-up
* Logic errors - program runs fine but does not execute as expected
    * creating local variables to print out more steps / states of your function to help solve logic errors
* In general, always unit test each component of your program during incremental development. 
* In Python:
    * 0 == False
    * non-zero numbers == True
    * empty string == False
    * non-empty string == True
    * However, it is best to always use boolean expressions in conditional statements to avoid confusion.
    ***

    ### **Binary Arithmetic & Data Encoding**
    * When working with computers at the most basic level, the only values that are used are 0's and 1's. 
    ![](https://i.gyazo.com/180e0a67616f45b9888d3f574be6410f.png)
    * When adding binary numbers together:
        * either find each binary number's value and complete basic addition
        * or add the binary numbers, 1 + 1 = 0 and the 1 is carried over to the left
* Binary digits 0 and 1 are called "bits".
* Eight bits is called a "byte".
* ASCII characters:
    * 48 - 57 = digits 0 - 9
    * 58 - 64 = symbols and punctuation
    * 65 - 90 = uppercase letters
    * 91 - 96 = symbols and punctuation
    * 97 - 122 = lowercase letters
    * 123 - 126 = punctuation
    * the only important control characters:
        * \n = newline / escape character
        * \t = tab character
    * How Carriage Retun Differs Across Operating Systems:
        * Windows: "\r\n"
        * Linux and Mac: "\n"
        * Mac (before OS X): "\r"
    
