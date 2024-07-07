# Chapter 1 Exercise

## Solve 
> [1] Suppose you have a sorted list of 128 names, and you're searching through it using binary search. 
What's the maximum number of steps it would take?
```
log2(128) = 7
then 7 steps.
```

> [2] Suppose you double the size of the list. 
What's the maximum number of steps now?
```
log2(128 * 2) = 8
then 8 steps.
```

## Give the run time for each of these scenarios in terms of Big O.
> [3] You have a name, and you want to find the
person's phone number in the phone book.
```
Binary Search -> O(log n)
```

> [4] You have a phone number, and you want to
find the person's name in the phone book.
(Hint: You'll have to search through the whole
book!)
```
Simple Search -> O(n)
```
> [5] You want to read the numbers of every person in the phone book.
```
all persons -> O(n)
```
> [6] You want to read the numbers of just the As.
```
number of As -> O(n/26) = O(n) ignore the number
```