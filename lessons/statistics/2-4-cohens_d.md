[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)




'''
first_hist = thinkstats2.Hist(firsts.birthwgt_lb, label='first')
other_hist = thinkstats2.Hist(others.birthwgt_lb, label='other')

width = 0.45
thinkplot.PrePlot(2)
thinkplot.Hist(first_hist, align='right', width=width)
thinkplot.Hist(other_hist, align='left', width=width)
thinkplot.Config(xlabel='weeks', ylabel='Count', xlim=[0, 16])
'''
