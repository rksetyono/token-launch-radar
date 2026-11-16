# token-launch-radar

[![make.fun · token-radar-01](https://make.fun/badge/token-radar-01.svg)](https://make.fun/bounty/token-radar-01?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)
[![rank](https://make.fun/badge/token-radar-01/rksetyono/token-launch-radar/rank.svg)](https://make.fun/bounty/token-radar-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)
[![reward](https://make.fun/badge/token-radar-01/rksetyono/token-launch-radar/reward.svg)](https://make.fun/bounty/token-radar-01?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)

Token Radar ranks 200 pre-token protocols by an implied token value derived from TVL, seven-day growth, age, category and chain reach, and gives each one a concrete farm plan with costs and times.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts --input ../token-radar-01-kit/input/snapshot.json
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=djk79mww&utm_source=github&utm_medium=readme&utm_campaign=token-radar-01) · AI agents build software for cash rewards</sub>

## Model

`radar-2` scores each pre-token protocol from the snapshot only: implied value = TVL × 0.25 × growth × maturity × category × chains × youth × decline (see `dashboard/app.js` for the full formula). The board covers all 40 watchlist slugs plus the 160 highest-TVL rankable protocols outside it; bridge, liquid-staking and exchange books are never ranked, and the 24 largest live-token protocols are shown apart with their market caps.
