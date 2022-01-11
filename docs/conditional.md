# Conditionals

## Need of conditions

Say I am using the quadratic formula to find the square roots of a quadratic equation.

The discriminant `√(b²-4ac)` can be a positive, negative value or can be zero, but you don't want the value to be less than zero so you don't have to go into calculating imaginary and complex roots.

!!! note

    Quadratic Formula is a formula that can be used to find the square roots of any quadratic equation.



So you probably wanna check if the value is greater or equal to zero.

So you may wanna do something like this in pseudocode:

```
If Discriminant < 0{
    print "The value of discriminant is less that 0"
}
```

So that is going to handle the problem for us.

<hr>

## Conditionals in python

Similarly in python we have a way to do this, python `if...elif...else` statement is very common in use however since `python 3.10` a new conditional statement has been added, the `match...case`.

Basic syntax of a `if...elif...else` statement :

=== "if...elif...else"

    ```py
    if <condition-1>:
        #do something
    elif <condition-2>:
        #do something else
    elif <condition-3>:
        #do this instead
    else:
        #don't do all the stuff from before instead do this.
    ```

=== "match...case"

    ```py
    match subject:
        case <pattern-1>:
            #<action-1>
        case <pattern-2>:
            #<action-2>
        case <pattern-3>:
            #<action-3>
        case _:
            #<action-wildcard>
    ```