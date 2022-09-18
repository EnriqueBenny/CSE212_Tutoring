[Home](landing.md)
[Back](list_comprehension.md)

1 : Fix this list comprehension
```python
broken_list_comprehension = [for x in range(10): print(x) if x != 1]
print(broken_list_comprehension)

# 0 2 3 4 5 6 7 8 9
# Answer:
[print(x) for x in range(10) if x != 0]
```
2 : Write a list comprehension that prints a letter or number 100 times.
```python
#Answer:
[print(0) for x in range(100)]
```

3 : The dataset below is 15 too high, use a list comprehension to bring it down to where it needs to be.
```python
broken_data = [18, 15, 30, 25, 68, 45, 99, 44, 12, 85, 77]
# Answer:
fixed_data = [x - 15 for x in broken_data]
print(fixed_data)
```