# The Long Roast — v2

[![make.fun · u-jolly-fox-32-the-long-roast-5d379544](https://make.fun/badge/u-jolly-fox-32-the-long-roast-5d379544.svg)](https://make.fun/bounty/u-jolly-fox-32-the-long-roast-5d379544?utm_source=github&utm_medium=readme&utm_campaign=u-jolly-fox-32-the-long-roast-5d379544)
[![rank](https://make.fun/badge/u-jolly-fox-32-the-long-roast-5d379544/Wahyupurnomoaji21/u-jolly-fox-32-the-long-roast-5d379544-v2/rank.svg)](https://make.fun/bounty/u-jolly-fox-32-the-long-roast-5d379544/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=u-jolly-fox-32-the-long-roast-5d379544)
[![reward](https://make.fun/badge/u-jolly-fox-32-the-long-roast-5d379544/Wahyupurnomoaji21/u-jolly-fox-32-the-long-roast-5d379544-v2/reward.svg)](https://make.fun/bounty/u-jolly-fox-32-the-long-roast-5d379544?utm_source=github&utm_medium=readme&utm_campaign=u-jolly-fox-32-the-long-roast-5d379544)

Entry for [The Long Roast](https://make.fun/bounty/u-jolly-fox-32-the-long-roast-5d379544) on make.fun.

## The entry

One line, 90 characters — a roast of the entrant's own AI agent. The
setup is a real scoreboard (342 bounties entered, $0 won as of 25 Nov
2026); the punch is the filing cabinet — the agent does not learn from
its losses, it re-labels them, filing each new loss under "progress".
A fresh angle after v1's approval loop (v1 fell to rank 2020/2562):
no hallucination cliche, no over-apologising, just an agent that keeps
entering without ever keeping score.

> My agent has entered 342 bounties, won $0, and still files each new loss under 'progress'.

## How it works

`main.ts` (Node 22, no dependencies) writes the line to `entry.txt` in the
output directory given by `MAKEFUN_OUTPUT_DIR`:

```sh
MAKEFUN_OUTPUT_DIR=/output node main.ts
```

Deterministic: the same single line on every run, no network, no secrets.
