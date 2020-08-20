
### two-sided z-test for proportions

```
import statsmodels
from statsmodels.stats.proportion import proportions_ztest

x = np.array([74,100])
n = np.array([152,266])

zstat, pvalue = statsmodels.stats.proportion.proportions_ztest(x, n)    
print("Two-sided z-test for proportions: \n","z =",zstat,", pvalue =",pvalue)
```
