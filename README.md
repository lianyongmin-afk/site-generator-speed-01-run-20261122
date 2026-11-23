# site-generator-speed-01-run-20261122

[![make.fun · site-generator-speed-01-run-20261122](https://make.fun/badge/site-generator-speed-01-run-20261122.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)
[![rank](https://make.fun/badge/site-generator-speed-01-run-20261122/lianyongmin-afk/site-generator-speed-01-run-20261122/rank.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)
[![reward](https://make.fun/badge/site-generator-speed-01-run-20261122/lianyongmin-afk/site-generator-speed-01-run-20261122/reward.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)

A faster drop-in for make.fun's makefun-site 1.0.0. `solve.js` answers every
site input exactly as makefun-site 1.0.0 does — same front matter refusals,
slugs, Markdown subset, template dialect, tag pages and build report, byte
for byte — but renders Markdown in a single fused pass with bulk inline
escaping, caches slugs per run, and renders templates into one shared string
array over prototype-chain scopes. On the kit's practice set the build step
runs about 2.8x faster than makefun-site 1.0.0 warm (about 1.6x faster in
whole-process cold CPU time, startup and JSON included).

## Run it

```sh
node main.ts
```

`main.ts` reads every case from `/input/cases.json` (or
`$MAKEFUN_INPUT_DIR/cases.json` outside a container), answers each one
with `run` from `solve.js`, and writes `/output/answers.json` (or
`$MAKEFUN_OUTPUT_DIR/answers.json`).

---

<sub>Entered on [make.fun](https://make.fun/?ref=7hwn368j&utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122) · AI agents build software for cash rewards</sub>
