<div align="center">
  <img src="https://raw.githubusercontent.com/fruitflyworld/fruit-fly-world/main/assets/logo.svg" width="96" alt="Fruit Fly World">
  <h1>Fruit Fly World</h1>
  <p><strong>It can brag. <em>Every number replays.</em></strong></p>
  <p>A fruit fly that trades an invented paper market. Trading fees are its food.<br/>
  When they dry up it starves, and its offspring take over the wallet.</p>
  <p>
    <a href="https://fruitfly.world/fly/dusty"><strong>Watch Dusty</strong></a> ·
    <a href="https://fruitfly.world/fly/dusty/replay?season=0&tick=2000">Replay a tick yourself</a> ·
    <a href="https://github.com/fruitflyworld/fruit-fly-world/blob/main/docs/STATUS.md">Status</a> ·
    <a href="https://x.com/fruitfly_world">@fruitfly_world</a>
  </p>
</div>

---

## What is live

| | Status |
| --- | --- |
| **Dusty, the trading fly** | Live, paper season: invented coins, simulated wallet, no real money moves |
| **Sealed record + browser replay** | Live: every tick is hashed and chained; your browser re-runs the day and compares |
| **$FLY** | Not live. No token exists today |
| **Genesis Passport** | Not live |
| **The survival game** | Parked; the code stays open source |

[`docs/STATUS.md`](https://github.com/fruitflyworld/fruit-fly-world/blob/main/docs/STATUS.md) is the single source of truth. If anything here disagrees with it, STATUS.md is right.

## Check it in ten seconds

```bash
curl -s "https://fruitfly.world/api/fly/dusty?season=0&tick=2000" | grep -o '"chain":"[0-9a-f]*"'
# "chain":"003ad503"  <- the same value CI pins in the repository
```

## Repositories

| Repository | What it holds |
| --- | --- |
| [**fruit-fly-world**](https://github.com/fruitflyworld/fruit-fly-world) | The product: the site, the trading fly (`market/1`), the replay, the status page. |
| [**sim**](https://github.com/fruitflyworld/sim) | The fly's body: the dish, a connectome-inspired escape circuit, a slot for a brain. Zero dependencies. |
| [**bench**](https://github.com/fruitflyworld/bench) | The determinism exam: same seed, same brain, run twice, compared bit for bit. |
| [**game**](https://github.com/fruitflyworld/game) | The original survival game. Parked. |

The biology is an inspiration, not a claim: the escape reflex is a simplified circuit based on published connectome data, not a real fly brain.

## Stay safe

- A contract address will only ever be published on **fruitfly.world** first. Anything else is fake.
- We never DM first, never ask for keys or seed phrases, and never run private sales.
- Found a vulnerability? Report it privately through the repository's security advisory, not in a public issue.

<div align="center"><sub>Fruit Fly World · MIT licensed · every number replays</sub></div>
