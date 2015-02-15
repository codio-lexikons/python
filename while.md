# While loop
A while loop statement repeatedly executes a target statement as long as a given condition is true.

```python
count = 0
while (count < 9):
   print ('The count is:', count)
   count = count + 1

print ("Good bye!")
```

produces

```
The count is: 0
The count is: 1
The count is: 2
The count is: 3
The count is: 4
The count is: 5
The count is: 6
The count is: 7
The count is: 8
Good bye!
```



## The break statement
The `break` statement terminates the current loop and resumes execution at the next statement after the loop.

The most common use for `break` is when some external condition is triggered requiring a hasty exit from a loop. The break statement can be used in both `while` and `for` loops.

If you are using nested loops (i.e., one loop inside another loop), the break statement will stop the execution of the innermost loop and start executing the next line of code after the block.

```python
var = 10 
while var > 0:              
   print ('Current variable value :', var)
   var = var -1
   if var == 5:
      break

print ("Good bye!")
```

## The continue statement
The `continue` statement returns the control to the beginning of the `while` loop. The continue statement rejects all the remaining statements in the current iteration of the loop and moves the control back to the top of the loop.

The continue statement can be used in both while and for loops.

```python
var = 10 
while var > 0:              
   var = var -1
   if var == 5:
      continue
   print ('Current variable value :', var)
print ("Good bye!")
```

The above example will **not** print out the number 5.

## The else statement
The `else` statement can be used by both `for` and `while` loops and executes once the loop has completed unless the loop is exited using a `break` statement.

```python
for x in range(2, n):
    if n % x == 0:
        print(n, 'equals', x, '*', n//x)
        break
else:
    # loop fell through without finding a factor
    print(n, 'is a prime number')
```

Note that the `else` statement belongs to the loop, not the `if` statement.

##Beware Infinite loops
You must use caution when using while loops because of the possibility that this condition never resolves to a false value. A loop becomes infinite loop if a condition never becomes false.  This results in a loop that never ends.

An infinite loop might be useful in client/server programming where the server needs to run continuously so that client programs can communicate with it as and when required.

```python
var = 1
while var == 1 :  # This constructs an infinite loop
   num = raw_input("Enter a number  :")
   print ("You entered: ", num)

print "Good bye!"
```

When the above code is executed, it produces the following result:

```
Enter a number  :20
You entered:  20
Enter a number  :29
You entered:  29
Enter a number  :3
You entered:  3
Enter a number between :Traceback (most recent call last):
  File "test.py", line 5, in <module>
    num = raw_input("Enter a number :")
KeyboardInterrupt
```
