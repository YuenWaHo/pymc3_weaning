# Ontogenetic Dietary Shift with Bayesian Estimation in PyMC3

This is an application of the Bayesian estimation on stable isotope data investigating the ontogenetic dietary shift in Indo-Pacific humpback dolphins using stable isotope data, using the PyMC3 package. The idea behind is that individual heterogeneity was commonly neglected and the whole population data was pooled together to perform modelling. In the real world, individual ontogenetic development can differ and progress at a different rate (i.e. the rate of diet shifting). The difference in dietary shifting is governed by a hyperparameter that overlook the individual developmental parameters - intercept (SIA level at birth), pre-weaning rate and post-weaning rate. 

This repository showcase the following components:
1. Data clean up
2. Data Visualization
3. Complete pooling
4. Hierarchical model
5. Multilevel Hierarchical Model - with Regional & Sexual Difference

Trial2

### Conventional approaches
The two conventional alternatives to modeling radon exposure represent the two extremes of the bias-variance tradeoff:

Complete pooling:
Treat all individuals the same, and estimate a single intercept, pre-weaning rate and post-weaning rate.

                                  𝑦𝑖∼Normal(𝛼+𝛽𝑥𝑖+𝜖𝑖),𝑟𝑡={preweaning_rate, postweaning_rate,if 𝑡≤𝑠if 𝑡>
                                                           
No pooling:
Model intercept, pre-weaning rate and post-weaning rate for each individual independently.

                                                            𝑦𝑖=𝛼𝑗[𝑖]+𝛽𝑥𝑖+𝜖𝑖   where 𝑗=1,…,n
