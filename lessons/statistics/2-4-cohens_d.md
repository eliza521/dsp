[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

>> 0.0289

firsts = live[live.birthord == 1]
others = live[live.birthord != 1]
preglen_first=firsts.prglngth 
preglen_other=others.prglngth
CohenEffectSize(preglen_first, preglen_other)
