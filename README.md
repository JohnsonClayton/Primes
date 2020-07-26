# ML-Primes
Predicting prime numbers with machine learning algorithms

## Algorithms
### sklearn
 - RandomForestRegressor
 - KernelRidge
 - DecisionTreeRegressor (Optimized version of CART)
 
## Investigations
### Kernel Ridge Regression
 - How does it work?
 - Why does it take up so much memory?

## Projects
### Predicting Primes
Given primes p<sub>n</sub>, p<sub>n+1</sub>, and p<sub>n+2</sub>, predict the value of prime p<sub>n+3</sub>. We can see from the results given below that this is just a warm-up. These models clearly have no restraints when it comes to this problem, *however they should be tested with a larger prime series*.
 - [x] Random Forest   
     This model performs extremely well (R<sup>2</sup> > 0.9999) at predicting the next prime number in the series
 - [x] Decision Tree  
     DT is performing exceptionally well (R<sup>2</sup> > 0.9999) at predicting the next prime in the series
 - [x] Kernel Ridge Regression  
     KRR shows extremely high performance (R<sup>2</sup> > 0.9999), however there is a memory usage issue. KRR takes substantially longer than RF or DT. This should be investigated further.  
 - [ ] Deep Learning
 

### Factoring Primes
Given a product of two primes, predict the values of the factors.  This problem contains a few different scenarios:   
i) model has the product and a factor, can the algorithm can easily predict the other factor? and   
ii) model has only the product, can the algorithm predict the lower or upper factor with fair metrics?   
iii) Can we combine these two experiments (i.e. predict low factor, then use that prediction as the input for the prediction of the upper factor)?
 - [x] Random Forest  
   1) R<sup>2</sup> > 0.99  
   2) R<sup>2</sup> ~0.91 for both upper and lower factors
   3) R<sup>2</sup> ~0.74      
 - [x] Decision Tree  
   1) R<sup>2</sup> > 0.99  
   2) R<sup>2</sup> ~0.88 for lower factor and extremely poor performance for the upper factor
   3) R<sup>2</sup> ~0.73
## Resources
 - [ML for Factoring Primes](https://www.datasciencecentral.com/profiles/blogs/factoring-massive-numbers-a-new-machine-learning-approach)
 - [Scikit-Learn Supervised Learning](https://scikit-learn.org/stable/supervised_learning.html#supervised-learning)
