## Python Worksheets

Written because Danny is an *idiot*

### Worksheet #4
1. What is the difference between `=` and `==`<br>
  (**a**) `=`: The *set* operator, registered as `__eq__` in `python`, <br>
  it sets a variable equal to a value. For example, `a = 4 + 5` <br>
  (**b**) `==`: The Logical Comparison Operator, returns a boolean<br>
  For Example, `a = True if 4 == 5 else False`, `a` will then equal `False`<br>

2. Explain how x=x+1 can happen in programming:<br>
~~~py
# This:
x = x + 1

# Is the Same As:
x += 1

# Which Means set x equal to one plus itself
# SO:
A = 4
# A is now equal to 4
A += 1
# A is now equal to 4 + 1, or 5
~~~

3. What is the return type of a user input?<br>
~~~py
# The Return Type is going to be a string.
# We Can verify By Doing This:
print(help(input))
# Which States:
# Read a string from standard input.  The trailing newline is stripped.
# The keyword is "string"
~~~

4. Can you change the data type from an input?<br>
~~~py
# Yes, we can use Python's implementation of casting to do such.
# Here are some examples
INPUT = input("Enter a Number")
parsed_float = float(INPUT)
parsed_int = int(INPUT)
# This would come in handy if you needed the user to enter a number,
# and then were to use it in calculations.
~~~

### Python Exercises
1. Temperature Question:<br>
~~~py
DATA = {k:float(input(f"Enter the {k} temperature: ")) for k in ["first", "second", "third"]}
averageTemp = sum(list(DATA.values())) / 3
print(f"Average Temperature: {averageTemp}")
~~~
Or the Expanded Version:<br>
~~~py
temp1 = input("Enter the first temperature")
temp2 = input("Enter the second temperature")
temp3 = input("Enter the third temperature")

temp1 = float(temp1)
temp2 = float(temp2)
temp3 = float(temp3)

averageTemp = (temp1 + temp2 + temp3) / 3

print("Average Temperature:", averageTemp)
~~~









