---
layout: post
title: "linear programming (LP) concept review"
description: ""
category: Mathematics
tags: [Trading, Equity, Fundamental Analysis, Mathematics]
---
{% include JB/setup %}

筆者曾經在學校算術課了解過[Linear Programming (LP)](http://en.wikipedia.org/wiki/Linear_programming)的原理及用途。而LP是筆者較有興趣鑽研的其中一個數學原理。因此，想藉此機會溫故知新及將一己所學所得在這裡跟大家分享一下。

LP是一種數學方法，其主要原理是在特定的約束條件之下計算出最優化(最大彧最小)的目標函數的結果。LP曾在WWII時被應用於軍事開支預算以減低軍用成本及增加敵軍的損失。起初，LP的原理是美軍的軍事機密。不過，[George B. Dantzig]( http://en.wikipedia.org/wiki/George_Dantzig)則在1947年公開了LP的計算方法。之後，LP的表述便解決了許多營運上的實際問題如網路流或多商品流等等。另外，因為很多商業機構都希望解決收入極大化或成本極小化等的問題，LP亦因而經常大派用場。另外，LP的其他主要用途亦包括有效的資源調配。其數式的表達如下:

![resourcesallocation](http://ryancheng.s3.amazonaws.com/Linear%20Programming/resourcesallocatelpmathexpress.png)

以下是一個簡單的例子以說明LP formulation的細節:

E.g.:
假設現在有一間專門生產書包的公司，其製作原料分別是皮質或布質兩種選擇。書包可以以皮質或布質製成。另外，放置原料的倉庫可以容納50公斤的原料。該公司只可以使用有限數量的員工工時(600小時)及加工物料(500公斤)，而每一個皮質或布質製成的書包都需要不同數量的工時及加工物料才能製成。每一個皮製書包需要45工作小時和60公斤物料，而每一個布質製成的書包則需要30工作小時和45公斤物料。設每銷售一個皮製書包和布製書包的公司利潤為150及100港元，則該公司的營利問題可以表示為以下的LP formulation:

Max P = 150X + 100Y, 
where Max P is the maximized profit, X is 皮製書包的數目 and Y is 布製書包的數目

Subject to.:
X + Y =< 50			(倉庫容量限制),
45X + 30X =< 600	(工時限制)
60X + 45Y =< 500	(加工物料限制)
X, Y => 0			(不能生產負數的書包數量)

上述所舉的例子是一個較簡單的例子方便大家明白。LP的應用是可以非常廣泛，而當中所設約束條件當然可以更多，算式亦可以更複雜。讀書時期，筆者曾見識了[Markowitz]( http://en.wikipedia.org/wiki/Harry_Markowitz)的the theory of portfolio choice. 當中[efficient frontier (EF)]( http://en.wikipedia.org/wiki/Modern_portfolio_theory)更是LP應用當中的其中一個最佳例子。它利用了LP的原理找出不同Asset Class所產生的最佳投資組合。這個theory更令Markowitz在1990年獲取了Nobel Prize的。筆者曾在讀書時期嘗試利用excel的solver進行LP formulation，試圖運用EF的原理從三個不同資產類別之間計算各自所需的Weighting，籍此找出最佳的投資組合。筆者顯醜將當年所製的excel檔案在此附上[(click here)]( http://ryancheng.s3.amazonaws.com/Linear%20Programming/MPT.xls)，以供參詳。他日將另再撰文詳述相關的原理及具體計算細則。

Reference:

Linear programming. (2012). In Wikipedia, The Free Encyclopedia. Retrieved from http://en.wikipedia.org/w/index.php?title=Linear_programming&oldid=512581944

Vanderbei. R. J. (2007). Linear Programming: Chapter 1 Introduction. Princeton University. Retrieved from http://www.princeton.edu/~rvdb/542/lectures/lec1.pdf


