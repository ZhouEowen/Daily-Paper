# scipy

### normal distribution 

```
from scipy.stats import norm
import matplotlib.pyplot as plt

x = np.linspace(-10, 10, 1000) # returns evenly-spaced numbers over a specified interval
pdf_x = norm.pdf(x, 1, 3)
plt.plot(x, pdf_x);
```

# statsmodels

### two-sided z-test for proportions

```
import statsmodels
from statsmodels.stats.proportion import proportions_ztest
import numpy as np

x = np.array([74,100])
n = np.array([152,266])

zstat, pvalue = statsmodels.stats.proportion.proportions_ztest(x, n)    
print("Two-sided z-test for proportions: \n","z =",zstat,", pvalue =",pvalue)
```
