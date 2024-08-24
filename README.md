# This Repository gives you complete python programing usecase and its solutions

## Python
---------
name = input('What is your name? ')
print ("Hi, "+name )

colour = input('What is fav colour? ')
print(name + " likes " + colour)

birth_year = input('Birth Year ')
print(birth_year)

age = 2019 - int(birth_year)
print(age)

Conver lb in kilogram
weight = input('Enter your weight in lbs: ')

kilogram = int(weight) * 0.45
print(kilogram)

name = "Learning in progress"
print(name[1:-1])

Output:
earning in progres
|--------------------------------|
|Define multiple lines like email|
|--------------------------------|

name = '''   (Enter 3 singe Quote to enter multiple line
Hi Good Day!

Welocm on board

Regards
'''
print(name)

output
------|
Hi Good Day!

Welocm on board

Regards

String
******



|---------------|
|Index of string|
|---------------|
name = 'Hi Good Day'
        0123456  #Index   
print(name[0]) 	# print (name[1:4]) will return first to 3rd character, # print (name[-2]) will return character from last
output- H
output- i g

|---------------|
|Formated string|
|---------------|
first_name = 'john'
last_name = 'smith'
message = f'{first_name} [{last_name}] is a good coder'
print(message)

|-------------|
|String method|
|-------------|
len() - counts the number of character also we can enforce the limit for particular text box like "comment"
upper()- convert the value to upper case
lower() - conver the value to lower case
find() - particular value in string and retun the index of present string also its case sensitive
replace() - will replace the value with new string
in  - check the value in provide string, this returns true or false(Boolean value)

|--------------------|
|Arthemetic opertator|
|--------------------|
+,-,*,/ will return float value, // will return the integer, % will return the reminder, 2**3(Exponent)
increment x=10, x=x+2, x+=3(Augmented assignment operator)

|-------------------|
|Operator precedence|
|-------------------|
X=(10+3)*2 = 16 1. Paranthesic, 2. exponentiation 3. Multiplication or division, 4. Addition or subraction
x=(10+3)*2**2 = 22

|-------------|
|Math function|
|-------------|
round() - will round the value
abs() - will return positive number if we give negative it return positive

import math - is a module can access math function
https://docs.python.org/3/library/math.html use the link to know math functions

|---------|
|condition|
|---------|
if :
else:

|----------------|
|Logical operator|
|----------------|
AND - Both Condition should be satisfied 
OR - Any one condition should be satisfied
NOT - If condition return TRUE it will be converted into false
	  if condition return FALSE it will be converted into true
	  
|--------------------|
|Comparision operator|
|--------------------|
name = 'araaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa'
length = len(name)
if length < 3:
 print("Name must be greater than 3 characters")
elif length > 50:
  print("Name must be less than 50 character")
else:
  print("Name is good")

|-----|
|While|
|-----|
To execute block of code multiple times
While (condition) #if condition is true going to execute the program
Break	          #if given condition is passed but while loop will still exectue untill while condition fails, so to stop break staement is used

|---------------------------|
|Guess game using while loop|
|---------------------------|
Computer has scerect nummber of 10 it lets user to guess the number 1-10 by giving 3 chance .
secret = 10
total_chance = 3
guess = 0
while guess < total_chance:
  value = int(input('Enter your guess: '))
  guess += 1
  if value == secret:
    print("You Win!")
    break
else:
  print("Better luck next time :(")
  
|-----------|  
|Car program|
|-----------|
command = ""
while command !="quit":
  command=input('>').lower()
  if command == "start":
    print("Car Started....")
  elif command == "stop":
    print("Car stopped....")
  elif command == "help":
    print ("""
 Start - to start the Car
 Stop - to stop the Car 
 Quit - to terminate the function
    """)
  elif command == "quit":
    break
else:
  print("Sorry i dont understand")

|-----------------------------------------------------------| 
|Program to check if car already started and already stopped|
|-----------------------------------------------------------| 
command = ""
started = False
while command !="quit":
  command=input('>').lower()
  if command == "start":
      if started:
        print("Car already started")
      else:
        started = True
        print("Car Started....")
            
  elif command == "stop":
      if not started:
        print("Car already stopped")
      else:
        started = False
        print("Car stopped....")
  elif command == "help":
    print ("""
 Start - to start the Car
 Stop - to stop the Car 
 Quit - to terminate the function
    """)
  elif command == "quit":
    break
  else:
    print("Sorry i dont understand")

