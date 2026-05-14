# Superteam Birdeye Sprint 4 Submission Draft

## Title
Solana Token Radar with Safety Scoring

## Short description
A Birdeye-powered dashboard that scores trending Solana tokens by liquidity, volume, holder distribution, authority risk, and momentum so traders and agents can quickly separate watchable tokens from risky noise.

## Demo / repo
- Local build path: `output/birdeye_sprint4_demo`
- Build verified with `npm run build`
- Ready to push/deploy when final submission account is available.

## What I built
I built a React/Vite dashboard that integrates Birdeye's public API in live mode and includes a demo dataset for reviewers without a key. The dashboard fetches trending tokens, enriches them with token overview and token security data, then assigns each token a transparent risk score.

## Why it matters
Most new-token tools show momentum but hide risk. This app combines market activity with safety signals: liquidity depth, holder count, concentration, mint/freeze authority, and abnormal price movement. The goal is to help users avoid low-quality tokens before they waste time or capital.

## Birdeye endpoints used
- `/defi/token_trending`
- `/defi/token_overview`
- `/defi/token_security`

## Evaluation fit
- Product utility: clear first-pass token research workflow.
- Technical depth: multiple API calls per token + explicit scoring model.
- Presentation: polished UI, demo mode, README, and submission copy.
- Community support: can be paired with an X thread and screenshot.

## Next extensions
- Telegram alerts when a high-score token appears.
- Watchlist persistence.
- Historical score movement.
- Configurable scoring weights.
