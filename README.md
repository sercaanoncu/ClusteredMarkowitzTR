# ClusteredMarkowitzTR

A fully automated, research-grade portfolio optimization workflow for BIST30 stocks, combining hierarchical clustering (correlation-based) and Markowitz efficient frontier theory.  
Scientific methods are used at each step to determine the number of clusters, representative stocks, and optimal portfolio weights.  
Outliers, missing data, and time alignment are robustly handled to ensure reproducibility and reliability.

## Features

- **Data Collection:** Pulls 10+ years of daily data for BIST30 stocks
- **Clustering:** Uses hierarchical clustering with distance = sqrt(2(1-corr)) for maximum sectoral diversification
- **Scientific Selection:** Number of clusters, cluster representatives, and portfolio size are all determined by data-driven algorithms (e.g., Silhouette Score, KneeLocator)
- **Portfolio Optimization:** Markowitz Efficient Frontier, Max Sharpe Ratio and Minimum Variance portfolio calculated with annualized returns and risk
- **Bias Handling:** Only stocks with complete data are used to avoid survivorship and lookahead bias
- **Full Automation:** No manual selection; all steps are fully automated and reproducible
