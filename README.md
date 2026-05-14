# Birdeye Sprint 4 Token Radar

A Superteam Earn / Birdeye Data Sprint 4 demo that turns Birdeye's Solana market data into a practical token safety radar.

## What it does

- Fetches trending Solana tokens from Birdeye.
- Enriches each token with overview and security data.
- Scores liquidity, volume, holder count, top-holder concentration, mint/freeze authority risk, and momentum.
- Produces three buckets: high-confidence, watchlist, and risk-flagged.
- Tracks API calls locally so a builder can verify the 50+ call qualification threshold.
- Works in demo mode without a key, and live mode with a user-provided Birdeye API key.

## Why it is useful

New token discovery is noisy. This dashboard gives traders and agents a quick first-pass filter before spending time on deeper research. It is also easy to extend into Telegram/Discord alerts.

## Run locally

```bash
npm install
npm run dev
```

Open the app, paste a Birdeye API key locally, then click **Fetch live data**.

The key is stored only in browser localStorage and sent directly from the browser to Birdeye's public API.

## Build

```bash
npm run build
```

## Sprint 4 fit

- Uses Birdeye live endpoints: trending tokens, token overview, token security.
- Designed to exceed the 50 API call minimum during normal exploration.
- Delivers a real onchain utility, not just a static page.
- Agent-friendly scoring logic can be reused in bots and alerts.