|---------|	
|For loops|
|---------|

for 
item_cost = [10,20,300,400]
total = 0
for item in item_cost:
  total += item
print(f"Total value :{total}") this will print the only the total value

item_cost = [10,20,300,400]
total = 0

for item in item_cost:
  total += item
  print(f"Total value :{total}") putting inside the for loop will print all value iteration
  
Nested loop
-----------
For value 1 in loop1
	for value 2 in loop 2
	

List
----
number = [1,2,3]

2d list
--------

list has list inside 

program to remvoe duplicates
list = [1,2,5,4,2,5]
unique = []
for value in list:
  if value not in unique:
    unique.append(value)
print (unique)

TUPLES
------
are same as list
they cannot be modified

Value = (1,2,3)

Iteration by item
-----------------
fruits = ['apple', 'pearls', 'strawberrys', 8, 9 , 10]

for fruit in fruits
	if fruit = 'pearls'
	print(fruit);
	else:
	print('not fruit')
 

UNPACKING
----------
it used to assign the value to all variable in single lines

i.e 

Coordinates = (1,2,3)
x = Coordinates(0)
y = Coordinates(1)
z = Coordinates(2)

insted it can be written in below way

Coordinates = (1,2,3)
x,y,z = coordinates

it can also used in list

Coordinates = [1,2,3]
x,y,z = coordinates

DICTONARIES
-----------
we want to store key values

Phone = input("Enter the phone: ")
dictnary = {
"1":"one",
"2":"two",
"3":"Three"
}
output = ""
for c in Phone:
  output += dictnary.get(c,":(") + ""
print (output)

Emoji Convertor
----------------
message = input(">")
words = message.split(" ")

the above line splits the character

Function
---------
Function is like a container stores few lines of code(action to perform), it breaks the code smaller and more managable conent
name the function with lower case character and if multiple words then seperate them with underscore then () followed by : 
we are telling block of code belongs to function

whenever we end column at end of the function 
function will be executed only when it is called
function can be defined as below
Syntax:	def function_tutorial() 
		{
		}
Function can be called after it is defined, so always define the function first and call them
we need to have 2 line breaks after the funcation

Parameter
----------
we can define parameter in function 
Syntax:
Syntax:	def function_tutorial(parameter1, parameter2) 
		{
		}
		def function_tutorial(name):
			print(f' hi {name}')
			print("john how are you")
		
		print("hello")
		function_tutorial("jhone", "smith")
		function_tutorial("Mary")


Whenever function parameter are provide always should suppy value, if values are not passed it will throw an error

Keyword Arguments
-----------------
Positional arguments 
		def function_tutorial(name):
			print(f' hi {name}')
			print("john how are you")
		
		print("hello")
		function_tutorial("jhone", "smith") -> this is called "Positional Arguments"
		function_tutorial("Mary")

Jhone and smith are position based were as if we exchange the value gets changed

		def function_tutorial(name):
			print(f' hi {name}')
			print("john how are you")
		
		print("hello")
		function_tutorial(50, 6, 7)
as user we will not be aware what is those parameter value is
so python, has option of improve the readablity of the code 

	function_tutorial(total = 50, shipping = 6, discount = 7)
	this is called keyword arguments, which improve the readablity of the code
most part use position argument, if we are taking numerical value we should go with "keyword argument"

when passing both 
Also, "keyword argument" has to be provided after the "Positional Argument"

Retrun Statement
----------------
Function that return value
if we have function that calculates the value so it will return the statement
Syntax

def square(number):
	print (number*number)
	
	
print (square(8)) in this program default it returns None because there is not return statement, also none is object

def square(number):
	return (number*number)
	
	
print (square(8))

Creating a reusable function
-----------------------------



Function call
--------------
Detail about how the code works

