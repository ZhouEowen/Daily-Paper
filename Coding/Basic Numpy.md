### generate array，all elements in the array have the same type, such as integer or floating point(default)

```
my_array = np.array([1, 2, 3, 4])
np.ones(10) # generates 10 floating point ones
np.zeros(10) 
np.random.random(10) # generate randomly from uniform [0,1]

normal_array = np.random.randn(1000) #generate from N(0,1)
np.mean(normal_array)
np.std(normal_array))

np.dtype(float).itemsize #8
```

### have similar functionality as lists

```
len(my_array) #4
my_array.shape #(4,)
my_array.dtype #dtype('int64')
```

### two ways to manipulate numpy arrays 

```
my_array.mean()
np.mean(my_array)
```

