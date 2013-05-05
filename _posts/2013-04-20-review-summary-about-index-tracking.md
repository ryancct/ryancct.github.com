---
layout: post
title: "review summary about index tracking"
description: ""
category: Trading
tags: [Trading, Equity]
---
{% include JB/setup %}

Index tracking aims to replicate the returns of a given index as closely as possible, by trading in various investment products.

This passive investment style is getting popular because, given that company research is not required and the target index composition is known, the total expense ratio (TER) is always lower compared to the active managed fund. Also, the Efficient Market Hypothesis (EMH) stated that equilibrium market prices fully reflect all available info, nothing can be done to systematically beat the market through active management. If EMH works, the index that represents the market is already the best strategy that investors should choose. In addition, Burton G Malkiel (2003) concluded in his paper that investors are likely to achieve for higher returns by employing a passive indexing strategy than they are likely to achieve from active portfolio management.

To perform index tracking, there are several replication strategies which can be adopted. They are full replication, optimization, stratified sampling, synthetic approach and Blended/Pragmatic approach. Among which, the full replication and optimization are very common. The performance of these replication strategies is determined by tracking error (TE) in finance. It is a measure of how closely a portfolio follows the index to which it is benchmarked. The method of calculating the TE varies, but the most common one is called the standard deviation of the active returns. It is caclulated based on root mean square (RMS) as shown below:

[![trackingerror]( http://ryancheng.s3.amazonaws.com/Linear%20Programming/trackingerror.jpg)](http://en.wikipedia.org/wiki/Tracking_error)

Source: http://en.wikipedia.org/w/index.php?title=Tracking_error&oldid=544329895

For full replication strategy, australian scholars explained that TE is related to index revisions, share issuances, spin-offs, share repurchases, index replication strategy itself and fund size. For optimization approach, scholars have conducted widely research on reducing TE to solve index tracking problems. One of the popular research is done by Nigel Meade & Gerald R. Salkin (1990). They suggested that the TE can be minimized by using a multivariate model that is formulated as a quadratic programme. One must choose an objective function that is an appropriate function for tracking error ie. The difference between portfolio return and the index return. On the other hand, this function should come along with the set of constraints imposed on the solution. E.g.: restriction on the positions on each asset or the number of assets selected in the portfolio, etc. In their paper, they discussed the portfolio performance by using not just TE, but also readustment policies, no. of shares, transaction costs and portfolio & index return difference. Other TE optimization methods include Genetic Algorithms for investment portfolio selection form J Shapcott (1992), Franesco Corielli (2002)'s Factor Based Index Tracking. Methods that extend the idea of quadratic programming include An evolutionary heuristic for the index tracking by Beasley et al (2002), differential evolution to solve constrained index tracking problems by Maringer (2008) and Threshold Accepting to obtain the portfolio compositions that track market index return from Gilli and Kelezi (2002).

Though many methods about TE optimization are suggested, Marshall E. Blume and Roger M. Edelen from the university of Pennsylvania indicated that it is virtually impossible to maintain tracking errors without holding all the stocks in proportion to the index in their 2002 paper "On replicating the S&P 500 index". They stressed that omitting even a few stocks can introduce unacceptable tracking errors. To conclude, the indexing objective is easy to understand but it is actually not a simple strategy and has little room for error.


Reference:

Passive management. (2013). In Wikipedia, The Free Encyclopedia. Retrieved from http://en.wikipedia.org/w/index.php?title=Passive_management&oldid=544027300

Malkiel. B. G. (2003). Passive Investment Strategies and Efficient Markets. Retrieved from http://www.ifa.com/Media/images/PDF%20files/Malkiel_PassiveInvestmentStrategiesandEf
ficientMarkets%20(2).pdf

Jin. Z., Maringer. D. (2009). Index Mutual Fund Replication. Retrieved from http://comisef.eu/files/Jin1.pdf

王偉丞. (2008). 增值指數基金績效分析-創新「多剖面調整」建構模型. 國立中山大學財務管理學系研究所.

Tracking error. (2013). In Wikipedia, The Free Encyclopedia. Retrieved from http://en.wikipedia.org/w/index.php?title=Tracking_error&oldid=544329895

Frino. A., Gallagher. D.R., Neubert. A. S. & Oetomo. T. N. (2001). Index Design and Implications for Index Tracking. Retrieved from http://wwwdocs.fce.unsw.edu.au/banking/workpap/wp9_03.pdf

Meade. N. & Salkin. G. R. (1990) Developing and Maintaining an Equity Index Fund. Journal of Operational Research Society. Vol. 41, No. 7, pp. 599-607.

Blume. M. E. & Edelen. R. M. (2002). On Replicating the S&P 500 Index. University of Pennsylvania. Retrieved from http://finance.wharton.upenn.edu/~rlwctr/papers/0208.pdf


