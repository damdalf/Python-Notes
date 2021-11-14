# **Python Module 3:**
## **Writing our own functions, value-returning statements, boolean operators, more about the return statement.**

---
To declare and define a function in python use the following syntax:

``` python
def function_name(paremeter_one, paremeter_two):
    print('this is my first function')
    print(paremeter_one + paremeter_two)
    return(parameter_one + parameter_two)

```
If you create the function inside its own script, and want to use it in another script, you have to import it.

```python
from scriptName import functionName
```

To import modules that are not a part of the Python libraries, the script must be in the same folder as the one that imports it.
* import * - imports all of the functions from the script
To import multiple functions from a module simply separate them by commas
* import area, encouraging_words

When you try to use a vlue of a function, meaning it is a local variable, then you will receive the following output: None
    * This happens when you try to use a 'value' of a function that doesn't return a value.
* return
* return None
> Both of thesae achieve the same results.

Functions that return a value are called 'value-returning functions' and functions that reads or writes outside of its own arguments (such as the console) is called a 'functions with side-effects'.

In python, the syntax for boolean oprators is the following:
* or
* and
* not
These can be combined but you must user parentheses as neccessary. 
