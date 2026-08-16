# paper-trading-bot

Persistent state for an automated options paper-trading pipeline. No real trades are ever placed — this repo only stores a simulated portfolio ledger.

- `portfolio.json` — simulated cash balance, open positions, and trade history. Updated hourly (weekdays, market hours) by a scheduled cloud routine that reads live option quotes from Robinhood and records hypothetical fills here.
- Candidate tickers for each trading day come from the Robinhood "Setups" watchlist, populated each morning by a separate scheduled scan routine.
