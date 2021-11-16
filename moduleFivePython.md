# **Python Module 5**
## **Strings, Brackets, Lists, String Operations, For-Loops, and Number Ranges**
***

### **Strings, Brackets, Lists**
* characters of Strings can be accessed using bracket notation, treating the String like an array of chars.
* len() is extremely useful when doing this
    * avoid 'IndexError'
* s[-1] is shorthand for s[len(s) - 1]
    * Ex) s[-1 * len(s)] == s[0]
* to take a substring, set your starting index and ending index inside of the brackets using a colon.
    * first = name[0:5]
* name[0: ] - means all characters up to end of the String (abbreviates name[0 : len(name) - 1])
* name [ :5] - mean all characters up to index 5 of the String
* In Python Strings are immutable, that means once they are created they cannot be modified
    * Ex) 
```python
word1 = "see"
# the code below will not work
word1[0] = "b"
# you must create a new String
word2 = "b" + word1[1: ]
```
* to create a list in Python, simply create a variable and assign it to a list of items separated by commas inside of brackets.
    * Ex)
```python
my_list = [7, 2, 5, 32, 69, 420]
ducks = ["Louie", "Huey", "Donald"]
```
* printing a list will print all of the items in the list in the above format.
* lists are accessed the exact same way as Strings, including the shorthand indices using the ':'
***

### **String Operations**
* String.upper() - converts all lowercase letters to uppercase letters, but the starting String is not modified.
    * remember, Strings are immutable so we must do something like this:
        * new_str = str.upper()
* len(String) - returns the length of the String
    * includes white spaces and symbols (any characters)
* String.lower() - converts all uppercase letters to lowercase letters, but the starting String is not modified.
* String.capitalize() - converts the first letter in the String to uppercase and the rest to lowercase, but the starting String is not modified.
* String.strip() - returns a new String where all whitespaces are removed from the beginning and end of the String, except for those that appear directly before a String.
    * the starting String is not modified.
    * tabs, newlines, spaces
* String.find(char) - returns the index of the first ooccurence of the specified char.
    * if the char is not found, the method returns -1.
* String.startswith() - returns True if the targeted String's first character (or sequence of characters) is the specified character (or sequence of characters), and returns False otherwise.
    * capitalization matters
* String.endswith() - returns True if the targeted String's first character (or sequence of characters) is the specified character (or sequence of characters), and returns False otherwise.
    * capitalization matters
* String.split() - returns a list containing the individual words of the String.
* In Python, you can chain these functions together:
    * if status.strip().lower().startswith("y"):
* These functions that use 'dot notation. are called methods.
* Format Strings
    * format specifiers - 'placeholders' in the output.
        * %s - placeholder for a String
        * %d - placeholder for an int
        * %f placeholder for a float
        * Ex)
```python
fmt = "My name is %s and I ate %d pies."
result = fmt % ("Steve", 42)
print(result)
# produces "My name is Steve and I ate 42 pies."
# if there is only one specifier, the commas are optional.
```
* formatting width
    * %6.2f - prints the float with six spaces before it, and only two decimal places
    * %10d - prints the int with 10 spcaes before it.
    * to add spaces behind the item, place a '-' in front of the width specifier
        * %-10d
    * if you place a 0 in front of the width specifier, all extra spaces will be filled with zeros (spaces not already taken up by a whitespace).
***

### **For-Loops and Number Ranges**
```python
values = [2, 4, 6, 8, 10]
for v in values:
    print(v)
# prints all values in the sequence
```

* can also iterate through a String using the String as the sequence
* range(begin, end) - creates a sequence or list from begin - end - 1.
    * begin - your starting index
    * end - the length of the array
    * range(beging, enter, step) - creates a sequence from begin - end - 1 while incrementing by the step value.
    * range(begin, end, -1) - counts down from the starting value to the ending + 1 value by decrementing by 1 each time.