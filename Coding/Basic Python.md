# dictionary

```
enroll2017_dict = {'CS50': 692, 'CS109A / Stat 121A / AC 209A': 352, 'Econ1011a': 95, 'AM21a': 153, 'Stat110': 485} #Keys can be immutable data type such as numbers or tuples or strings (not lists, as lists are mutable)
enroll2017_dict.get('CS630', 5) #providing a default value if the key isn't found,does not store a new value, only provides a value to return if the key isn't found

enroll2017_dict.values()
enroll2017_dict.items()
```

# creating tuples with zip

zip() returns an iterator that aggregates elements from each of the iterables. The iterator stops when the shortest input iterable is exhausted.

set() returns a set object, using set() can make zip printable

```
float_list = [1., 3., 5., 4., 2.]
int_list = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

viz_zip = set(zip(int_list, float_list))
viz_zip
```

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
