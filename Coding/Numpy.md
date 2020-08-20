### generate array，all elements in the array have the same type, such as integer or floating point(default)

```
my_array = np.array([1, 2, 3, 4])
np.ones(10) # generates 10 floating point ones
np.zeros(10) 
np.random.random(10) # generate randomly from uniform [0,1]

normal_array = np.random.randn(1000) #generate from N(0,1)
np.mean(normal_array)
np.std(normal_array))

normal_5_7 = 5 + 7*normal_array #generate from N(5,7)
np.mean(normal_5_7), np.std(normal_5_7)

np.arange(0.,1.01,0.1) #a list with evenly-spaced values
np.random.choice(my_array, number, replace=False) #sample with/withour replacement
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

### arithmetic of two numpy arrays

#### '+' is different the one for lists

```
first = np.ones(5)
second = np.ones(5)
first + second # adds in-place

first_list = [1., 1., 1., 1., 1.]
second_list = [1., 1., 1., 1., 1.]
first_list + second_list # concatenation
```

#### multiply each element by the number, add the number to each element

```
first+1, first*5 
```

#### Multiplying two arrays element-by-element

```
(first +1) * (first*5)
```

#### dot product

```
np.dot((first +1) , (first*5))
```
