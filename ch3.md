# Chapter 2 Exercise

## Solve
> [1] Suppose I show you a call stack like this.
![problem 3.1](img/3-1.png)
What information can you give me, just based on this call stack?
```
the greet function called first with name = maggie
then it called greet2 function with name = maggie
and still in greet2 function after it completes will return to greet function and resume
```

> [2] Suppose you accidentally write a recursive function that runs
forever. As you saw, your computer allocates memory on the
stack for each function call. What happens to the stack when your
recursive function runs forever?
```
stack has limited amount of space.
so program will run until the stack runs out of space 
then program will exit with stack overflow Error.
```