# Data Handling

## Truth Values

Truth values are basically logical values of some data.

It can have either of two values : `True` / `False`

In python, except : `False`, `""`, `''`, `''''''`, `""""""`, `None`, `0`, `{}`, `[]` and `()` have a truth value as `False`.

Truth Value of some data can be found out using `bool(x)`, where `x` is some data.

Lets test it out :

```py
>>> bool("Hello")
True
>>> bool(0)
False
>>> bool(None)
False
>>> bool(1)
True
>>> bool(3.56)
True
>>> bool([1,50,97])
True
>>> bool({})
False
```
<hr>

## Logical Operators

As discussed earlier the logical operators in python are : `and`, `or`, `not`.

### `not` Operator 
is the inverse operator it will invert every result (True becomes False and False Becomes True).

```py
>>> not True
False
>>> not False
True
```

### `or` Operator 

Is an operator which returns `True` if either of the conditions specified is `True`.
If both conditions specified are `False` then it returns `False`.


```py
>>> 5 > 3 or 2 < 1
True
>>> 10 > 20 or 11 > 200
False
>>> 1 < 2 or 2 < 3 #it will return True even if both conditions specified are True
True
```

### `and` operator 
Returns `True` only if both conditions are `True` otherwise it will return `False`.

```py
>>> 5 > 3 and 2 < 1
False
>>> 200 < 1 and 2 > 1
False
>>> 1 == 1 and 500 != 21
True
>>> 23 < 25 and 5 > 1
True
```

### Some Errors which do not show up

These errors would show up when used individually but they are not read by python because :

(i) the `or` operator only reads the second condition if the first condition is `True`

```py
3 > 2 or a > b #a and b are not defined yet we are comparing them
True
>>> #no errors
```

(ii) the `and` operator only reads the second condition if the second condition is `False`

```py
>>> 3 < 2 and a != b
False
>>> #no errors yet again
```

Lets confirm  that they do give errors if used individually:

```py
>>> a > b
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
NameError: name 'a' is not defined
>>> a != b
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
NameError: name 'a' is not defined
```