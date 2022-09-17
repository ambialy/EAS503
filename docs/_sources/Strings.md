# Strings in Python
## *1. What is the meaning of the + and * operators for strings? Give example of each.*
\+ can add strings, but not str and type float or int <br>
\* – to repeat a string<br>
```python
x = 'str' + 'ing'
y = 'Ha' * 3
```
## *2. What does the length of an empty string and how can you determine that?*
the length of an empty string is 0
```python
x = ''
len(x)
```
## *3. How to convert an int and float to string?*
It's simple! just use the str() function.

## *4. What is the different between x and y in x = '3.14' and y = 3.14?*
y is of type float, and x is type string. You can perform mathematical operations with y, and with x you can perform string manipulations such as + and * with other strings.

## *5. What is the value of var3 in the following lines of code?*
```python
var1 = 'Na'
var2 = 3
var3 = var1 + var2
returns TypeError: can only concatenate str (not "int") to str
```

## *6. When using the oldest string method, how can you concatenate a string and a number? Give an example*
```python
PI = 3.14159265359 
name = 'PI'
print('%s is %.2f' % (name, PI)) 
```
## *7. We covered five special characters. What is the purpose of special characters and how do you use them? Give one example of a special character.*
Special characters are characters that envoke a syntax in python but can also be used in strings.
Ex. if you wanted to print 'I won't be "home" for dinner' because (' and ") are special characters you would have to print('I won\\'t be \\"home\\" for dinner)

## *8. We covered the concept of creating string templates. What is a string template and how are they used? Give an example.*
A string template tells python to format a string variable a certain way. In the example below we are telling str_template to accept to values and place a colon after the first.
```python
str_template = '{}: {}'
print(str_template.format(2324, 1))
```
## *9. How are indices used with the newer methods? Give an example*
Indices in f strings are very easy to use, where if you want to swap the order all you have to do is swap the variable call.
```python
f_string = f'The course number is {course_number}. It has {class_size} students.'
f_string = f'The course number is {class_size}. It has {course_number} students.'
```

## *10. String-formatting allows you to do at least five things. These string-format specifiers come after a colon. Explain each of the following using f-string examples.*
### 1. specify width
```python
variable = 'Hey'
f_str = f'This variable has up to ten spaces {variable:10}'
```
### 2. align data to left, right, or center
```python
var = 'Hey'
left = f'{var:<10}'
right = f'{var:>10}'
middle = f'{var:^10}'
```
### 3. specify padding character when specified width is greater than the width of the string/number being used; make sure to explain the default padding character; How can you print 0012300 given x = 123? Where do the padding characters appear with respect to the above two things?
The defaul padding character is a space in python. If you pad a variable with length 3 by 10, there will be 7 spaces to the right by default. The example shows how you can pad with zeros left aligned and middle aligned.
```python
var = 123
left = f'{var:<010}' # padded with zeros to the right
middle = f'{var:^010} # Middle padded with zeros
```
### 4. specify precision for floating values; where is this put in relation to the other string specifiers? How can you print '3.14000000' (10 width) given 'PI = 3.1415'?
Precision for floating values can be specified within an f string.
```python
PI = 3.1415
PI2 = f'{PI:.2f}'
print(f"{PI2:<010}")
```
### 5. add commas to numbers for easier viewing; with respect to the other specifiers, where does this come? How would you print -----123,456.00-----, given x = 123456 - width is 20.

```python
x = 123456
x1 = f'{x:,.2f}'
print(f'{x1:-^20}')
```
## *11. Explain what the .strip() method does?*
.strip() returns a copy of the string with leading and trailing whitespace removed.

## *12. What is the purpose of the in operator for strings?*
You can check is a sequence of characters is in a variable
```python
x = 'Hello'
y = 'Hello World'
x in y is True
```

