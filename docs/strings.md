# Strings

Strings in python are a very essential datatype and other programming languages too, its a sequence of characters in python.

<hr>

## Single-line and Multi-line strings

### Single-line strings

```py
string = "Hello World" #this is an example of a string, it uses ""

another_string = 'Hi World' #this is another example of a string, using ''
```

### Multiline-line strings

```py
First_multiline_string = """Hello World \n
How are you doing
""" # \n is a special character ( escape sequence character ).

Second_multiline_string = '''Hi World \n
How are you doing
'''
```
<hr>

## Using `type()` function on a string

```py
>>> type(string)
<class 'str'>
>>> type(another_string)
<class 'str'>
>>> type(First_multiline_string)
<class 'str'>
>>> type(Second_multiline_string)
<class 'str'>
```

<hr>

## Finding length of a string

We can use the `len` function to find the length of a string.

```py
>>> len(string)
11
>>> len(another_string)
8
>>> len(First_multiline_string)
32
>>> len(Second_multiline_string)
29
```

<hr>

## String Indexing and String Slicing

### String Indexing
```py
>>> text = "Hello"
>>> text[0] #this is going to get the first character of the string
'H'
>>> text[1] #this is going to get the second character of the string
'e'
>>> text[4] #this is going to get the fifth character of the string
'o'
>>> text[-1] #this is going to get the last character of the string
'o'
>>> text[-5] #this is going to get the fifth character of the string from the first
'H'
```

|0 and Positive indexing :| 0  | 1 | 2 | 3 | 4 |
|-------------------------|----|---|---|---|---|
|          Word :         | H  | e | l | l | o |    
|    Negative Indexing :  | -5 | -4| -3| -2| -1|

String Indexing starts from `0` and goes upto `(length of string - 1)`.

Negative indexing starts from `-(length of string)` upto `-1`

Lets see another example : 

```py
>>> "Python is a very popular language"[0]
'P'
>>> "Python was created by Guido Van Rossum"[-1]
'm'
>>> "Python has a very easy syntax"[13]
'v'
```
<hr>

