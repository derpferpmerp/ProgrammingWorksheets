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

2. Name Parser:<br>

```py
NAME = input("What is your Name? : ")
print(f"Hello, {NAME[1:-1]}. Have a nice day!")
```

### Worksheet #5
1) b, Processing <br>
2) c <br>
3) <br>

```py
# In Python, a conditional statement is structured as such:
if ( SOME_BOOLEAN ):
  DO_SOMETHING()
# As stated, the condition inside of the "if" statement is SOME_BOOLEAN,
# Which clearly would have the type "bool". A boolean can hold 2 values,
# True, or False. Thus we are checking the truth value of the Boolean.
```
4) c
5) b and c

### Python Exercises
1. William Shakespeare:<br>

```py
name = input("What is your name? : ")

if name == "William Shakespeare": print("William, would you write me a sonnet?")
print("Have a nice day.")
```

2. Age Detector<br>

```py
def parseAge(age):
    if age <= 16:
        print("Be Patient.")
    elif age == 17:
        print(
            "Drive Safely.",
            "A person may purchase cigarettes and be drafted into the military at 18.",
            sep="\n"
        )
    elif age == 18:
        print(
            "Smoking is bad for your health,",
            "But don\'t forget to register for the draft",
            "A Person may consume alcohol at 21.",
            sep="\n"
        )
    elif age == 21:
        print(
            "Please Drink Responsibly.",
            "A Person Typically Retires at 65.",
            sep="\n"
        )
    elif age >= 22 and age <= 64:
        print("Just Living Life")
    elif age > 65:
        print("Enjoy Retirement")
        
AGE = input("How Old are you? : ")
AGE = int(AGE)
parseAge(AGE)
```

3. Weather Modulus<br>

```py
temp = input("Enter current temperature:")
temp = int(temp)
if temp < 0: print("I have icicles in my nose.")
elif temp >= 0 and temp <= 32: print("It\'s an icy cold day.")
elif temp >= 33 and temp <= 60: print("Bundle up, it\'s cold outside.")
elif temp >= 61 and temp <= 75: print("Spring is in the air!")
elif temp >= 76 and temp <= 95: print("Let\'s go to the beach!")
elif temp > 96: print("Stay in the AC today.")
```







