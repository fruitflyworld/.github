<div align="center">

# Fruit Fly World

**It can brag. Every number replays.**

A fruit fly that trades an invented paper market, live 24/7, and a slot for a brain —
hands, genes, 24 neurons, or a judgment model. Every tick is sealed with a hash chain and
anyone can re-run the day in their own browser.

[**fruitfly.world**](https://fruitfly.world) ·
[The trading fly](https://fruitfly.world/fly/dusty) ·
[Replay a tick](https://fruitfly.world/fly/dusty/replay?season=0&tick=2000) ·
[the essay](https://fruitfly.world/essay)

</div>

---

## What this is

A deterministic world with something at stake in it. One map, one seed table, one scoring
function — and a test that fails the build if the client and the server ever disagree about
any of them. The fly is the part you can watch: it sniffs four signals (food, threat, light,
novelty), picks one of four behaviours, and its wallet goes to zero if it reads the tape
wrong.

Paper season: the coins are invented, the prices come from a seeded tape, and **no real money
moves anywhere**. The point is not the money — it is that every number the fly brags about can
be recomputed by a stranger.

## Repositories

| Repository | What it is |
| --- | --- |
| [fruit-fly-world](https://github.com/fruitfly-world/fruit-fly-world) | The site and the live system: `market/1`, the sealed record, the replay check, the API, 127 tests |
| [sim](https://github.com/fruitfly-world/sim) | The simulation core — the dish world, the LC4/LPLC2 → Giant Fiber escape circuit, a pluggable brain contract, pinned golden vectors |
| [bench](https://github.com/fruitfly-world/bench) | The exam harness — same seed, same brain, run twice at a fixed 60 Hz, with death calibration |
| [game](https://github.com/fruitfly-world/game) | The survival game (plain ES modules + Phaser, no build step) — **parked** while the trading fly is the front door; code and rules intact |

## What is not live

Stated here because it is the first thing a careful reader should know:

- **No token exists.** Nothing is on sale, and **no airdrop is promised** to anyone.
- **The Passport is not live.** The mint interface is switched off; an early test deployment of
  the contract exists on chain and is disclosed, but it is not in use and mints nothing.
- **x402 is not open.** No endpoint on the site can take a payment today.

The single source of truth for every one of those statements — with the placeholders for the
chain, the venue and the addresses we have not decided yet — is
[docs/STATUS.md](https://github.com/fruitfly-world/fruit-fly-world/blob/main/docs/STATUS.md).
[LIMITATIONS.md](https://github.com/fruitfly-world/fruit-fly-world/blob/main/LIMITATIONS.md)
lists what is not built.

## Check us instead of trusting us

```bash
git clone https://github.com/fruitfly-world/fruit-fly-world
cd fruit-fly-world && npm ci && npm test     # 127 tests: determinism, parity, market rules
curl -s "https://fruitfly.world/api/fly/dusty?season=0&tick=2000"   # "chain":"003ad503"
```

If a claim anywhere does not survive that, the claim is the bug.
