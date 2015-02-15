#If Statements and Control Flow

```python
x = int(input("Please enter an integer: "))
if x < 0:
    x = 0
    print('Negative changed to zero')
elif x == 0:
    print('Zero')
elif x == 1:
    print('Single')
else:
    print('More')
```

There can be zero or more `elif` parts, and the `else` part is optional. The keyword `elif` is short for ‘else if’, and is useful to avoid excessive indentation. An `if ... elif ... elif` sequence is a substitute for the switch or case statements found in other languages.

##Nested if statements
```python
var = 100
if var < 200:
   print ("Expression value is less than 200")
   if var == 150:
      print ("Which is 150")
   elif var == 100:
      print ("Which is 100")
   elif var == 50:
      print ("Which is 50")
elif var < 50:
   print ("Expression value is less than 50")
else:
   print ("Could not find true expression")

print ("Good bye!")
```

##Boolean logic

``` python
var = 100
if var:
   # This will print as 'var' is non-zero and 
   # `if var:` is simply another way of saying 'if var<>=0'
   print ("Here I am")
```
