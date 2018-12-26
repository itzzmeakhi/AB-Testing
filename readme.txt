 I got an error like AttributeError: module 'scipy.stats' has no attribute 'chisqprob' while importing scipy.stats module.

 So, i ran through a google search to come over this.

 In the link that i have provided in References, chisqprob is deprecated and removed from the scipy from 1.0.0, so there mentioned to use 0.19.0 environment or add the following line at the time of importing the module.

from scipy import stats
stats.chisqprob = lambda chisq, df: stats.chi2.sf(chisq, df)

So, by adding this i get over this error occured.

And when i have any doubt, i go through theexamples provided in the resources and videos of Udacity Nanodegree. 
