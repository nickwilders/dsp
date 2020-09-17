[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

### First, I completed a histogram comparing the two values: 

~~~~
first_hist = thinkstats2.Hist(firsts.birthwgt_lb, label='first')
other_hist = thinkstats2.Hist(others.birthwgt_lb, label='other')

width = 0.45
thinkplot.PrePlot(2)
thinkplot.Hist(first_hist, align='right', width=width)
thinkplot.Hist(other_hist, align='left', width=width)
thinkplot.Config(xlabel='weeks', ylabel='Count', xlim=[0, 16])
~~~~
### Then, I found the Cohen Effect Size, which was equal to -0.10. The Cohen Effect Size
### for pregnancy length, by comparison, is 0.02. 
~~~~
CohenEffectSize(firsts.birthwgt_lb, others.birthwgt_lb)
CohenEffectSize(firsts.prglngth, others.prglngth)
~~~~
### We previously concluded that pregnancy length is not strongly correlated to first-
### term babies in either direction. There is a somehwat stronger correlation for 
### birth weight, supporting an observation that non-first babies are often heavier
### than first babies. 
