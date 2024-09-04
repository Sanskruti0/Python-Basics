# Python Bootcamp

This notebook provides a comprehensive overview of basic and intermediate Python concepts. Let's walk through each section.

## 1. ARITHMETIC OPERATIONS

### Simple Arithmetic

```python
a = 5
b = 6
c = a + b
print(c)
```

### Simple Arithmetic - Get Input from User

```python
a = float(input("Enter the value of a: "))
b = float(input("Enter the value of b: "))
add = a + b
print(add)

a = int(input("Enter the value of a: "))
b = int(input("Enter the value of b: "))
add = a + b
sub = a - b
mult = a * b
div = a / b
mod = a % b
print("ADD:", add)
print("Sum: {0}, Diff: {1}, Mult: {2}, Div: {3}, Mod: {4}".format(add, sub, mult, div, mod)) # Print using Format

print("Sum: %d, Diff: %d, Mult: %d, Div:%15.6f, Mod:%d" % (add, sub, mult, div, mod)) # Print using PADDING & PRECISION

print('{0:<4} | {1:^4} | {2:^4} | {3:>4}'.format('Sum', 'Diff', 'Mult', 'Div'))
print('{0:<4} | {1:^4} | {2:^4} | {3:>4}'.format(add, sub, mult, div))
```

### Simple Arithmetic - Power Operation

```python
a = 2
b = 3
power = a ** b # Power
print(power)
```

## 2. STRINGS

### Create String

```python
a = 'Python'
b = "Bootcamp"
print(a + b)
```

### Length of String

```python
a = "Champ"
print(len(a))

a = "S"
b = a * 5
print(b)
```

### String Index

```python
a = "champ"
print(a[3]) # identifying the element based on index
print(a[2:]) # Grab the remaining elements except up to the Index
print(a[:2]) # Grab the elements up to the Index
print(a[-1]) # Grab the Last element
print(a[:-1]) # Grab the elements except last element
print(a[::2]) # Grab everything with 2 steps
print(a[::-1]) # Print string backwards
```

### String Functions

```python
a = "Master Class"
print(a.upper()) # Changing to Upper case
print(a.lower()) # Changing to Lower case

b = a.split() # Splitting String
print(b)
print(b[1]) # Printing the splitting string based on Index

c = "ElonMusk,SteveJobs,BillGates"
d = c.split(",") # Splitting string based on Delimiter
print(d)
print(d[1])

a = "Master Class"
print(f"Welcome to Python {a}!") # Formatting string Literals
```

## 3. LIST

### Create List

```python
a = [1, 2, 3, 4, 5]
b = ["Champ", 21, 99.5]
print(a, b)
print(len(b)) # Length of List
print(b[0]) # Locate list element based on Index
print(a[1:]) # print elements except 1st
print(a[:2]) # Print elements up to 2nd element
print(a + b) # Concatenate 2 list

a = [1, 2, 3, 4, 5]
a.append(6) # inserting new elements to the existing list
print(a)

a = [1, 2, 3, 4, 5]
a.reverse() # Reverse list
print(a)
print(min(a)) # Minimum
print(max(a)) # Maximum

a = [1, 2, 3, 4, 5]
from random import shuffle
shuffle(a)
print(a)

a = [1, 2, 3]
b = [4, 5, 6]
c = [a, b] # Nested List Matrix
print(c)
print(c[0]) # Printing row
print(c[0][0]) # Printing 1st element
```

## 4. DICTIONARIES

### Creating Dictionary : Key & Value

```python
a = {"Name": "Elon", "Age": 50, "Company": ["SpaceX", "Tesla"]}
print(a)

print(a["Name"]) # Printing value based on its Key
a["Age"] = 51 # Changing values
print(a)

b = {"Climate": {"Condition": {"Temperature": "38 Degree", "Humidity": "70 Percentage"}}}
print(b["Climate"]["Condition"]["Humidity"])

print(a.keys()) # Printing Keys of the Dictionaries
print(a.values()) # Printing Values of the Dictionaries
print(a.items()) # Printing Tuple of the all items
```

## 5. TUPLES

### Creating Tuples

```python
a = ("Champ", 21, 99.5)
print(a)

print(len(a)) # Length of tuple
print(a[0]) # Printing elements from tuple via index
print(a.index("Champ")) # Getting Index of Elements
```

## 6. SETS

### Creating Set

```python
a = set()

a.add("Champ")
print(a)

a.add(30)
print(a)

b = ["Champ", 21, 99.5]
print(set(b))
```

