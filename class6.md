# Random Module in Python

## What is it?

Python offers random module that can generate random numbers.

These are pseudo-random number as the sequence of number generated depends on the seed.


![d](https://techvidvan.com/tutorials/wp-content/uploads/sites/2/2020/07/generating-random-numbers-in-python.jpg)


## When to use it?
> We want the computer to pick a random number in a given range Pick a random element from a list, pick a random card from a deck, flip a coin etc. When making your password database more secure or powering a random page feature of your website.


## Random functions

- ***Randint***
To generate a random number between 1 and 5.

```
import random
print random.randint(0, 5)
```



- ***Random***
To generate a random number between 1 and 5.

```
import random
print random.randint(0, 5)
```



- ***Randint***
To generate a large random number.

```
import random
random.random() * 100
```


- ***Choice***
To generate a random value.

```
random.choice( ['red', 'black', 'green'] ).
```



- ***Shuffle***
To randomly shuffle elements of lists (list), strings (str) and tuples (tuple).

```
from random import shuffle
x = [[i] for i in range(10)]
shuffle(x)
```


- ***Randrange***
The randrange() method returns a randomly selected element from the specified range.

```
random.randrange(start, stop[, step])
import random
for i in range(3):
    print random.randrange(0, 101, 5)
```

![r](https://www.programmersought.com/images/352/dc3dbb3214b9e329cee7edfda275d3b8.png)
