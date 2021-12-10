Q4 .Auditors at a small community bank randomly sample 100 withdrawal transactions made during 
 the week at an ATM machine located near the bank’s main branch. Over the past 2 years, the average 
 withdrawal amount has been $50 with a standard deviation of $40. Since audit investigations
 are typically expensive, the auditors decide to not initiate  further investigations if the mean transaction amount of the sample is between $45 and $55.
 
 The auditors from the above example would like to maintain the probability of investigation to 5%. Which of the following represents the minimum number transactions that they should sample if they do not want to change the thresholds of 45 and 55? Assume that the sample statistics remain unchanged.
 
 A.	144
B.	150
C.	196
D.	250
E.	Not enough information



```python
### importing libraries

import numpy as np 
from scipy import stats
from scipy.stats import norm 
```

 For 5%, z has to be +/-1.96


```python
## As z = (sample_mean-population-mean)/(standard deviation/sqrt(n))

## So 1.96 = 5 /(40/sqrt(n))
## => 1.96 = 5 * sqrt(n)/40
## => sqrt(n) = (1.96*40)/5

n = ((1.96*40)/5)**2
print("n =",n, ", round off to", round(n))
```

    n = 245.86240000000004 , round off to 246
    

As n=246. So the correct answer is Option D


```python

```
