[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

~~~~

from scipy.stats import norm

~~~~

create function to convert feet/inches to centimeters

~~~~

def centimeters(ft, inch):
    return (ft * 12 + inch) * 2.54

~~~~

represent percentage of U.S. male population between 5'10 and 6'1 on the normal distribution applied to male height. 

~~~~

norm.cdf(centimeters(6, 1), 178, 7.7) - norm.cdf(centimeters(5 , 10), 178,7.7)


