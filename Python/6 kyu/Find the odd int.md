## Check out this [kata](https://www.codewars.com/kata/54da5a58ea159efa38000836)
### Description:

Given an array of integers, find the one that appears an odd number of times.

There will always be only one integer that appears an odd number of times.

## My Solution:
```
from collections import Counter
from functools import reduce

def find_it(seq):
    counts = list(Counter(seq).items())
    for x in counts:
        if x[1] % 2 !=0:
            return x[0]
    return reduce(lambda x, y: x^y, seq)
```
