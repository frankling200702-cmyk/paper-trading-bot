# Trade Journal

Human-readable log of every simulated trade (open or close), written by the "Hourly Paper Trading (Cloud)" routine alongside its update to `portfolio.json`. This is the readable companion to `trade_history` in that file.

Format per entry:

```
## YYYY-MM-DD HH:MM ET — TICKER — OPEN/CLOSE
- Contract: TICKER $STRIKE CALL/PUT exp YYYY-MM-DD
- Price: $X.XX x N contracts
- Why: one or two sentences on the setup/trigger (entry) or the reason for exiting (target/stop/expiration/thesis change)
- Cash after: $X,XXX.XX
```
