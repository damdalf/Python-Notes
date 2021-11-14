## **MODULE 2:** Variables, Expressions, and Statements
***
* In python, you cannot concatenate non-string variables with strings using '+' like you can in Java, you must use commas (similar to C).
    * When using a comma to include a non-string variable in a print statement or concatenation, there is no need to leave a space - one is automatically created between the two items. , = " "
    * How to add non-string variables into strings without unwatned spaces then?
        * Simply use the built-in converter method 'str(var)' and concatenate the two string using the '+' operator... pretty much just cast the variable to a str.
            - int()
            - strr()
            - float()
* However, strings can be concatenated with other strings using '+'.
* There is a built-in input function that makes getting input from the user extremely easy. 
    * However, this function always returns a string, even if an integer value was entered. Thus, it is important to convert any input from the user if needed.
```python
name = input("Please enter your name: ")
```
* What is a function's syntax in Python?
    * Generally, a functions statements or body expressions should be indented by four spaces.
```python
def <NAME>( <PARAMETERS> ):
    <STATEMENTS>
```
* What is the syntax for boolean?
    * bool
* How do you write if-else statements in Python?
```python
if score >= 65:
    print("You are passing.")
else:
    print(score, "is below 65.")
    print("Better study some more!")
print("Bye.")
```
* Or
```python
if score >= 65:
    print("You are passing.")
elif score < 65 && score != 0:
    print(score, "is below 65.")
    print("Better study some more!")
else:
    print("Dude...")
print("Bye.")
```

### **Common Built-In Functions**
![](https://i.gyazo.com/bebd33360715e58131d3ab8805363ff0.png)

![](https://i.gyazo.com/0f5be99a83273ae24aeb9d0189f2475f.png)