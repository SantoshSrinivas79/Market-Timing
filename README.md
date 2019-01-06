# Market-Timing
Rewards of Perfect Market Timing

**_Timothy R. Mayes, Ph.D. (http://www.tvmcalcs.com)_**  
*1 January 2019*

*******
This code will calculate the rewards that can be had given great skill at market timing. It shows the value of a portfolio where the trader is good enough to be out of the market on the worst *N* days between the start and end dates. Obviously, this is not possible in reality, but it is interesting.

The impetus for this idea was [“The Truth About Timing,” by Jacqueline Doherty, Barron’s (November 5, 2001)](https://www.barrons.com/articles/SB1004756712494481760). In order to replicate those results, load the data and then call the `total_returns` function as:

```total_returns(data['1/1/1966':'10/29/2001'],5,invest=1).round(2)```

Actually, the exact dates that were used isn't clear. The chart in the article says that it starts in Feb 1966, but the table implies that it starts at the beginning of 1966 (3 January 1966). Also, there may be some slight rounding or data issues that cause the results here to vary a bit from the results reported in the Barron's article.

Finally, note that you can substitute your own data (different index or stock, different time frame, whatever), but this is probably best used if you have complete data for each calendar year. That is because the calculations drop the n worst/best days by calendar year.

Data is from [Yahoo! Finance](https://finance.yahoo.com/quote/%5EGSPC/history?period1=-631126800&period2=1546326000&interval=1d&filter=history&frequency=1d) as of 1 January 2019, and includes the daily adjusted close of the S&P 500 each day from 1 January 1950 to 31 December 2018.
![Reproduced Barron's Chart](https://github.com/mayest/Market-Timing/blob/master/Barrons%20Chart.jpg)

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mayest/Market-Timing/master)

