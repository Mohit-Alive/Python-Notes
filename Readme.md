# Python Notes

## Data Types
``` Python
a = 12
b = 2.3
c = complex(2,3)
d = "Hello"
isconnected = true

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