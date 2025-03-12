# Robust Portfolio Optimization with Rolling Window Analysis

## Introduction

This project explores portfolio optimization using the Modern Portfolio Theory (MPT) framework, incorporating robust covariance estimation and a rolling window approach for dynamic asset allocation.

## Motivation

Traditional MPT relies on sample covariance estimates, which can be noisy and unstable, especially with limited data or volatile assets. This project aims to address these limitations by employing a robust covariance estimation technique (Ledoit-Wolf) to enhance portfolio stability. Additionally, real-world markets are not stationary, prompting the use of a rolling window to re-estimate returns and covariance over time, better reflecting real-world rebalancing strategies.

## Critical Thinking Process

1. **Robust Covariance Estimation:** The Ledoit-Wolf shrinkage estimator is employed to mitigate the instability of sample covariance estimates, producing a more robust and reliable input for portfolio optimization.
2. **Rolling Window Analysis:** A rolling window approach is implemented to adapt to evolving market conditions. The covariance matrix and returns are re-estimated over time, simulating a dynamic rebalancing strategy.
3. **Asset Diversification:** The portfolio includes multiple asset classes (equities, bonds, commodities, and crypto) to illustrate the benefits of diversification in risk management.
4. **Efficient Frontier & Capital Market Line:** The project constructs the efficient frontier and identifies the maximum Sharpe ratio portfolio, visualizing the trade-off between risk and return and the optimal allocation.
5. **Transaction Cost Penalty:** A simple transaction cost penalty is introduced to account for the real-world costs associated with portfolio rebalancing.
6. **Comparison with Naive Portfolio:** The performance of the optimized portfolio is compared with a naive 1/N portfolio, highlighting the potential benefits of robust optimization.

## Observations

- The robust covariance estimation using Ledoit-Wolf significantly improves portfolio stability compared to traditional sample covariance estimates.
- The rolling window approach allows the portfolio to adapt to changing market conditions, leading to a more realistic and dynamic asset allocation strategy.
- The efficient frontier and maximum Sharpe ratio portfolio provide valuable insights into the risk-return trade-off and the optimal portfolio allocation.
- Introducing a transaction cost penalty provides a more realistic perspective on portfolio performance.
- The optimized portfolio consistently outperforms the naive 1/N portfolio in terms of risk-adjusted returns.

## Results

- **Improved Stability:** The Ledoit-Wolf shrinkage estimator demonstrably enhances portfolio stability, especially during periods of market volatility.
- **Dynamic Allocation:** Rolling window analysis allows for a more responsive and adaptive asset allocation strategy.
- **Enhanced Performance:**
    * The optimized portfolio, leveraging robust techniques and dynamic allocation, achieves an annualized return of **15.37%**, with an annualized volatility of **15.83%**, resulting in a Sharpe Ratio of **0.97**.
    * In comparison, the naive 1/N portfolio yields an annualized return of **9.35%**, with an annualized volatility of **15.33%**, leading to a Sharpe Ratio of **0.61**.
    * This highlights the significant outperformance of the optimized portfolio in terms of risk-adjusted returns.
- **Real-World Considerations:** Including a transaction cost penalty provides a more practical and realistic perspective on portfolio performance and management.

## Conclusion

This project provides a comprehensive analysis of robust portfolio optimization techniques, emphasizing the significance of adapting to market dynamics and incorporating real-world constraints. By combining robust covariance estimation, rolling window analysis, and thoughtful asset allocation, the project demonstrates the potential for enhancing portfolio performance and risk management.
