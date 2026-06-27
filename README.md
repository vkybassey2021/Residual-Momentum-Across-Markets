# Residual-Momentum-Across-Markets
Empirical asset pricing project comparing traditional, residual, and volatility-targeted momentum strategies in US and European equity markets.
# Residual Momentum Across Markets

## Project Overview

This project investigates whether residual momentum improves traditional momentum consistently across equity markets.

Residual momentum is designed to remove broad market exposure and rank stocks based on firm-specific performance. The expectation from the literature is that this should produce a cleaner and more reliable momentum signal.

This study tests that expectation in two markets:

* United States: S&P 500 constituents
* Europe: Stoxx 600 constituents

## Research Question

Does removing market exposure improve momentum in every market, or only in some?

## Strategies Compared

The project compares three momentum strategies:

1. Traditional momentum
2. Residual momentum using the Fama-French three-factor model
3. Volatility-targeted momentum

A robustness test also compares residual momentum using the Fama-French five-factor model.

## Key Findings

* Traditional momentum was profitable in both markets over each market's full sample.
* Residual momentum worked well in Europe but performed poorly in the United States.
* Matching both markets to the same 2006–2018 period did not reduce the gap; it widened it.
* In Europe, a positive residual momentum signal survived after removing market exposure.
* In the United States, the residual signal became weak, unstable, and statistically close to noise.
* Removing additional factors using the five-factor model improved the US result slightly, but did not make it profitable.

## Main Conclusion

Residual momentum is not universally better than traditional momentum. Whether removing market exposure helps or harms depends on the market where the strategy is applied.

## Tools Used

* R
* R Markdown
* Fama-French factor models
* Monthly equity return data
* Performance metrics: annualised return, annualised volatility, Sharpe ratio, and maximum drawdown

## Repository Contents

```text
.
├── report/
│   └── Residual_Momentum_Across_Markets.pdf
├── code/
│   └── analysis.Rmd
├── figures/
│   └── project_charts
└── README.md
```

## Note on Data

The analysis uses survivorship-free index constituent data for the S&P 500 and Stoxx 600. If the raw data is proprietary or restricted, it is not included in this repository.
