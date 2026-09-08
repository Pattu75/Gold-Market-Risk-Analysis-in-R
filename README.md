Gold Market Risk Analysis in R

Returns, Tail Risk, Simulation, and GARCH Volatility

Author: Zakariya Boutayeb

Instrument: COMEX gold futures (GC=F)

Analysis period: December 2006 through December 2023


Summary:

This report evaluates gold-market risk using daily Yahoo Finance closing prices. It combines return construction, distribution diagnostics, parametric and empirical tail estimation, multi-day simulation, autocorrelation analysis, and a GARCH(1,1) model with Student-t innovations.

Four conclusions emerge:

- Gold returns are negatively skewed and heavy-tailed;
- Empirical tail losses are more severe than normal-model estimates;
- Return direction has little serial dependence while volatility clusters strongly;
- and conditional volatility is highly persistent.
  
Although the fitted GARCH model is informative, its stability and sign-bias diagnostics show that it should not be treated as a complete production model.

Research questions:

- How should gold returns be constructed across different horizons?
- How sensitive are VaR and ES to distributional assumptions?
- Does Student-t modeling improve the representation of tail risk?
- Does preserving the order of returns change 10-day risk estimates?
- Can a GARCH model explain the observed volatility clustering?
- What weaknesses remain after fitting GARCH?

Project Highlights:

- Construct daily and calendar-period returns correctly.
- Diagnose skewness, heavy tails, serial correlation, and volatility clustering.
- Estimate one-day 99% VaR and ES under several distributional approaches.
- Compare three 10-day simulations.
- Estimate a GARCH(1,1)-t model and bootstrap its one-day 95% tail risk.

Data and sample:

- Instrument: continuous COMEX gold futures (GC=F)
- Field: Yahoo Finance daily closing price
- Requested range: 2006-12-31 through 2023-12-31
- 4,275 usable daily log returns.

The instrument is a continuous gold futures series rather than physical spot gold. Futures can differ from spot because of carrying costs, contract maturities, and the method used to join successive contracts.

