# Answers to Big O Notation Practice:
---
```python
x = 10
b = True
def first():
    if b is True:
        print('yes')
# O(1)
def second():
    for i in range(x):
        print('no')
# O(n)
def third():
    for i in range(x):
        print('hi')
    for i in range(x):
        print('bye')
    for i in range(x):
        print('later')
# O(3n)
def fourth():
    for i in range(x):
        for i in range(x):
            print('Stop!')
# O(n^2)
def fifth():
    for i in range(x):
        for i in range(x):
            for i in range(x):
                if b is True:
                    print('hi')
    for i in range(x):
        for i in range(x):
            for i in range(x):
                if b is True:
                    print('hi')
# O(2n^3)
def sixth():
    '''Create a function that prints a phrase with a time of O(n). 
    Use the variable 'x' for your range.'''
    for i in range(x):
        print('phrase')
def seventh():
    '''Create a function that prints a phrase with a time of O(4n^2).
    DON'T CALL THIS FUNCTION, YOUR COMPUTER WILL CRY!
    Use the variable 'x' for your range. '''
    for i in range(x):
        for i in range(x):
            print("don't do this normally")
    for i in range(x):
        for i in range(x):
            print("it's really bad for your computer")
    for i in range(x):
        for i in range(x):
            print("probably shouldn't even run this code")
    for i in range(x):
        for i in range(x):
            print("just to be safe")
def eigth():
    '''Turn this O(n^2) into a O(2n).
    Use the variable 'x' for your range.'''
    for i in range(x):
        print("I'm broken")
    for i in range(x):
        print('fix me')
```