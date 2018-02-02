---
title: Random Walks!
layout: post
---

```python
#Random Walks!
from random import seed
from random import randrange
from matplotlib import pyplot
seed(1)
```
The seed is just for reproducibility
```python
series = [randrange(10) for i in range(10)]
```
We're taking a random number in the range of 0-9, and doing this 10 times
print(series)
```python
[2, 9, 1, 4, 1, 7, 7, 7, 6, 3]
pyplot.plot(series)
pyplot.show()
```


![png](output_1_0.png)

