# VWCE Investment Analysis (Dollar Cost Averaging)

## Overview
This project analyzes a personal investment history in the VWCE ETF (Vanguard FTSE All-World UCITS ETF) to evaluate contribution patterns and the impact of Dollar Cost Averaging (DCA) on the weighted average cost.

## Business Questions
- Were contributions consistent over time?
- Which months had the highest investment volume?
- How did the weighted average price evolve?
- Did higher-price purchases significantly impact the final average cost?
- What is the impact of fees on the total invested amount?

## Dataset
Source: Manual extraction from Revolut trade confirmations (July–October 2025)

Columns:
- date
- contribution_eur
- shares
- unit_price_eur
- fee_eur
- time

## Method
- Data cleaning and standardization (dates, time, numeric formats)
- Net invested calculation (contribution - fee)
- Cumulative shares and net invested amount
- Weighted average cost over time
- Monthly aggregation of contributions
- Visualizations for contribution timeline and price evolution

## Key Results (Current Snapshot)
- Total contributed (gross): €2000
- Total fees: €7
- Total net invested: €1993
- Total shares: 14.442598
- Final weighted average cost: ~€137.99 per share

## Visuals
(Insert charts in /images and reference them here)

## Next Steps
- Add portfolio market value over time to compute unrealized P/L
- Compare VWCE performance vs a benchmark index
- Build a simple dashboard (optional)
