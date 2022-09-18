# List Comprehension:
[Home](landing.md)
[Next](big_o_notation.md)

## Intro
---
List comprehension can be difficult to wrap your brain around at first, but with some practice, you'll find it to be a useful and concise tool to put in your belt.

### What is it?
List comprehension is the process of condensing a loop into a single line, best used for simple processes, it is effectively used when you need to create a simple data set or change an existing data set in the same way.
### Breaking it down
Typically, the most difficult thing with list comprehension is what parts of the code correlate with a standard for loop, so let's start with a basic loop:
```python
for x in range(100):
    print('loop')
```
We can now break this loop down into three parts: the identifier, the range, and the body. 
- The identifier is the target of the loop, so whatever the loop is achieving will be done to the identifier for each time it loops through. In this case, the x will print('loop') for each time the loop runs. 
- The range is a bit more self explanatory, you can find plenty of other resources online for specifics, but it is used to determine how many times the loop will occur.
- The body is where you write the code that will determine what the loop does. 
### Connecting the pieces
Now that we've broken down the pieces of a for loop, let's take a look at how that relates to list comprehension.
A standard LC will look something like this:
```python
#This is one way.
[print('loop') for x in range(100)]
#This is another.
lc = ['loop' for x in range(100)]
print(lc)
```
>Despite being a list, you don't have to give it a variable, but I would personally highly suggest it.

- Let's focus on the first of these two examples, we see that the first part, our identifier, is 'loop' this will create and add the string 'loop' to the list for each instance of the loop. If you compare the example in the 'breaking it down section,' you can see that this part belongs to the body of the loop, but is placed first in list comprehension.
- Everything else after that is exactly what you'd see in a normal for loop. 'for x in range.' This is the easiest part of list comprehension to remember - don't let the surrounding differences confuse you.

#### Stepping it up a little.
Once you have a basic idea how list comprehension works, you can now further expand the idea a little by adding an if statement.
```python
#Won't print 0, but will print 1-9
[print(x) for x in range(10) if x != 0]
#Prints only odd numbers.
[print(x) for x in range(100) if x % 2]
```
With the 'if' condition on the end, you've got another tool to affect the list comprehension.

#### Examples:
Additional examples, and a few scenarios to look at. Feel free to play around with the code for a bit.
```python
# Scenario: measuring data, but all the values are off by the same amount due to a forgotten variable. 
broken_data = [10, 15, 30, 25, 68, 45, 99, 44, 12, 85, 77]
y = 6
fixed_data = [x + y for x in range(broken_data)]
print(fixed_data)
# You don't want any of the values that are divisable by 3
[print(x) for x in range (100) if x % 3]
```

#### Practice:
>This practice is purely for your sake, be honest with yourself and don't just copy the other examples, try to see if you actually know it.
1 : Fix this list comprehension
```python
broken_list_comprehension = [for x in range(10): print(x) if x != 1]
print(broken_list_comprehension)
# 0 2 3 4 5 6 7 8 9
```
2 : Write a list comprehension that prints a letter or number 100 times.

3 : The dataset below is 15 too high, use a list comprehension to bring it down to where it needs to be.
```python
broken_data = [18, 15, 30, 25, 68, 45, 99, 44, 12, 85, 77]
```

[Answer Sheet](list_comprehension_answers.md)