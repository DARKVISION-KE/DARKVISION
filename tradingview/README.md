# XAUUSD AMD Strategy for TradingView

Open `XAUUSD_AMD_Supply_Demand.pine` in TradingView's Pine Editor and add it to a 5-minute XAUUSD chart.

The script combines confirmed 1H/4H EMA bias and swing-candle supply/demand zones, a 15-minute compressed-range sweep cue, and a 5-minute structure-break/displacement confirmation. It plots prior-day dPOC/dVAH/dVAL estimates as context and calculates risk-based estimated order size, stop, and three R-multiple targets.

## Data and sizing notes

- The prior-day profile is an approximation. It assigns each chart candle's entire volume to the bin containing its `hlc3` price. XAUUSD volume is feed-specific and may represent tick volume rather than centralized traded volume.
- Supply/demand zones are pivot-candle approximations and require the configured right-side bars to confirm.
- Position sizing assumes USD account currency and 100 ounces per standard lot. Confirm your TradingView symbol and broker quantity conventions before using strategy results.
- The strategy is an analysis and backtesting tool, not a guarantee of results. Apply realistic commission, spread, and slippage settings before evaluating it.

