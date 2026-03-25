# Historical VaR—Market Risk Analysis
*Python | pandas | numpy | matplotlib*

## Overview
This project implements a Historical Value at Risk (VaR) model 
on a French insurance and banking portfolio. It was built to 
apply market risk concepts from my work as a Financial Analyst 
at BNP Paribas Cardif.

## Portfolio
| Asset | Ticker | Sector |
|-------|--------|--------|
| BNP Paribas | BNP.PA | Banking |
| AXA | CS.PA | Insurance |
| SCOR | SCR.PA | Reinsurance |

> Portfolio chosen intentionally to reflect the French insurance 
> and banking sector, directly aligned with my professional experience.

## Methodology
- **Method**: Historical VaR (non-parametric)
- **Period**: January 2022 – December 2025 (1,021 daily observations)
- **Confidence levels**: 95% and 99%
- **Data source**: Yahoo Finance via yfinance

## Key Results
| Asset | VaR 95% | VaR 99% |
|-------|---------|---------|
| BNP.PA | -2.79% | -5.18% |
| CS.PA | -2.04% | -4.31% |
| SCR.PA | -2.93% | -5.91% |

> SCOR shows the highest tail risk at -5.91% (VaR 99%), 
> consistent with its exposure to catastrophic reinsurance events.

## What This Means
- **VaR 95% BNP = -2.79%** → 95% of the time, 
BNP does not lose more than 2.79% in a single day
- **VaR 99% SCOR = -5.91%** → in the worst 1% of days, 
SCOR can lose more than 5.91%

## Files
- `VaR_Historique.ipynb` — main notebook
- `VaR_Historique.png` — distribution charts with VaR thresholds

## Libraries
```
yfinance | pandas | numpy | matplotlib
```

## Author
Raniya Sirat — Financial Analyst @ BNP Paribas Cardif  
CFA Level I Candidate | MSc Sustainable Financial Management  
[LinkedIn](https://www.linkedin.com/in/raniya-sirat)
