# Market Making & Risk Control in MSFT Options (Python)

This repository contains the deliverables for a group project on equity-options market making and market risk control.  
We construct a delta-hedged options portfolio on **Microsoft (MSFT)** using a mix of **listed** and **OTC** options and assess the portfolio’s risk under a market-making framework.

## Objectives
- Build and monitor a **delta-neutral** market-making portfolio (options + underlying hedge)
- Analyse P&L drivers (e.g., **gamma/vega** exposure) and dynamic hedging effects
- Implement a market risk framework with:
  - **Sensitivities / Greeks**
  - **5-day VaR (95%)** and **5-day Expected Shortfall (97.5%)** via Monte Carlo
  - **Stress testing** with historical and hypothetical scenarios
  - Limit structure (global + granular) and limit-usage monitoring

## Methodology (high level)
1. Portfolio construction: listed and OTC options on MSFT + delta hedging with the underlying
2. Risk measurement: Monte Carlo simulation for VaR/ES over a 5-day horizon
3. Stress testing: predefined scenarios to identify tail risks and potential breaches
4. Reporting: summary outputs suitable for risk-committee style review

## Repository structure
- `report/` – Final report and/or presentation
- `data/` – Input data used for the analysis (if shareable)
- `notebooks/` – Jupyter notebooks (analysis workflow)
- `src/` – Python modules/functions (pricing, simulation, risk metrics)
- `outputs/` – Figures, tables and intermediate results

## Key results (summary)
- Delta hedging reduces first-order exposure but leaves meaningful second-order risks (gamma/vega)
- VaR/ES and stress tests highlight tail-risk sensitivity to volatility/spot shocks
- Granular limits improve control of concentration risks across option positions

## Requirements
- Python 3.x
- Common libraries: numpy, pandas, scipy, matplotlib (and any others you used)

## How to run
1. Clone the repository
2. (Optional) Create a virtual environment
3. Run the notebooks in `notebooks/` in order, or execute scripts in `src/`  
(Names can be added here if agreed with the team.)