## 7. BOOLEAN

### Creating Boolean

```python
a = True

a = 10
b = 5
c = 15
print(a < b)
print(a > b)
print(a == b)
print(a != b)
print(a <= b)
print(a >= b)
print(a < b and c > a)
print(a < b or c > a)
```

## 8. Python Statements

### If

```python
a = True
if a:
  print("Positive")
else:
  print("negative")

a = 10
b = 6
c = 6

if a < b:
  print("a less than b")
elif c == b:
  print("a is equal to b")
  print("a is not less than b")
  if c < a:
    print("c is less than b")
else:
  print("a is not less than b")
```

### For Loop

```python
a = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
for i in a:
  print(i)

a = [i for i in 'Champ']
print(a)
```

### Odd & Even Number

```python
for i in range(1, 11):
  if i % 2 == 0:
    print(i, "Even Number")
  else:
    print(i, "Odd Number")
```

### String - For Loop

```python
for a in "Hello all":
  print(a)
```

### Dictionary - For Loop

```python
a = {"Name": "Elon", "Age": 50, "Company": ["SpaceX", "Tesla"]}
for k, v in a.items():
  print(k, ":", v)
  
```

### While Loop

```python
a = 0
while a < 11:
  print(a)
  a += 1 # a = a + 1
```

### While Loop - Break & Continue

```python
a = 0
while a < 10:
  print(a)
  a += 1
  if a == 5:
    print("a is equal to 5")
    break
  else:
    print("Continueeee")
    continue
```

### Emulating Do-While in python

```python
while True:
    a = int(input("Enter a number greater than 10: "))

    if a > 10:
        break

    print("Try again!")
```

### Range

```python
for a in range(6):
  print(a)

for a in range(1, 10, 1):
  print(a)

for a in range(10, 0, -3):
  print(a)

a = [i ** 2 for i in range(0, 5)]
print(a)

a = [i for i in range(10) if i % 2 == 0]
print(a)
```

### Enumerate - To track no. of iteration in the loop, without working with variable increment

```python
for i, a in enumerate("Hello Champ"):
  print(i, a)
```

### Zip - Creating tuples by zipping 2 lists

```python
a = ["Name", "Age", "Country"]
b = ["Champ", 27, "India"]
print(list(zip(a, b)))
```

## 9. Functions

### Initializing & Calling basic function

```python
def welcome():
  print("Hello guyz Welcome to Python Bootcamp !!!")

welcome()
```

### Initializing & Calling basic function - With Argument

```python
def welcome(a):
  print("Hello {0}, Welcome to Python Bootcamp !!!".format(a))

welcome("Champ")
```

### Print & Return

```python
def add(a, b):
  add = a + b
  print("Sum of {0} and {1} is {2}".format(a, b, add))

def addR(a, b):
  add = a + b
  return add

ans = addR(45, 5)
final

 = ans + 10
print(final)
```

### Function to check whether no is even/odd

```python
def oddEven(a):
  if a % 2 == 0:
    print("{0} is Even".format(a))
  else:
    print("{0} is Odd".format(a))

oddEven(45)
oddEven(50)
```

### Positional Arguments

```python
def sample(a, b, c):
  return a ** b * c

print(sample(2, 4, 6))
print(sample(4, 2, 6))
print(sample(6, 2, 4))
```

### Default Arguments

```python
def sample(a, b, c = 2):
  return a ** b * c

print(sample(2, 4, 6))
print(sample(2, 4))
```

### Variable Length Arguments

```python
def sample(*a):
  print(a)

sample(1, 2, 3, 4)
```

### Function to check whether no is even/odd & to identify the element within list - Using Variable Length Arguments

```python
def sample(*a):
  for i in a:
    if i % 2 == 0:
      print("{0} is Even".format(i))
    else:
      print("{0} is Odd".format(i))

sample(45, 2, 32, 51, 49)
```

## 10. LAMBDA EXPRESSIONS

### Basic

```python
def add(a, b):
  return a + b

addL = lambda a, b : a + b
print(addL(50, 5))
```

### Map & Filter

```python
def oddEven(a):
  if a % 2 == 0:
    print("{0} is Even".format(a))
  else:
    print("{0} is Odd".format(a))

sample = [2, 4, 7, 5, 3, 9, 11]
a = list(map(oddEven, sample))
print(a)

sample = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
def sqr(a):
  return a ** 2

print(list(map(sqr, sample)))
print(list(map(lambda a : a ** 2, sample)))

sample = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
print(list(filter(lambda a : a % 2 == 0, sample)))
```

