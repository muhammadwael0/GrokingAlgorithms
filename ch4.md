# Chapter 2 Exercise

## Solve
> [1] Write out the code for the earlier sum function.
```
def sum(arr):
    total = 0
    for x in arr:
        total += x
    return total
```

> [2] Write a recursive function to count the number of items in a list.
```
def get_len(l):
    if not l:
        return 0
    return 1 + get_len(l[1:])
```

> [3] Find the maximum number in a list.
```
def get_max(l):
    maximum = l[0]
    for i in range(1, len(l)):
        if l[i] > maximum:
            maximum = l[i]
    return maximum
```

> [4] Remember binary search from chapter 1? It's a divide-and-conquer
algorithm, too. Can you come up with the base case and recursive
case for binary search?
```
base case is array with one element otherwise can't find element.
recursive case split the array to half and throw away one half and 
call binary search function on the other one.
```

## How long would each of these operations take in Big O notation?
> [5] Printing the value of each element in an array.
```
you will go through each element -> O(n)
```

> [6] Doubling the value of each element in an array.
```
you will go through each element and double it -> O(n)
```

> [7] Doubling the value of just the first element in an array.
```
access the first element in an array and double it -> O(1)
```

> [8] Creating a multiplication table with all the elements in the array. So
if your array is [2, 3, 7, 8, 10], you first multiply every element by 2,
then multiply every element by 3, then by 7, and so on.
```
you will go through array n time n time -> O(n2)
```