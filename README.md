# ML-Primes
Predicting prime numbers with machine learning algorithms

## Algorithms
### sklearn
 - RandomForestRegressor

## Projects
### Predicting Primes
Given primes p<sub>n</sub>, p<sub>n+1</sub>, and p<sub>n+2</sub>, predict the value of prime p<sub>n+3</sub>.
 - [x] Random Forest   
     This model performs extremely well (R<sup>2</sup> > 0.9999) at predicting the next prime number in the series

### Factoring Primes
Given a product of two primes, predict the values of the factors.
 - [x] Random Forest  
     RF is performing well in two scenarios: 1) RF has the product and a factor, the algorithm can easily predict the other factor (R<sup>2</sup> > 0.99) and 2) RF has only the product, the algorithm can predict the lower factor with fair metrics (R<sup>2</sup> ~ 0.91). When combining these two experiments (predict small factor, then use that prediction as the input for the prediction of the second factor), RF demonstrates lower capabilities (R<sup>2</sup> ~0.74). 

## Resources
 - [ML for Factoring Primes](https://www.datasciencecentral.com/profiles/blogs/factoring-massive-numbers-a-new-machine-learning-approach)
