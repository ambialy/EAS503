# Functions in Python
## *1. Why do you need functions? What are the advantages of using a function? Give an example of a function?*

### What is a function?
A function is a small self-contained sequence of statements/instructions that has a name.<br>

### Why do we need functions?
Functions make our code cleaner and allow us to reduce repetative code

### What are the advantages of functions?
- Many programs require a particular sequence of statements/instructions to be executed repeatedly. The repeated statements/instructions can be placed with a single function, which can be accessed whenever needed. Therefore, they reduce repeated statements/instructions.
- Functions help decompose larger programs into logical subprograms. Such programs are easier to write and debug.
- Functions can be executed at any point by using their name
- Functions can call other functions
- Functions can OPTIONALLY take argument(s) that they can use inside the function
- Functions can OPTIONALLY return value(s)

```python
def add_two_numbers(a,b):
    return a + b
add_two_numbers(2,3)
```

## *2. How can functions make repeated lines of code more general?*
Let's say we want to find the value of a number to the power of a number
```python
two_pow_4 = 2 ** 4
```
Now, we can use the pow() function to do this without having to perform the math ourselves
```python
two_pow_4 = pow(2,4)
```

```{note}
pow() is a built-in function. Explained later
```
## *3. What are input arguments to a function? What is the purpose of the return keyword? Explain the four possible combinations of input arguments and outputs values of a function and give one example for each*

### What are input arguments
Input arguments are the values passed into function to be evaluted on.
```python
pow(2,4)
```
The input arguments are 2 and 4

### What is the purpose of the return keyword
Return tells the function to send back a value to when the function is called

### Explain the four possible combinations of input arguments and outputs values of a function and give one example for each
- No input; no output; example – print something
  ```python
  def hello_world():
    print('Hello World')
  ```
- One or more input; no output; example – print the input
  ```python
  def print_input(input):
    print(input)
  ```
- One or more input: one or more output; example – take two numbers and return their sum
  ```python
  def multiply(a,b):
    return a * b
  ```
- No input; one or more output; example – a random number
  ```python
  def rando():
    import random
    return random.randint(1,100)
  ```

## *4. What are built-in functions? Give two examples.*
Built-in functions are functions that come with the default install of python.
```python
pow(2,4)
sum(10,20)
```

## *5. What is a local variable and how does it relate to a function? Use some example code to illustrate the concept of a local variable.*
A local variable is a variable that exists only within the scope of a function
```python
x = 10
print(x)
def sun(x):
  print(x)
sun('Zebra')
```

## *6. What is the default return value of a function? When is the default return value returned?*
The default return value is `None`. The default return value is returned when no return value is specified in the function.