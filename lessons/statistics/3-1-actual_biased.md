[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)


constructs actual distribution using pmf function
~~~~
pmf = thinkstats2.Pmf(resp.numkdhh, label='numkdhh')
~~~~

constructs biased distribution using previously defined BiasPmf function
~~~~
biased_pmf = BiasPmf(pmf, label='observed')
~~~~

creates plot for actual distribution
~~~~
thinkplot.Pmf(pmf)
thinkplot.Config(xlabel='>18 years old in household', ylabel='Pmf')
~~~~

creates plot side by side
~~~~
thinkplot.PrePlot(2)
thinkplot.Pmfs([pmf, biased_pmf])
thinkplot.Config(xlabel='Class size', ylabel='PMF')

print('Actual mean', pmf.Mean())
print('Observed mean', biased_pmf.Mean())
~~~~
