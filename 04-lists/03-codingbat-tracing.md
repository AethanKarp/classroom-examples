# Codingbat Solution Tracing
This is a collection of [Codingbat](http://codingbat.com) solutions that may or may not work. 
The idea is to trace the code to discover the errors or to determine if the solution is infact correct.

## Adding a post
Simply edit this document and add your code as shown below with the following rules:
1. Ensure your code is within triple backticks like below. 
2. Add [type annotations](https://docs.python.org/3/library/typing.html) for the function header so we know what type of data the function recieves and returns.
3. Ensure that the name of the function is under an appropriate `###` header.
4. Ensure that the problem's explanation text is above all the "solutions". 
5. Keep the problems in alpha order.

## Example:
### double
Create a function that will double the given integer.
```
double(5) -> 10
double(3) -> 6
double(0) -> 0
```
Solutions:

```python
def double(n: int) -> int:
    return n * 2
```

```python
def double(n: int) -> int:
    return n * 1
```

End example
---

### swapEnds
Create a list that swaps the places of the last term and the first term
```
swapEnds([1, 2, 3]) → [3, 2, 1]
swapEnds([5, 11, 9]) → [9, 11, 5]
swapEnds([7, 0, 0]) → [0, 0, 7]
```
Solutions:

```python
def swapEnds(nums):
  newlist = []
  newlist.append(nums[-1])
  for i in range(len(nums)):
    if i < len(nums) - 1 and i > 0:
      newlist.append(nums[i])
  newlist.append(nums[0])
  return newlist
```
