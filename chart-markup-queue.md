# Chart Markup Queue

Written by the "Daily Options Scan (Cloud)" routine each weekday morning. Each entry records the EXACT numeric levels needed to redraw that day's confluences on TradingView later — since the cloud routine has no TradingView access itself. When you're next at your laptop with a local Claude Code session open, just ask to "draw the queued setups" (or similar) and the exact levels below get replayed onto TradingView via draw_shape, then marked `drawn: yes` so they aren't redrawn. Entries may pile up across multiple days if you're away — that's fine, all undrawn entries get replayed in one pass.

Format per entry:

```
## YYYY-MM-DD — TICKER (drawn: no)
- Horizontal line (support): $XX.XX
- Horizontal line (resistance, if any): $XX.XX
- Trendline (if any): from (YYYY-MM-DD, $XX.XX) to (YYYY-MM-DD, $XX.XX)
- 50-SMA: $XX.XX | 200-SMA: $XX.XX
- Text label: short confluence note to place on chart
```
