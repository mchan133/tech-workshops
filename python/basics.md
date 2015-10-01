
# Rutgers IEEE Student Branch - Python Basics Workshop

## Workshop Leaders

Ravi Bhankharia, Niral Shah

## Module 0 - What is Python?

Cover what python is, what it's used for (interpreted, dynamically typed scripting language etc)

Python is a powerful, popular, general-purpose programming language.

Some important facts about python:

* **Python is dynamically typed.** This means that a variable can be an int, string, double, etc., without being declared as such.
* **Python is white-space delimited.** This means that there are no `{ curly brackets }` surrounding blocks of code, rather blocks are indicated by their indentation level (we will show examples of this later).
* **Python is an interpreted scripting language.** This means that Python should run identically on different operating systems, you don't compile Python programs, and additionally that Python scripts can help automate tasks.

## Module 1 - Basic Syntax

### A. Input/Output

Cover how to run a python program, how to print Hello World, how to use raw_input/prompt, how to make a variable

Here's an example of a simple Python Hello World program:

```python
# Hello World Program!
# <- Octothorpes indicate comments.

a_variable = "Hello World!"
print(a_variable)
```

Notice here that there is no set type for `a_variable`. We could have put `a_variable = 42` at the end and Python would be totally okay with that. And while this allows for flexibility, it can also lead to hard-to-detect errors. So be careful!

To take user input, another relatively common task, use the `input("some prompt")` function. Here's another example:

```python
# An example of input.

user_name = input("What is your name? ")
user_age = input("What is your age? ")

print("So you are " + user_name + " and you are " + str(user_age) + " years old.")
print("Nice to meet ya!")
```

Notice how the input function was used. Also, notice the `str(user_age)`. This is done because `print` can only put together strings, and age is (most likely) an `int`! Don't beleive me? Try putting in a number for your name.


### B. Loops and Conditionals

Cover if statements, while loops, for loops

An important feature of any language is loops and if/else logic! So to explain how to use them, here's an example:

```python
# Loops, and if/elif/else

print("Here's a question for you: ")
guess = input("How many lines would it take to write this program in Java? ")

while(str(guess.strip().lower()) != "too many"):
  print("Not quite...")
  guess = input("Try again! ")
print("You got it!")
```

Some important things to notice here are the colon after the while loop condition, and the indented lines following. The indentations represent the statements within the while loop block, and this helps force more readable code. And though tabs are preferable, any amount of whitespace will do, even a single space (though that would make your code much more difficult to read).

### C. Lists/Arrays and Dicts

Show how to make a list and a dict (and what they are)

### D. Functions

Show how to make a function using def

## Module - References

http://www.astro.ufl.edu/~warner/prog/python.html

https://en.wikipedia.org/wiki/Python_%28programming_language%29
