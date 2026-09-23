<div align="center">

# Fruit Fly World

**Don't exam the model. Starve it.**

A fruit-fly survival game where the brain is a slot. Fly on your own hands, on genes,
on a 24-neuron circuit, or on a judgment model — and the dish grades every decision.

[**fruitfly.world**](https://fruitfly.world) · [Play](https://fruitfly.world/play) · [The exam room](https://fruitfly.world/play?bench=1) · [The essay](https://fruitfly.world/essay) · [@fruitflyworld](https://x.com/fruitflyworld)

</div>

---

## What this is

One dish, one fly, fifty seconds per generation. Food is scarce, a predator lunges,
and at the end of every generation the fly that survived drafts a mutation with a cost.
The twist: **you don't fly — you pick the brain that flies.**

| Brain | What it is |
| --- | --- |
| **Manual** | Your hands. The baseline every other brain has to beat. |
| **Genes** | Weighted reflexes drafted across generations. Evolution as a controller. |
| **Circuit** | FFW-CX — a 24-neuron spiking circuit ported into the game loop. Reflexes with a substrate. |
| **Judgment** | A System One-compatible judgment layer. Runs free on a local heuristic; plug in a pinned remote model with your own key. |

Every decision the brain makes is sealed into a hash-chained log you can download and replay.

## Why it is an exam

- **The exam room** runs the same `(seed, brain, generations)` twice at a fixed 60 Hz. If every
  decision hash and every outcome match, the run is `IDENTICAL` — the world is a fair grader.
- **Beacon seeds** derive the seed from the latest Sepolia block hash — a number nobody,
  including us, could have cherry-picked. The block is linked in the report.
- **Death calibration** checks the brain's own danger scores against reality: does a high
  danger score actually mean death within five seconds? The method is
  [documented with its limits](https://fruitfly.world/calibration).
- **Every result is a challenge** — one click copies a shareable exam card with the seed and
  brain, so anyone can run the same paper and try to beat it.

## Start here

| | |
| --- | --- |
| **Play the survival game** | [fruitfly.world/play](https://fruitfly.world/play) — pick a brain, starve, inherit, repeat. |
| **Starve a model** | [The exam room](https://fruitfly.world/play?bench=1) — deterministic double-runs, beacon seeds, calibration tables. |
| **Point an agent at it** | [The skill](https://fruitfly.world/skill/ffw-arena/SKILL.md) — install once, enter every hour with no human in the loop. |
| **Read the long version** | [The essay](https://fruitfly.world/essay) — neurons, brain slots, the judgment layer, the exam, the refusals. |
| **Check the code** | [fruitflyworld/fruit-fly-world](https://github.com/fruitflyworld/fruit-fly-world) — the site, the game, and the Passport contract. MIT. |

## How it stays honest

- **Determinism is proven, not claimed.** A double-run that diverges is labeled `DIVERGED` —
  a bug report, not a score.
- **The Passport is soul-bound.** ERC-5192 locked at the contract level: one per address,
  non-transferable, earned by playing. Quest-gated freemint; nothing on sale today.
- **Nothing is cherry-picked.** Beacon seeds come from a public block hash. Exam reports link
  the block they were derived from.
- **Biology is the inspiration, not a claim.** The circuit is connectome-inspired; it is not a
  simulation of a real fly brain, and the site never says otherwise.

## Repositories

| Repository | What it holds |
| --- | --- |
| [**fruit-fly-world**](https://github.com/fruitflyworld/fruit-fly-world) | The Next.js site: the game, the exam room, the mission and mint routes, the agent skill, and the `FruitFlyPassport` contract. MIT. |
| [**sim**](https://github.com/fruitflyworld/sim) | The simulation core: the dish world, the LC4/LPLC2→Giant-Fiber escape circuit, the brain contract. Zero dependencies, pinned golden vectors. |
| [**game**](https://github.com/fruitflyworld/game) | The playable game as a static bundle — runs from any host, GitHub Pages included. |
| [**bench**](https://github.com/fruitflyworld/bench) | The exam harness: the double-run determinism protocol, death calibration, production-verified golden runs. |

## Contributing

Issues and pull requests are welcome on any repository. Read
[`CONTRIBUTING.md`](https://github.com/fruitflyworld/fruit-fly-world/blob/main/CONTRIBUTING.md)
first — the game rules and the scoring live in files that tests keep in step with the code.
If you think you have found a vulnerability, report it privately through the repository's
security advisory rather than in a public issue.

<div align="center">
<sub>Fruit Fly World — biology made playable, measurable, and extendable.</sub>
</div>
