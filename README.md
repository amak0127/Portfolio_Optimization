# Portfolio_Optimization
The idea is the fundamental concept of diversification and essentially boils down to the idea that pooling risky assets together, such that the combined expected return is aligned with an investor’s target, will provide a lower risk-level than carrying just one or two assets by themselves. The technique is even more effective when the assets are not well correlated with one another.


## Modern Portfolio Theory
Modern portfolio theory (MPT) is a theory on how risk-averse investors can construct portfolios to maximize expected return based on a given level of market risk. Harry Markowitz pioneered this theory in his paper "Portfolio Selection," which was published in the Journal of Finance in 1952.

Higher risk is associated with greater probability of higher return and lower risk with a greater probability of smaller return. MPT assumes that investors are risk-averse, meaning that given two portfolios that offer the same expected return, investors will prefer the less risky one. Thus, an investor will take on increased risk only if compensated by higher expected returns.

Modern portfolio theory says that it is not enough to look at the expected risk and return of one particular stock. By investing in more than one stock, an investor can reap the benefits of diversification — chief among them, a reduction in the riskiness of the portfolio.
What you need to understand is that “risk of a portfolio is not equal to average/weighted-average of individual stocks in the portfolio”. In terms of return, yes it is the average/weighted average of individual stock’s returns, but that’s not the case for risk. The risk is about how volatile the asset is, if you have more than one stock in your portfolio, then you have to take count of how these stocks movement correlates with each other. The beauty of diversification is that you can even get lower risk than a stock with the lowest risk in your portfolio, by optimising the allocation.

## Monte-Carlo Simulation
One approach to optimizing a portfolio is application of the Monte Carlo Method. For unfamiliar readers, this is the idea of carrying out repeated trials using randomly generated inputs and observing the outcomes. A physical example of this would be flipping a coin 100 times and counting the number of heads and tails. Based on the results, the observer could estimate whether the coin is fair or not. In the digital world, computers can rapid generate random numbers extremely quickly, enabling observation of outcomes from complex scenarios that are based on the probabilities of certain events occurring. The code below illustrates how simple it is to implement a Monte Carlo simulation using Python:

## Sharpe Ratio
The Sharpe ratio was developed by Nobel laureate William F. Sharpe and is used to help investors understand the return of an investment compared to its risk.1﻿﻿2﻿ The ratio is the average return earned in excess of the risk-free rate per unit of volatility or total risk. Volatility is a measure of the price fluctuations of an asset or portfolio.

Risk-adjusted return refines an investment’s return by measuring how much risk is involved in producing that return, which is generally expressed as a number or rating.

## Markowitz’s Efficient Frontier 

Based on the insights from Figure 1, it is evident that a target return can be achieved with a wide range of risk levels. This introduces the concept of the “Efficient Frontier.” The Efficient Frontier is the set of portfolios that achieve a given return with the minimum amount of risk for that return. In Figure 1, these were the portfolios furthest to the left for each expected return.

Keeping this concept in mind, a more structured approach can be applied to the selection of asset weights such that we consider only these efficient portfolios which meet a criteria important to the investor. First, she could optimize the weights to target a metric such as the Sharpe Ratio. Alternatively, the investor could opt to find the minimum volatility portfolio and accept the return that that provides. The code below consists of several helper functions that make use of SciPy’s optimization library to solve these two problems.

