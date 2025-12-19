# VWCE Investment Analysis (Dollar Cost Averaging)

## Overview
This project analyzes an investment transaction history for the VWCE ETF (Vanguard FTSE All-World UCITS ETF) with the goal of evaluating contribution behavior and the effectiveness of a Dollar Cost Averaging (DCA) strategy over time.

The focus of the analysis is not forecasting, but understanding how contribution timing, volume, and price variation affect the weighted average cost of the position.

## Business Questions
- Were contributions consistent over time?
- Which months concentrated the highest investment volume?
- How did the weighted average cost evolve after each contribution?
- Did purchases at higher prices negatively impact the final average cost?
- What is the impact of transaction fees on the total invested amount?

## Dataset
Source: Manual extraction from Revolut trade confirmations (July–October 2025).

Each record represents an individual purchase transaction.

Columns:
- date  
- contribution_eur  
- shares  
- unit_price_eur  
- fee_eur  
- time  

## Methodology
The analysis followed these steps:
- Data cleaning and standardization (date, time, numeric formats)
- Net invested calculation (contribution minus transaction fee)
- Cumulative invested amount and cumulative shares
- Weighted average cost calculation over time
- Monthly aggregation of contributions
- Exploratory visualizations to identify trends and patterns

## Key Results
- Total contributed (gross): €2,000  
- Total fees paid: €7  
- Total invested (net): €1,993  
- Total shares acquired: 14.442598  
- Final weighted average cost: approximately €137.99 per share  

## Insights
- The majority of capital was allocated within a lower price range (€134–€137), helping maintain the weighted average cost below recent market prices.
- Higher-price purchases had limited impact on the final average cost due to their smaller relative weight in the overall investment.
- Concentrated contributions during periods of higher capital availability contributed positively to cost stabilization over time.

## Visualizations
- Contribution timeline by transaction
- Unit purchase price vs. cumulative weighted average cost

(Charts generated using Python and stored in the `/images` directory.)

## Conclusion
The analysis indicates that the Dollar Cost Averaging strategy applied in this investment history was effective in managing price volatility and controlling the weighted average cost.

Maintaining consistent contributions, especially during periods of market fluctuation, can further strengthen the long-term efficiency of the strategy.

## Tools
- Python  
- Pandas  
- Matplotlib  
