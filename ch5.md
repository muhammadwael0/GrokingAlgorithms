# Chapter 2 Exercise

## Which of these hash functions are consistent as hash function?
> [1] f(x) = 1 <-- Returns "1" for all input
```

```

> [2] f(x) = rand() <-- Returns a random number every time
```

```

> [3] f(x) = next_empty_slot() <-- Returns the index of the next empty slot in the hash table
```

```

> [4] f(x) = len(x) <-- Uses the length of the string as the index
```

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
> [5]
```

```

> [6]
```

```

> [7]
```

```