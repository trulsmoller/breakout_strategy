# Breakout Strategy
## by Truls Møller

### Date created
2021-09-15

## Summary
Breakout Strategy is the second project delivery of Udacity's Nano-degree program: AI for Trading

The hypothesis:

- In the absence of news or significant investor trading interest, stocks oscillate in a range.
- Traders seek to capitalize on this range-bound behaviour periodically by selling/shorting at the top of the range and buying/covering at the bottom of the range. This behaviour reinforces the existence of the range.
- When stocks break out of the range, due to, e.g., a significant news release or from market pressure from a large investor:
- the liquidity traders who have been providing liquidity at the bounds of the range seek to cover their positions to mitigate losses, thus magnifying the move out of the range, and
- the move out of the range attracts other investor interest; these investors, due to the behavioural bias of herding (e.g., Herd Behavior) build positions which favor continuation of the trend.

## Results
I was able to implement the breakout strategy in a number of steps (functions):
- Compute highs and lows in a lookback window
- Compute long and short signals
- Filter signals
- Compute signal returns
- Test for significance with outliers
- Using the Kolmogorov-Smirnov Test to remove outliers
- Test for significance without outliers

There was no clear indication of a profitable strategy even with outliers removed. However I was able to implement as intended.

## Files
- project_2_starter.ipynb - Notebook with the code for this project
- close.csv - daily close prices
- high.csv - daily high prices
- low.csv - daily low prices
