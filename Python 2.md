```python
print 'shanioob' + 5/2	#will produce an error
#TypeError: unsupported operand type(s) for /: 'str' and 'int'
print 'shanioob' * 5/2	#will produce an error
print 'shanioob' * (5/2)	#will produce 'shanioobshanioob'
print          5/2.0
```
## Strings
```python
the_king = "the king"
assert the_king[0] == 't'
assert the_king[0] + the_king[1] == "th"
assert the_king[0:2] == "th"
assert the_king[1:] == "he king"
assert the_king[:2] == "th"
assert the_king[:-1] == "the kin"

the_king.find('king')
the_king.find('king',3)
the_king.replace('king', 'queen', 1)
assert the_king.split() == ["the", "king"]
```

```python
assert type(shanioob_the_king) == "<class ‘string’>"
dir()
dir('__builtins__')
help('modules')
```

## String Templates
```python
"{}- I am the number {} programmer".format(1,1)
```
## Coercion
```python
assert bool(28) == True
assert str(True) == 'True'
assert int(False) == 0
```
## functions
```python
def say_hello(name):
	return 'Hello ' + str(name) + '!' 
	
print say_hello('Susan')

five, seven = 5, 7
fiveSeven = [five, seven]

def sum(a, b):
    a = a + b
sum(five, seven)	#five still == 5

def summer(list):
	list[0] = list[0] + list[1]
summer(fiveSeven)	#fiveSeven == [12, 7]
```

### Function's Default Arguments
```python
def cm(feet = 0, inches = 0):
	inches_to_cm = inches * 2.54
	feet_to_cm = feet * 12 * 2.54
	return inches_to_cm + feet_to_cm

cm(inches = 70)
```

## if Statement & Ternary Operator
```python
def bigger(a, b):
	if a > b:
		return a
	elif b > a:
		return b
	else:
		return a

def bigger(a, b):
    return a if a > b else b
```
## Logic Operators
```python
True or False
True and False
not True and not False
not True != None
```
## While Loops
```python
while True:
	sum += 1	#the ++ syntax is not supported
```

## For Loops
```python
for num in range(10):
	#do that 10 times
```

## Lists
```python
list = [1,2,3,[4,5]]
assert list[1] == 2
assert list[:2] == [1,2]
assert list[:3] + list[3] == [1,2,3,4,5]

list = list + [6, 7]	#will create a new array
list.append(6)			#will mutate the actual array
list += [6, 7]			#will mutate the actual array

assert list[:2] * 2 == [ 1, 2, 1, 2 ]

assert len(list) == 4
assert len("My list") == 7

list.index(6)	#return index or error
6 in list 	#return True or False
not 6 in list == 6 not in list

" ".join(list)
```
## Tuples
```python
tuple = (1,2,3)
(one, two, three) = tuple

one, two, three = 1, 2, 3	#valid syntax
```

## Assertion & Error Handling
```python
try:
	assert isDefined(arg1)
except AssertionError:
	print "AssertionError raised"
```

## User Input
```python
user_input = raw_input("Type your input: ")
```
## Used Import Statement
```python
from random import randint
random = randint(0,1)

import random
random = random.randint(0,1)

import webbrowser
webbrowser.open("https://www.google.com")

import time
time.sleep(60)		#time is seconds
this_time = time.ctime()

import os
os.listdir(r"c:\OOP\prank")
os.rename(src, dst)
os.getcwd()
os.chdir(path)

string.translate(s, table[, deletechars])
string.translate(None, "0123456789")
```

### turtle class
```python
import turtle

window = turtle.Screen()
window.bgcolor("red" or 255,255,255 or "#rrggbb")

my_turtle = turtle.Turtle() 
	or turtle.Pen()

my_turtle.forward(distance) 
	or fd(distance)
my_turtle.backward(distance) 
	or bk(distance) 
	or back(distance)
my_turtle.right(degrees) 
	or rt(degrees)
my_turtle.left(degrees) 
	or lt(degrees)
my_turtle.circle(radius, extent=None, steps=None)

my_turtle.speed(0..10)	#0 is fastest (no animation), then speed drops from 10 to 1
my_turtle.shape("arrow" or "turtle" or "circle" or "square" or "triangle" or "classic" or "blank")
my_turtle.shapesize(stretch_wid=None, stretch_len=None, outline=None) 
	or my_turtle.turtlesize()
my_turtle.pensize(lines) 
	or width(lines)

my_turtle.color(color)
my_turtle.pencolor(color)
my_turtle.fillcolor(color)

#turn off tracer
my_turtle.tracer(0, 0)
#because tracer is off
my_turtle.update()

#only exit onclick
window.exitonclick()
```

## File Manipulation - Built-in Functions
```python
myFile = open("path")	#open() returns a file object
content = myFile.read()
myFile.close()

import urllib
connection = urllib.urlopen("http://www.wdyl.com/profanity?q="+text)
output = connection.read()
print(output)
connection.close()
```

## Class Definition
```python
class Parent():
	"""This String will be accessable using the __doc__ variable"""
   money = "under zero"
   state = "exausted"
   
   def __init__(self, last_name, eye_color):
      self.last_name = last_name
      self.eye_color = eye_color

   def show_info(self):
      print("Last Name - " + self.last_name)
      print("Eye Color - " + self.eye_color)


class Child(Parent):
   state = "lively"
   
   def __init__(self, last_name, eye_color, number_of_toys):
      Parent.__init__(self, last_name, eye_color)
      self.number_of_toys = number_of_toys

   def show_info(self):
      Parent.show_info(self)
      print("Number of Toys - " + str(self.number_of_toys))
      print("State - " + self.state)

gabgoob = Child("Ben Shanioob", "Honey", 3)
print gabgoob.money
gabgoob.show_info()

Parent.__doc__		#The class documentation string.
Parent.__module__	#The name of the module in which this class was defined.
Parent.__name__		#The name of the class.
Child.__bases__	#The classes from which this class inherits.
```
