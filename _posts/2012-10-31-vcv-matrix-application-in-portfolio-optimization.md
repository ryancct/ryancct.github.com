---
layout: post
title: "VCV Matrix 在Portfolio Optimization中的應用"
description: ""
category: Mathematics
tags: [Trading, Equity, Fundamental Analysis, Mathematics]
---
{% include JB/setup %}

如果想計算出Efficient Portfolio, 我們必須能夠運用資產的回報數據先計算出Variance-Covariance Matrix (VCV Matrix)。顧名思義，這Matrix包含了Asset自身的Variance及Asset與其他Asset之間的Covariance。Variance及Covariance這兩個measures都是尋找Efficient Portfolio時必需考慮的因素。

在數學層面，Variance及Covariance的Formula分別如下圖所示：

[![vcvdef](http://ryancheng.s3.amazonaws.com/Linear%20Programming/vcvdef.bmp)](http://stattrek.com/matrix-algebra/covariance-matrix.aspx)
Source: http://stattrek.com/matrix-algebra/covariance-matrix.aspx

事實上，在Excel亦有相應的function 可供用家使用的。請留意，Excel提供的Variance和Covariance的Formula是針對整個population size而不是整個sample size的。所以，它們的denominator都是N而不是N-1。若有需要使用sample size的Variance或Covariance，可自行乘以 N/(N-1) 調整。

在可接受的Portfolio Variance的情況下獲取最大的Portfolio Return 或以承擔最少的Portfolio Variance去賺取特定的Portfolio Return 是EF原理中Portfolio Optimization的目標。雖然VCV Matrix的結果會影響其Portfolio的Weighting，它的計算卻未能完美地解釋到Asset Return變化的原因。VCV Matrix在EF的Portfolio Optimization的應用上可能會出現大手的沽空盤或非現實可以完成的買入盤。另外，Asset之間在VCV Matrix的Correlation有時會過大或出現不合理的負數。例如，從1993年到2004年，Boeing與Kellogg的annual price correlation係 -0.1 (詳細計算方法請參考[附件](http://ryancheng.s3.amazonaws.com/Linear%20Programming/correl.xls))。這顯然是奇怪的。因為Boeing和Kellogg是屬於不同的板塊。因此Boeing股價上升的原因是很難解釋到為什麼Kellogg的股價會下跌。也許可勉強說這是蝴蝶效應吧。但這種關係是不明顯的。

筆者認為VCV Matrix的correlation是可以自行調整的。另外，大手的Large & Short Position亦可以用受到限制的。Financial Modeling的作者Simon Benninga對VCV Matrix的計算主要提出了三個alternatives。筆者不選擇在此詳談因認同作者在後續章節的說法，這三個問題都只能治標不能治本。不過，筆者認為不能因為上述的問題便斷言EF的Portfolio Optimization是沒有參考價值的。筆者建議VCV Matrix中的correlation是可以根據實際的情況自行調整而得出一個比較貼合Asset與Asset之間關係的adjusted correlation。另外，Simon在書中亦指出在Portfolio Optimization方面，Investors是可以accommodate其他的Position Limit，如沽空限制或所有Asset均不得多於百分之二十五的限制等等。

Reference:

Simon. B. (2008). Financial modeling. Cambridge, MA : MIT Press.
