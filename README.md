# Monte Carlo simulation weighted with Sentiment scores from news data to determine Call and Put Prices

> Thesis pdf link: https://github.com/gaurav-95/Thesis---Monte-Carlo-Options-using-Sentiment/blob/main/UMDS19001_Gourab_Thesis_MonteCarlo.pdf
 
<img src="https://github.com/gaurav-95/Thesis---Monte-Carlo-Options-using-Sentiment/blob/main/Images/mcsent.png"> 

<img src="https://github.com/gaurav-95/Thesis---Monte-Carlo-Options-using-Sentiment/blob/main/Images/scape.png"> 

## Abstract — 
Investor sentiment affects the ups and downs of a
stock according to many previous studies. In this study I produce
an empirical method of pricing stock options using sentiment
weights in the way that they are less dependent on rigid measures
that are used in models like Black Scholes model. Also they are
not as unreliable as a traditional Monte Carlo Simulation model.
I introduce sentiment weights into the picture in order to reign
in on the randomness created by the Monte Carlo simulation.
Which helps create a more consistent yet dynamically obtained
call and put option pricing. As apart of previous research, I had
also seen the effects of sentiments playing a role in the market
value of a stock. The weights generated from that previous study
is used here with to base the Monte Carlo Simulation on. I see
the sentiment inputs provide great potential for option pricing
improvements.

Dataset scraped from finviz.com:

## Approach:

1. Generate sentiment scores from news data scraped from finviz.com for US Stocks.

2.  Use sentiment scores as weights for portfolio assignment.

3. Perform Monte Carlo simulation to predict for the portfolio based on sentiment weights rather than random weights.

## Conclusions:

Clearly sentiments can be a good way to obtain
daily/weekly/monthly adjusted dynamic portfolios. Rather
than coming up without any intuition of assigning weights
to the portfolio, it is useful to have the sentiment scores
calculated as a reflection of recent trends of the stock market.
Over a longer period of time, it becomes harder to obtain news
data and so it also has its limitations. Also in my case I am
limited to only obtaining seven days of ticker data and less than
half a month of news data. But given that news can reflect up
to 20 days of stock price it is manageable.Options pricing that
are traditionally defined can be looked at a different light after
considering the results I obtain after testing out the methodology
that I propose in order to determine call option prices
and put option. This initial study does not show the result of
doing random weight simulation multiple times. Which when
performed will show the consistency of the Sentiment Monte
Carlo model vs. the Random Monte Carlo simulation which
will not change depending on the weight-age of the stocks
rather be dependent on getting multiple simulations across
multiple random weights which makes it computationally a
heavy task even for today’s computers.I run only 4 stocks here.
But in real life. A single portfolio can contain over 30stocks.
Running a single instance of sentiment weight will be more
feasible rather than25 7. Conclusion running multiple instances
of random weights. Further granular applications of the same
need to be performed in future. Right now it is using the
average score obtained from a particular day. In future the
hourly or 30 minute data intervals can be utilized to create
further variations for predictions in a shorter time frame than
what is used now.


REFERENCES

- [1] Z. Ben Ami and R. Feldman, “Event-based trading: Building superior
trading strategies with state-of-the-art information extraction tools,”
Available at SSRN 2907600, 2017.
- [2] L. A. Smales, “The importance of fear: investor sentiment and stock
market returns,” Applied Economics, vol. 49, no. 34, pp. 3395–3421,
2017.
- [3] P. Hafez and J. Xie, “Web news analytics enhance stock portfolio
returns,” Available at SSRN 2423362, 2014.
- [4] W. S. Leung, G. Wong, and W. K. Wong, “Social-media sentiment,
portfolio complexity, and stock returns,” Portfolio Complexity, and Stock
Returns (November 24, 2019), 2019.
- [5] D. de Franc¸a Costa and N. F. F. da Silva, “Inf-ufg at fiqa 2018 task
1: predicting sentiments and aspects on financial tweets and news
headlines,” in Companion Proceedings of the The Web Conference 2018,
2018, pp. 1967–1971.
- [6] C.-J. Wang, M.-F. Tsai, T. Liu, and C.-T. Chang, “Financial sentiment
analysis for risk prediction,” in Proceedings of the Sixth International
Joint Conference on Natural Language Processing, 2013, pp. 802–808.
- [7] M. S. Akhtar, A. Kumar, D. Ghosal, A. Ekbal, and P. Bhattacharyya,
“A multilayer perceptron based ensemble technique for fine-grained
financial sentiment analysis,” in Proceedings of the 2017 conference on
empirical methods in natural language processing, 2017, pp. 540–546.
- [8] N. C. Dang, M. N. Moreno-Garc´ıa, and F. De la Prieta, “Sentiment
analysis based on deep learning: A comparative study,” Electronics,
vol. 9, no. 3, p. 483, 2020.
- [9] A. Martin-Utrera, “Shrinking against sentiment: Exploiting behavioral
biases in portfolio optimization,” Available at SSRN 3551224, 2020.
- [10] H. K. Sul, A. R. Dennis, and L. Yuan, “Trading on twitter: Using social
media sentiment to predict stock returns,” Decision Sciences, vol. 48,
no. 3, pp. 454–488, 2017.
- [11] A. Bandopadhyaya, A. L. Jones et al., “Measures of investor sentiment:
A comparative analysis put-call ratio vs. volatility index,” Journal of
Business & Economics Research (JBER), vol. 6, no. 8, 2008.
- [12] M. Baker and J. Wurgler, “Investor sentiment in the stock market,”
Journal of economic perspectives, vol. 21, no. 2, pp. 129–152, 2007.
- [13] C. Yang, B. Gao, and J. Yang, “Option pricing model with sentiment,”
Review of Derivatives Research, vol. 19, no. 2, pp. 147–164, 2016.
- [14] R. Hao, “Option pricing model with investor sentiment,” 2017.
- [15] B. Han, “Investor sentiment and option prices,” The Review of Financial
Studies, vol. 21, no. 1, pp. 387–414, 2008.
