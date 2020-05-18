[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

>> The distribution of the PMF and CDF are both uniform. When you plot the PMF of a random number out of 1,000 the resulting plot is basically a rectangular box. All values from 0 to 1 (x axis) were valued at 0.001 (y axis) because of the equal probability percentages for each value, 1/1000. A CDF represents the probability accumulated by the random variable, so you add up all of the probabilities up to a specified point (i.e. 0-1,000). This generates a linear graph.


rand_num=np.random.random(1000)

rand_num_pmf=thinkstats2.Pmf(rand_num, label="number simulated")

thinkplot.Pmf(rand_num_pmf)

thinkplot.Config(xlabel='Number', ylabel='Count',)

rand_num_cdf=thinkstats2.Cdf(rand_num, label="number simulated")

thinkplot.Cdf(rand_num_cdf)

thinkplot.Config(xlabel='Number', ylabel='Count',)
