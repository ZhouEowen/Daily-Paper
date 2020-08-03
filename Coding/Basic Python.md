# lambda function

```
square = lambda x: x*x
print(square(3))

hypotenuse = lambda x, y: x*x + y*y
hypotenuse(3,4)
```

# Example 1: find prime

```
#using loop
N = 100;
primes = [];
for j in range(2, N):
    count = 0;
    for i in range(2,j):
        if j % i == 0:
            count = count + 1;
    if count == 0:
        primes.append(j)
print(primes)

#using one-line loop
primes_lc = [j for j in range(2, N) if all(j % i != 0 for i in range(2, j))]
```

# Example 2: isprime

```
#using lambda function
def isprime(N):
    count = 0;
    if not isinstance(N, int):
        return False
    if N <= 1:
        return False
    for i in range(2, N):
        if N % i == 0:
            count = count + 1;
    if count == 0:
        return(True)
    else:
        return(False)
```
