# Chapter 5 Exercise

## Which of these hash functions are consistent as hash function?
> [1] f(x) = 1 <-- Returns "1" for all input
```
consistent always return 1
```

> [2] f(x) = rand() <-- Returns a random number every time
```
not consistent return a random number
```

> [3] f(x) = next_empty_slot() <-- Returns the index of the next empty slot in the hash table
```
not consistent Returns the index of the next empty
```

> [4] f(x) = len(x) <-- Uses the length of the string as the index
```
consistent always return a fixed number for input
```

## which hash functions would provide a good distribution? Assume a hash table size of 10 slots.
```
Suppose you have these four hash functions that work with strings:

a. Return "1" for all input.

b. Use the length of the string as the index.

c. Use the first character of the string as the index. So, all strings
   starting with a are hashed together, and so on.

d. Map every letter to a prime number: a = 2, b = 3, c = 5, d = 7,
   e = 11, and so on. For a string, the hash function is the sum of all
   the characters modulo the size of the hash. For example, if your
   hash size is 10, and the string is "bag", the index is 3 + 2 + 17 %
   10 = 22 % 10 = 2.
```
> [5] A phonebook where the keys are names and values are phone
numbers. The names are as follows: Esther, Ben, Bob, and Dan.
```
a -> not good distribution, always return 1 for all inputs.
b -> not good you will have a linked list with 3 element and one with 1 element and a lot of empty slots
c -> good but still bad if a lot of names of the same first char will cause a big collision.
d -> very very good cause distribute depend on the word "SASA" and "SOSO" have different hash codes 
     you can decrease the collisions by increase the modulo
```

> [6] A mapping from battery size to power. The sizes are A, AA, AAA, and AAAA.
```
a -> not good distribution, always return 1 for all inputs.
b -> good becuase of different string size so it has a good distribution
c -> bad because all strings start with letter A
d -> very very good cause distribute depend on the word "A" : 2 and "AA" : 4 have different hash codes
     you can decrease the collisions by increase the modulo
```

> [7] A mapping from book titles to authors. The titles are Maus, Fun Home, and Watchmen.
```
a -> not good distribution, always return 1 for all inputs.
b -> good becuase of different string size so it has a good distribution
c -> good because all names has different first char will cause no collision.
d -> very very good cause distribute depend on the word "Maus" and "Home" have different hash codes 
     you can decrease the collisions by increase the modulo
```