#For loops

The **for** statement iterates over the items of any sequence (a list or a string), in the order that they appear in the sequence.

###Fixed iterations
```python
for i in range(5):
  print(i)
```

Prints numbers from 0 to 4

```python
for i in range(5, 10):
  print(i)
```

Prints numbers from 5 to 9

```python
for i in range(0, 10, 3)
  print(i)
```

Prints the numbers 0, 3, 6, 9. 

- Parameter 1 is the start of the range
- Parameter 2 is the end of the range
- Parameter 3 is the number to increment by at the end of each loop

###Lists

```python
words = ['cat', 'window', 'defenestrate']
for w in words:
    print(w, len(w))
```
Prints
```
cat 3
window 6
defenestrate 12
```

###Strings
```python
string='hello'
for w in string:
    print(w)
```
Prints
```
h
e
l
l
o
```

###break
Exits the enclosing loop. The following example searches for prime numbers.

```python
for n in range(2, 10):
    for x in range(2, n):
        if n % x == 0:
            print(n, 'equals', x, '*', n//x)
            break
    else:
        # loop fell through without finding a factor
        print(n, 'is a prime number')
```
###else for loops
Look at the `else` statement in the above example. It belongs to the loop, not to the `if` statement. Its contents executes once the loop is complete. If a `break` statement is encountered, the `else` statement is not executed. 

###continue
Continues with the next iteration of the loop.




