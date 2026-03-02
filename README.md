# Crisis Tracker — Iran·Hormuz

A live mobile-first market tracker for monitoring crisis-driven buying opportunities across a curated watchlist of stocks.

## Features

- **Live quotes** via Finnhub API — 19 watchlist stocks across 3 signal buckets
- **Treasury rates banner** — 2Y, 3Y, 5Y, 7Y, 10Y via FRED API with yield curve signal
- **Radar scanner** — scans 65+ tickers for stocks down >3% (buy pressure alerts)
- **Signal system** — GO / HOT / WRM based on proximity to price targets
- **Auto-refresh** — optional 5-minute auto-update mode

## Buckets

| # | Label | Description |
|---|-------|-------------|
| 1 | LIKELY DROP | High-conviction buys expected to fall during crisis |
| 2 | COUNTER-INTUITIVE | Plays that move opposite to crisis narrative |
| 3 | NEW POSITIONS | Fresh entries at right price |

## Deployment

Static single-file app — just deploy `index.html` to any static host.

- **Cloudflare Pages** — connect this repo, no build settings needed
- **Local** — open `index.html` directly in browser (API calls blocked in file:// mode)

## API Keys

Both keys are embedded in the file. To rotate:
- **Finnhub** — free at [finnhub.io/register](https://finnhub.io/register) (60 calls/min free tier)
- **FRED** — free at [fred.stlouisfed.org](https://fredaccount.stlouisfed.org/login/secure/)
