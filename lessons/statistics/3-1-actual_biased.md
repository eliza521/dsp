[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

>> Actual mean 1.024

>> Biased mean 2.024

resp = nsfg.ReadFemResp()

numkid=resp.numkdhh

copy_numkid=numkid.copy()

new_numkid=copy_numkid.add(1)

new_numkid.head()

new_numkid_pmf = thinkstats2.Pmf(new_numkid, label='biased')

numkid_pmf = thinkstats2.Pmf(numkid, label='actual')

thinkplot.PrePlot(2)

thinkplot.Pmfs([numkid_pmf, new_numkid_pmf])

thinkplot.Config(xlabel='How Many Kids', ylabel='Percentage of Whole',)

print('Actual mean', numkid_pmf.Mean())

print('Biased mean', new_numkid_pmf.Mean())
