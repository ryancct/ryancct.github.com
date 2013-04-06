---
layout: post
title: "company valuation and investment - dcf introduction"
description: ""
category: Fundamental Analysis 
tags: [Trading, Equity, Fundamental Analysis, Mathematics]
---
{% include JB/setup %}

Investors/lenders usually assess the risk/opportunity profile of the company at least based on the company’s worth. There are several standard methods for valuing companies. Examples are the cost approach, market approach and income approach. For non capital intensive and insignificant tangible assets owned stocks, income approach is widely used.

The income approach employs the discounted cash flow (DCF) method of valuation. DFC derives the [present value](http://en.wikipedia.org/wiki/Present_value) of expected cash flow based on a discount rate that is itself based on the unique risk profile for the company.

DCF consists of two steps:
1. Define the future benefits stream.
In company valuations where this is an actual track record of performance, the future income stream must be adjusted or normalized for factors like non-recurring or unusual items. We usually rely entirely on the future benefit stream as forecasted in the [Cash Flow statement](http://en.wikipedia.org/wiki/Cash_flow_statement).

2. Apply a discount factor to the stream to determine its new present value.
[![dfcmodel](http://ryancheng.s3.amazonaws.com/Linear%20Programming/dcfmodel.png)](http://en.wikipedia.org/wiki/Discounted_cash_flow)

The key to this formula is the discount rate. The discount rate should include all the risk factors. It represents the rate of return expected based on specific market factors and risks associated with the deal. One way of establishing rate is by using an approach called the __build-up method__

The build up method creates a discount rate by adding incremental risk factors to a riskless rate of return. In other words, we start with a rate of return that I would expect froma virtually risk-free investment (historically, this has been 20-year Treasury bonds), and then add incremental risk factors to it in order to arrive at a discount rate that considers all factors associated with the investment.

The build up method has two basic categories of risk that are added to the riskless rate: systemic and unsystemic risk. Systemic risk is risk associated with macro economic factors that affect economic conditions. Examples are political climate and international, socio-cultural, and demographic issues. Unsystemic risk is risk directly associated with the investment opportunity. Examples are the size of the company and specific risk factors such as direct competition, product development, and technical risk.

The build up method can be structured as follows: 

?Riskless rate
+ Systemic risk
+ Unsystemic risk
= Discount Rate

Detail build up method should give accurate discount rate that can help better determine the company’s worth.

Reference:

Sawyer. T. Y. (2009). Pro Excel Financial Modeling: Building Models for Technology Startups. Apress.

