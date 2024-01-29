# ES

Goal is to replicate some results from a paper via simulations.

## Usage
```
Rscript ES.R
```

## Output
*print_t(M)* looks at the *t*-distribution with *df = 3.5, 5, 8*, *n = 250, 500* and $\beta = 0.99, 0.995$  and prints out the MSE, variance, and bias of both the $\hat{\text{ES}}$ and AA ES estimators through a Monte Carlo simulation of *M* replications.
*print_gpd(M)*, *print_weibull(M)*, *print_t2(M)*, and *print_gpd2(M)* are defined similarly for other parameters/distributions.

The output for the above functions for *M = 2500* yields results that are re-organized into the tables in the following section.


## Results
This is currently work in progress.

**t-distribution, n = 250**
|        |                   | MSE $\beta = 0.99$ | MSE $\beta = 0.995$ | MSE $\beta = 0.99$ | MSE $\beta = 0.995$ | MSE $\beta = 0.99$ | MSE $\beta = 0.995$ |
|--------|-------------------|--------------------|---------------------|--------------------|---------------------|--------------------|---------------------|
| df=3.5 | $\hat{\text{ES}}$ | 3.513701           | 6.918576            | 3.349879           | 5.931118            | -0.4064011         | -0.9949018          |
|        | AA                | 3.045859           | 6.618685            | 2.757139           | 4.895043            | -0.5383521         | -1.313621           |
| df=5   | $\hat{\text{ES}}$ | 0.9119978          | 1.772814            | 0.8458146          | 1.465247            | -0.2579177         | -0.5551157          |
|        | AA                | 0.896156           | 1.88101             | 0.7838646          | 1.292381            | -0.3355666         | -0.7675588          |
| df=8   | $\hat{\text{ES}}$ | 0.3733118          | 0.6882679           | 0.3424361          | 0.5728771           | -0.1761041         | -0.3400294          |
|        | AA                | 0.3821088          | 0.7564698           | 0.3286057          | 0.5127364           | -0.2315912         | -0.4939012          |

**t-distribution, n = 500**
|        |                   | MSE $\beta = 0.99$ | MSE $\beta = 0.995$ | MSE $\beta = 0.99$ | MSE $\beta = 0.995$ | MSE $\beta = 0.99$ | MSE $\beta = 0.995$ |
|--------|-------------------|--------------------|---------------------|--------------------|---------------------|--------------------|---------------------|
| df=3.5 | $\hat{\text{ES}}$ | 2.32565            | 4.622969            | 2.311198           | 4.324478            | 0.1239996          | 0.547924            |
|        | AA                | 1.683792           | 4.569174            | 1.514917           | 4.20693             | 0.4116804          | 0.6032632           |
| df=5   | $\hat{\text{ES}}$ | 0.548986           | 1.095874            | 0.5352389          | 0.9876675           | 0.1181574          | 0.329547            |
|        | AA                | 0.4980796          | 1.152373            | 0.42303            | 1.005189            | 0.2742606          | 0.3841695           |
| df=8   | $\hat{\text{ES}}$ | 0.1927528          | 0.3692167           | 0.1858955          | 0.3318638           | -0.08325665        | -0.1936121          |
|        | AA                | 0.1933235          | 0.4038955           | 0.1597503          | 0.3446732           | -0.183404          | -0.2436394          |

## Authors

- [@jw8u](https://www.github.com/jw8u)
