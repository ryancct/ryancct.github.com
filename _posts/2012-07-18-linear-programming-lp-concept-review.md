---
layout: post
title: "linear programming (LP) concept review"
description: ""
category: Mathematics
tags: [Trading, Equity, Fundamental Analysis, Mathematics]
---
{% include JB/setup %}

筆者曾經在學校算術課了解過Linear Programming (LP)的原理及用途。而LP是筆者較有興趣鑽研的其中一個數學原理。因此，想藉此機會溫故知新及將一己所學所得在這裡跟大家分享一下。

LP是一種數學方法，其主要原理是在特定的約束條件之下計算出最優化(最大彧最小)的目標函數的結果。LP曾在WWII時被應用於軍事開支預算以減低軍用成本及增加敵軍的損失。起初，LP的原理是美軍的軍事機密。不過，George B. Dantzig則在1947年公開了LP的計算方法。之後，LP的表述便解決了許多營運上的實際問題如網路流或多商品流等等。另外，因為很多商業機構都希望解決收入極大化或成本極小化等的問題，LP亦因而經常大派用場。另外，LP的其他主要用途亦包括有效的資源調配。其數式的表達如下:

![resourcesallocation](http://ryancheng.s3.amazonaws.com/Linear%20Programming/resourcesallocatelpmathexpress.jpg)

�H�U�O�@��²�檺�Ҥl�H����LP formulation���Ӹ`:

E.g.:
���]�{�b���@���M���Ͳ��ѥ]�����q�A���s�@���Ƥ��O�O�ֽ��Υ������ؿ��ܡC�ѥ]�i�H�H�ֽ��Υ����s���C�t�~�A���m���ƪ��ܮw�i�H�e��50���窺���ơC�Ӥ��q�u�i�H�ϥΦ����ƶq�����u�u��(600�p��)�Υ[�u����(500����)�A�ӨC�@�ӥֽ��Υ����s�����ѥ]���ݭn���P�ƶq���u�ɤΥ[�u���Ƥ~���s���C�C�@�ӥֻs�ѥ]�ݭn45�u�@�p�ɩM60���窫�ơA�ӨC�@�ӥ����s�����ѥ]�h�ݭn30�u�@�p�ɩM45���窫�ơC�]�C�P���@�ӥֻs�ѥ]�M���s�ѥ]�����q�Q����150��100�䤸�A�h�Ӥ��q�����Q���D�i�H���ܬ��H�U��LP formulation:

Max P = 150X + 100Y, 
where Max P is the maximized profit, X is �ֻs�ѥ]���ƥ� and Y is ���s�ѥ]���ƥ�

Subject to.:
X + Y =< 50			(�ܮw�e�q����),
45X + 30X =< 600	(�u�ɭ���)
60X + 45Y =< 500	(�[�u���ƭ���)
X, Y => 0			(�����Ͳ��t�ƪ��ѥ]�ƶq)

�W�z���|���Ҥl�O�@�Ӹ�²�檺�Ҥl���K�j�a���աCLP�����άO�i�H�D�`�s�x�A�ӷ����ҳ]�����������M�i�H���h�A�⦡���i�H�������CŪ�Ѯɴ��A���̴����ѤF[Markowitz]( http://en.wikipedia.org/wiki/Harry_Markowitz)��the theory of portfolio choice. ����[efficient frontier (EF)]( http://en.wikipedia.org/wiki/Modern_portfolio_theory)���OLP���η������䤤�@�ӳ̨ΨҤl�C���Q�ΤFLP�����z���X���PAsset Class�Ҳ��ͪ��̨Χ����զX�C�o��theory���OMarkowitz�b1990�~�����FNobel Prize���C���̴��bŪ�Ѯɴ����էQ��excel��solver�i��LP formulation�A�չϹB��EF�����z�q�T�Ӥ��P�겣���O�����p���U�۩һݪ�Weighting�A�y�����X�̨Ϊ������զX�C���������N���~�һs��excel�ɮצb�����W[(click here)]( http://ryancheng.s3.amazonaws.com/Linear%20Programming/MPT.xls)�A�H�ѰѸԡC�L���N�t�A�����ԭz���������z�Ψ����p���ӫh�C

Reference:

Linear programming. (2012). In Wikipedia, The Free Encyclopedia. Retrieved from http://en.wikipedia.org/w/index.php?title=Linear_programming&oldid=512581944

Vanderbei. R. J. (2007). Linear Programming: Chapter 1 Introduction. Princeton University. Retrieved from http://www.princeton.edu/~rvdb/542/lectures/lec1.pdf


