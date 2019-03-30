# Ontogenetic Dietary Shift with Bayesian Estimation in PyMC3

This is an application of the Bayesian estimation on stable isotope data investigating the ontogenetic dietary shift in Indo-Pacific humpback dolphins using stable isotope data, using the PyMC3 package. The idea behind is that individual heterogeneity was commonly neglected and the whole population data was pooled together to perform modelling. In the real world, individual ontogenetic development can differ and progress at a different rate (i.e. the rate of diet shifting). The difference in dietary shifting is governed by a hyperparameter that overlook the individual developmental parameters - intercept (SIA level at birth), pre-weaning rate and post-weaning rate. 

This repository showcase the following components:
1. Data clean up
2. Data Visualization
3. Complete pooling
4. Hierarchical model
5. Multilevel Hierarchical Model - with Regional & Sexual Difference

### Conventional approaches
The two conventional alternatives to modeling radon exposure represent the two extremes of the bias-variance tradeoff:

Complete pooling:
Treat all individuals the same, and estimate a single intercept, pre-weaning rate and post-weaning rate.

No pooling:
Model intercept, pre-weaning rate and post-weaning rate for each individual independently.

>```python
    from IPython.core.pylabtools import figsize
    import numpy as np
    import pandas as pd
```

![alt text](https://raw.githubusercontent.com/YuenWaHo/pymc3_weaning/master/examples/posterior.png?token=Af9kMPIvdz2tQJP1x60zlKT-nZmca54zks5cnv-XwA%3D%3D "Posterior Distribution of Parameters")
