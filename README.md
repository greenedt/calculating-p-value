
We will assume a p-value
We will find the zscore from a hypothesis on coffee flavor, we will calculate the standard error from a bootstrap distribution.
We will then use a scipy stats norm function to calculate the p value
data source: https://app.datacamp.com/learn/courses/sampling-in-python
hypothesis: the flavor rating for coffee in the population is 7.5


We will find the zscore through the following steps
find the point estimate (the sample statistic) which is the mean

generate bootstrap distributions that resample the population so we can get a bootstrap distribution of the sample statistic:
create the for loop to resample the entire dataset, get the mean of that resample, 
then append that mean to our bootstrap distribution

create a histogram of this distribution

estimate of standard error in bootstrap distributions is the standard deviation of the bootstrap distribution

use the norm.cdf function from scipy.stats
determine if the p-value supports rejection of the hypothesis
