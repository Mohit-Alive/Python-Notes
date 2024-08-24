# Python Notes

## Data Types
``` Python
a = 12
b = 2.3
c = complex(2,3)
d = "Hello"
isconnected = True

print(type(c))

list = [1, 2, 3, 4, 5]               # Sequence Type
tuple = ("Here", "There", "Where")   # Immutable
dict = {"name": "Mohit", "age": 20}  # Mapping Type
set = {1, 2, 3, 4}                   # Set Type
```
## Some Good Practices
```Python
Number: int = 20
Name: str = "Mohit"
```

## Operations
```Python
a: int = 7
b: int = 3
c: int = 3

print(a // b)   # floor division => returns 2
print(a ** b)   # a to the power b
 
a = a + 2       # Both are same
a += 2

print(a == b)   # Returns false
print(a != b)   # Returns true

print(b == c and a < b)   # Returns false
print(b == c or a < b)    # Returns true
print(not (b > a))        # Returns true
```

## Strings
```Python
name:str =  "Mohit"
print("Hello my name is " + name)

print(                  # Prints as it is
    '''
Hi
i am here
        what are you doing
    '''
)
```
### String operations

```python
#Strings are immutable
a = ",,,Mohit,,,"
print(a.upper())            # ,,,MOHIT,,,
print(a.lower())            # ,,,mohit,,, 
print(a.strip(","))         # Mohit
print(a.replace(",","*"))   # ***Mohit***
print(a.split(" "))         # [',,,Mohit,,,']
```
* isalnum = A-Z, a-z, 0-9----> True

* isalpha = A-Z,a-z-----> True

* islower = All lower case -----> True

* isprintable = if all the values within the given string are printable ----> True

* isspace =  only and only if the string contains white spaces -----> True


* istitle = First letter of each word of the string is capitalized ------> True

* isupper = All upper case -----> True

* swapcase = Upper case are converted to lower case and lower case to upper case.

* title =  capitalizes each letter of the word within the string.

## Type Conversion

```python
int_value: int = 50
txt_value: str = "100"

print(int_value + int(txt_value))  # 150
print(str(int_value) + txt_value)  # 50100

# User input
num = int(input("Enter the number: "))
```

## Lists
```python
my_list: list = [True, 1, "Hello", [1, 2, 3]]  # Mutable
here: list[str] = ['txt', 'here', 'there'] 

# List Methods
name: list = ['James', 'Bob', 'Jerry']

name.append('Tom')      # Add              # ['James', 'Bob', 'Jerry', 'Tom']
name.pop()              # Remove last      # ['James', 'Bob', 'Jerry']
name.remove('Bob')      # Remove specific  # ['James', 'Jerry']
name[0] = 'Hey'         # Change           # ['Hey', 'Jerry']
name.insert(1, 'Tim')   # Insert           # ['Hey', 'Tim', 'Jerry']
name.clear()            # Clear            # []
```

## Tuple
Tuple doesn't need any parentheses they are indentify by commas.

```python
coordinates: tuple = 1.5, 2.4     # Immutable
coord: tuple = (1.3, 7.8)         # Both are valid syntax
```

## Sets And Fronzenset
Not in any particular order <br>
Are Mutable <br>
Cant access via index

```python
element: set = {True, 1, 'Tim'}

element.add('Tom')             # Will add in any order
element.remove('Tim')
element.pop()                  # Random
element.clear()          

freeze = frozenset({1, 2, 3})  # Immutable
```

## Dictionary

```python
weather = {'time': '12:00', 
            'duration': 
                {'morning': 'rainy', 
                'afternoon': 'sunny'}}

print(weather['time'])
print(weather['duration']['morning'])

# F-String

name = "Mohit"
chr = f"Hello, My name is {name}"
```

## If-Elif-Else

```python
age: int  = 19

if age <= 0:
    print("Please enter a valid age.")
elif age >= 18:
    print("You are allowed to vote.")
else:
    print("You are not allowed to vote.")

# Short Hand If-Else
number = 10

result = "Above 0" if number > 0 else "Below 0"
print(result)
```

## For-Loop
```python
name = "What are you doing?"

for i in range(5):    # 5 is Exclusive (Not included) 0 to 4
    print(name)

lst = ["Hello", "Hi", "Hey", "Bye"]

for i in lst:
    print(i)
```

## While-Loop

```python
while True:
    user: str = input("You: ")

    if user == "hello":
        print("Bot: Hey there!")
    else:
        print("Bot: Yes, that is interesting.")
```

## Break and Continue

```python
# Continue
number = 5

while number > 0:
    number -= 1

    if number == 2:
        print("Skipping 2")
        continue

    print(number)

print("Done")        # 4 3 Skipping 2 1 0 Done

# Break
number = 5

while number > 0:
    number -= 1

    if number == 2:
        print("Skipping 2")
        break

    print(number)

print("Done")        # 4 3 Skipping 2 Done
```

## Loop-Else

```python
for i in range(3):
    print(f'Iteration: {i}')
else:
    print('Success!')
```

# Functions

```python
from dateTime import dateTime
import time

def show_time():
    current = dateTime.now()
    print(f'Time: {current:%H:%M:%S}')

show_time()
time.sleep(2)
show_time()
```

## Pass And ...
```python
def dont_know:
    pass

def dont_know:
    ...

if num > 0:
    pass
else:
    pass

while True:
    pass
```