### Nested List Comprehension

```python
sample = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
print(list(map(lambda a : a ** 2, filter(lambda a : a % 2 == 0, sample))))

sample = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
print([a ** 2 for a in sample if a % 2 == 0])
```

### Global Variable

```python
def sample():
  global a
  a = 15

sample()
print(a)
```

## 11. FILE HANDLING

### Creating, Opening, Reading, Writing, Closing

```python
sample = open("sample.txt", "w+")
sample.write("Welcome to File Handling")
sample.close()

sample = open("sample.txt", "a+")
sample.write("\nHello Python")
sample.close()

sample = open("sample.txt", "r")
print(sample.read())

sample = open("sample.txt", "r")
print(sample.readlines())

sample = open("sample.txt", "r")
print(sample.readline())
```

## 12. EXCEPTION HANDLING

### Basic

```python
try:
  sample = open("sample.txt", "w")
  sample.write("Hello Python")
except IOError:
  print("File cannot be created")
else:
  print("Success")
finally:
  sample.close()
  print("Closed")
```

### Divisible by 0 - Exception Handling

```python
try:
  a = 10
  b = 0
  c = a / b
except:
  print("Divide by 0 Exception Error")
finally:
  print("Inside Finally block")
```

## 13. MODULES

### Basic - Importing Modules

```python
import sample

sample.add(4, 5)
sample.sqr(4)
```

### Importing Module - With Alias Name

```python
import sample as s

s.add(4, 5)
s.sqr(4)
```

### Importing Particular Function from Module

```python
from sample import add

add(4, 5)
```

### Importing Particular Function from Module - With Alias Name

```python
from sample import add as a

a(4, 5)
```

### Python in-built functions from module

```python
import math

print(math.sqrt(64))

import math as m

print(m.sqrt(49))

from math import sqrt

print(sqrt(36))

from math import sqrt as s

print(s(25))
```

## 14. CLASS

### Creating Class

```python
class sample:
  def __init__(self, a, b, c):
    self.fname = a
    self.lname = b
    self.salary = c

  def display(self):
    print("Name is {0} {1}, Salary: {2}".format(self.fname, self.lname, self.salary))

s = sample("Champ", "Gupta", 50000)
print(s.fname)
print(s.lname)
print(s.salary)
s.display()
```

### Creating Class - Using In-built Function - “getattr”, “setattr”, “delattr” & “hasattr”

```python
class sample:
  def __init__(self, a, b, c):
    self.fname = a
    self.lname = b
    self.salary = c

  def display(self):
    print("Name is {0} {1}, Salary: {2}".format(self.fname, self.lname, self.salary))

s = sample("Champ", "Gupta", 50000)
print(getattr(s, "fname"))
print(hasattr(s, "lname"))
setattr(s, "salary", 60000)
print(getattr(s, "salary"))
delattr(s, "fname")
print(getattr(s, "fname"))
```

### Inheritance

```python
class sample:
  def __init__(self):
    print("Welcome to Base Class")

  def baseClass(self):
    print("Method Belongs to Base Class")

class derived(sample):
  def __init__(self):
    sample.__init__(self)
    print("Welcome to Derived Class")

  def derivedClass(self):
    print("Method Belongs to Derived Class")

s = derived()
s.baseClass()
s.derivedClass()
```

## 15. REGEX

### Search within String

```python
import re

a = "Python Bootcamp"
b = re.search("Python", a)
print(b.start())

a = "Python Bootcamp"
b = re.findall("Python", a)
print(b)

a = "Python Bootcamp"
b = re.split(" ", a)
print(b)

a = "Python Bootcamp"
b = re.sub("Python", "Java", a)
print(b)

a = "Python Bootcamp"
b = re.match("Python", a)
print(b.group())
```

## 16. DATE TIME

### Current Date Time

```python
import datetime

a = datetime.datetime.now()
print(a)
print(a.year)
print(a.strftime("%A"))
print(a.strftime("%B"))

a = datetime.datetime(2021, 8, 15)
print(a)
print(a.strftime("%B"))
print(a.strftime("%A"))

a = datetime.datetime.now()
print(a.strftime("%c"))
print(a.strftime("%x"))
print(a.strftime("%X"))

print(a.strftime("%I"))
print(a.strftime("%H"))

print(a.strftime("%p"))
print(a.strftime("%P"))
```
