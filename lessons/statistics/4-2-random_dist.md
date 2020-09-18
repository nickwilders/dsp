[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)


This establishes the random sample of 1,000 numbers between 0 and 1

~~~~
random_numbers = np.random.random_sample(1000)
~~~~

Creates the pmf, prepares to be graphed, and initiates histogram

~~~~
random_pmf = thinkstats2.Pmf(random_numbers)
thinkplot.Hist(random_pmf)
thinkplot.Config(xlabel='Number value', ylabel='PMF')
~~~~

This returns a single value or blank graph. PMF would count the number of instances of a particular value. In a truly random set of numbers, a duplicate is highly unlikely, so a PMF is an inefficient way to represent the data.

~~~~
random_cdf = thinkstats2.Cdf(random_numbers)
thinkplot.Cdf(random_cdf)
thinkplot.Config(xlabel='number value', ylabel='CDF')
~~~~

This distribution is successfully plotted, and is uniform. 