def relative_fun(name):       Declaring the function name
  final = name.split(" ")		i am splitting the input values, after space
  reference = {					using the dictnary concept								
  "good" : ":)",					provided the values
  "bad"  : ":(" 
  }
  output = ""								
  for word in final:						now looping throgh the final variable, and storing each value in iteration				
    output += reference.get(word, "!")          searching the value in reference(dictnary) using get method we are searching value of word in each iteration,  
  return output								Then adding the values together and return the output


name = input('How are you doing: ')    Getting the input from the user
print(relative_fun(name))				next we are calling the function inside print state first, then control goes to the function, returned value is printed in name of function

Exception
----------
How to handle error in python
Look type of error
Syntax:
try:
  code 
Except provid the type of error 
	Print("the message as you wish")
	
0- Success
1- Crash

Comments in python
-------------------
Use "#"

Classes
-------
Classes define new types
number, string, boolean - types basic 
list and dictnary - concept

Class naming convention
-------------------------
variable and function lower case, def  add_value
for Classes we have Capitalize the first word and second word , class PointValue

Class defines  the blue print
Object is instance of the class

to create object
type the name of class 

Constructors
------------
Constructor is called at the time of creating the object 
class Construct
def __init__(self, x, y):
self.x=x
self.y=y





    for item in range(1, cell + 1):
        if(item=="Gold"):
            print(cell.value);

-------------------------------
Bash commands works with linux 
-------------------------------
ls - list all the directory 
pwd - present working directory
cd - Change Directory
cd.. - bring back to one dirctory behind
clear - clears the command from terminal
cd / - take to root directory
cd ~ - it takes to user directory
open .(dot refer the folder) - it folder we currently in
open filename - opens the file
mkdir foldername - make directory
tocuh filename - it creates the file
open -a "Sublime Text" 
open -a "Sublime Text" index.html
mv - move command 
rm - remove the file(works only for file)
rm -r(recurrsively) - remove the folder
Say this is sooo cool - it speaks 


OOP
----

Class - Blue Print
Object are memory created inside class

#method with parameters and it returns value
	def __init__(self, name, age):
			self -> is a reference keyword which is not created yet
			self.name
#attribute	self.age
	Intantiate - calling the object __int__
	memeory objected is created 
	here attribute is dynamic specific to each class object 
	self refers to the class name
	
#method with no parameters
	def run(self)
		print('run')
		return 'done'
	seperate memeory objected is created 

Attribute & Methods
-------------------
Class object Attribute - is different is static, doesnt change across different instances, it is not dynamic like attribute inside the method, it is a global
Class PlayerObject
	membership = True declared  after the class declaration
	
__init__
---------
Constructor, Intantiate object
"dunter method" - if it has __ underscore we should'nt modify


Class and Static method
-----------------------
@classmethod - decorator
instead "self" which we use in traditional class declaration
we can use the ClassMethod without instantiating a class
Used because of the Class attributes
#cls - used to intantiate the object
def add(cls, num1 + num 2)
	return cls('objectname' num1 + num2)
		
@staticmethod
it works like above but it wont have access to cls
def add(num1 + num 2)
	return num1 + num2

Reveiw 
------
Class 'Name' should be in camel case
we need to instantiate class to create instance i.e Object(memory)
def __init__ is called intatiate object - to customize our object
def method(self)
@classmethod - Method that call class without instanciating the object 
@staticmethod - 

Developer Fundamentals
----------------------
Test you assumption - Test our understanding of what it is?
return self -  

Encapsulation
-------------
Binding of data and function which can be encapsulate into one big object
so that other machine can interact
data and function are attributes inside the encapsulation

Abstraction
-----------
Hiding of information 
Abstrating information only based on requirment
At the same time, methods in abstraction could be overridden

Private vs Public
-----------------
There is no private variable in python
however we can use "self._name"
underscore - "_" means that is private no modification required
__doc__ dont try to modify the double underscore of dunter method 

inheritance
-----------
if we want to inherit method from other class
then use inheritance

class Users:
	def SigIn(self):
	print('logged in')
	
inherit:
---------
class Wizard(Users):
	pass
https://python.plainenglish.io/comprehensions-in-python-a244e55aa2e5#7f53













