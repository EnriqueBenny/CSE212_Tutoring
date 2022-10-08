# Stacks:
[Previous](big_o_notation.md)
[Home](landing.md)
[Next](queues.md)

## Intro
---
Stacks are both a concept and an object you will be working with in python. In particular, you need to make sure to get 'down' and remember the concept of a stack. You will need it later.

A stack is a series of data layered one on top of the other (stacked). To conceptualize it, it's similar to chips stacked in a pringles can. When you want to grab a chip out of a pringles can, you grab the one on the top. You can't just reach to the bottom without removing all the other chips. In a stack, data is arrange the same way. You can only put data on the back/top of the stack, and can only remove from the back/top. The reading called this FILO (First-in Last-out). To help you better understand it in code, lets look at some examples.

## Examples:
---
A stack in python is best represented by an array, so we'll be using a python list to help conceptualize it.
```python
stack = []
```
Once we've creaded our stack, let's start by adding items to it using the append() function.
```python
for x in range(10):
    stack.append(x)
print(stack) # [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
```
This is our stack. Notice that we used the append() function to add everything to the top of the stack, now we'll use the pop() command to remove a few items.
```python
for x in range(3):
    stack.pop()
print(stack) # [0, 1, 2, 3, 4, 5, 6]
#
```
The pop command will remove the items from the back, in this case we told it to pop() 3 times, so it removed 9, 8, and 7.
The commands can also be written out individually so you can better conceptualize it:

```python
#create the array
example = list()
#add items to the end of the array (remember FILO)
example.append(0)
example.append(1)
example.append(2)
example.append(3)
example.append(4)
example.append(5)
#remove items from the end of the array (FILO)
example.pop()
example.pop()
example.pop()
print(example)
# Result will be: [0, 1, 2]
example.append(6)
example.append(7)
example.append(8)
example.pop()
example.pop()
example.append(9)
print(example)
# Result will be: [0, 1, 2, 6, 9]
```
> In python, the different commands to interact with a stack are as follows:
> * list() - the array used for a stack. 
> * list.append() - adding items on top of the stack - FI (First-In)
> * list.pop() - remove the last item from the list. LO (Last-Out)

#### Problem
Now you try:

```python
#Problem 1
problem = list()
problem.append(0)
problem.append(1)
problem.append(2)
problem.pop()
problem.pop()
problem.append(3)
problem.append(4)
problem.append(5)
problem.append(6)
problem.append(7)
problem.append(8)
problem.pop()
problem.pop()
problem.pop()
problem.append(9)
problem.append(10)
problem.append(11)
problem.append(12)
problem.pop()
problem.append(13)
problem.append(14)
problem.append(15)
problem.append(16)
problem.append(17)
problem.pop()
problem.pop()
problem.append(18)
problem.append(19)
problem.append(20)
#What will the output be? Write it down before you print the list.
#print(problem)

#Problem 2
# We are looking for the output:
# [0, 1, 2, 3, 11, 12, 13, 14, 15, 16]
# Change the variables 'pops' to the proper value to find
# the output we are after.
problem = list()
problem.append(0)
problem.append(1)
problem.append(2)
problem.append(3)
problem.append(4)
problem.append(5)
problem.append(6)
problem.append(7)
problem.append(8)
problem.append(9)
problem.append(10)
#Change pops, will determine how many times the function pop is called. 
pops = 0
for i in range(0, pops):
    problem.pop()
problem.append(11)
problem.append(12)
problem.append(13)
problem.append(14)
problem.append(15)
problem.append(16)
problem.append(17)
problem.append(18)
problem.append(19)
problem.append(20)
#Change pops, will determine how many times the function pop is called. 
pops = 0
for i in range(0, pops):
    problem.pop()
print(problem)
```
Finish the problems, then compare with the solution.


[Solutions](stacks_solution.md)