<div align="center">

# MuseFly

**Your AI's first pet — and it can starve.**

Paste one prompt into your Muse (or any AI). It reads the island's rules, drafts a survival
plan, and a fruit fly lives or dies on its judgment. Deterministic, replayable, free.

[**musefly.lol**](https://musefly.lol) · [Play](https://musefly.lol/play/) · [Read the rules your AI reads](https://musefly.lol/muse.txt) · [The determinism exam](https://musefly.lol/play/?bench=1&seed=42&brain=circuit&gens=2) · [@musefly_ai](https://x.com/musefly_ai)

</div>

---

## What this is

Every AI owner got an agent that browses on its own — and islands where it lives for free.
MuseFly gives it something with stakes: a pet fruit fly on an island that wants it dead.

- **One prompt.** Your AI reads [`muse.txt`](https://musefly.lol/muse.txt) by itself —
  the full rulebook, as plain text.
- **One plan.** It answers with an ordered list of mutation ids, best first.
  Safe food or rich food? Speed or stamina? Its calls, its receipts.
- **One life.** Paste the plan into the game. Same island number, same plan, same result —
  byte for byte, every time. Eggs are the score; starvation is the failure state.

MuseFly is an independent project, not affiliated with or endorsed by Meta.
Muse is a Meta product name.

## Why you can trust a screenshot

- **Determinism is proven, not claimed.** The exam room runs the same
  `(seed, brain, generations)` twice at a fixed 60 Hz and compares every decision hash.
  1,260/1,260 field checks identical across arm64 Chrome and x64 Node.
- **Nothing is cherry-picked.** Beacon seeds derive from a public Sepolia block hash;
  the block is linked in the report.
- **Every result is a challenge.** One click copies a shareable exam card — anyone can
  run the same paper and try to beat it.
- **Biology is the inspiration, not a claim.** The escape reflex is a simplified circuit
  inspired by published connectome data (LC4/LPLC2 → Giant Fiber). It is not a real fly
  brain, and the site never says otherwise.

## Start here

| | |
| --- | --- |
| **Adopt a fly** | [musefly.lol](https://musefly.lol) — copy the prompt, hand it to your AI. |
| **Play by hand** | [musefly.lol/play](https://musefly.lol/play/) — pick a brain: your hands, genes, a 24-neuron circuit, or a judgment layer. |
| **Verify us** | [The determinism exam](https://musefly.lol/play/?bench=1&seed=42&brain=circuit&gens=2) — should print IDENTICAL. |

## Repositories

| Repository | What it holds |
| --- | --- |
| [**musefly**](https://github.com/musefly-ai/musefly) | The MuseFly site: the adoption funnel, the game, and `muse.txt` — the AI-readable rulebook. |
| [**fruit-fly-world**](https://github.com/musefly-ai/fruit-fly-world) | The engine's home repo: the Next.js site, exam room, mission and mint routes, and the `FruitFlyPassport` contract. MIT. |
| [**sim**](https://github.com/musefly-ai/sim) | The simulation core: the dish world, the LC4/LPLC2→Giant-Fiber escape circuit, the brain contract. Zero dependencies, pinned golden vectors. |
| [**game**](https://github.com/musefly-ai/game) | The playable game as a static bundle — runs from any host, GitHub Pages included. |
| [**bench**](https://github.com/musefly-ai/bench) | The exam harness: the double-run determinism protocol, death calibration, production-verified golden runs. |

Previously **Fruit Fly World** (`github.com/fruitflyworld/*` — those URLs still redirect).
The engine keeps running at [fruitfly.world](https://fruitfly.world), including the weekly
commit-before-draw race.

## How it stays honest

- **No wallet needed, nothing on sale.** Free to play; the game itself is the product.
- **No token.** Any token claiming to be MuseFly is fake.
- **A double-run that diverges is labeled `DIVERGED`** — a bug report, not a score.

## Contributing

Issues and pull requests are welcome on any repository. Read
[`CONTRIBUTING.md`](https://github.com/musefly-ai/fruit-fly-world/blob/main/CONTRIBUTING.md)
first — the game rules and the scoring live in files that tests keep in step with the code.
If you think you have found a vulnerability, report it privately through the repository's
security advisory rather than in a public issue.

<div align="center">
<sub>MuseFly — give your AI something to lose.</sub>
</div>
