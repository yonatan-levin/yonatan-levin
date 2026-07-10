# Yonatan Levin

I build trading systems — end to end, from market research to live execution. Based in Israel, writing software since 2020.

Most of my work right now goes into a single question: **what does it take to run an automated trading operation you can actually trust?** Not a backtest that looks good in a notebook, but a system that pulls data, forms decisions, executes, and — most importantly — behaves predictably when something goes wrong.

## The stack I'm building

Everything below is one connected effort: an algorithmic trading platform built from small, single-purpose tools rather than one monolith.

- **[midas](https://github.com/yonatan-levin/midas)** — the trading engine at the core. It owns the hot path: taking a strategy's decision and turning it into action, reliably.
- **[strade-orchestrator](https://github.com/yonatan-levin/strade-orchestrator)** — the piece that ties the tools together into real operations. Its defining constraint is **strict failure isolation**: any single tool can fail, and the failure stays contained instead of cascading through the pipeline. In trading, a system that fails safely is worth more than a system that's occasionally brilliant.
- **[borker](https://github.com/yonatan-levin/borker)**, **[swinger](https://github.com/yonatan-levin/swinger)**, **[fin_cli](https://github.com/yonatan-levin/fin_cli)** — the surrounding toolkit: execution, strategy, and the command-line surface for operating all of it.

## How I think about it

- **The code is second to the product.** A trading system is judged by how it behaves in the market, not by its architecture diagram.
- **Small tools, sharp boundaries.** Composable pieces with clear contracts beat a clever monolith — especially when money is on the line.
- **Design for the bad day.** Isolation, containment, and predictable failure modes are features, not afterthoughts.

## Beyond trading

- **[mockingjay](https://github.com/yonatan-levin/mockingjay)** — a separate track: real-time hand-gesture and sign-language recognition. Point a webcam at it and it reads your hands live — tracking up to two at once and classifying gestures, including American Sign Language, as you make them. Built as a real application, not loose notebooks, on top of Google MediaPipe and a custom-trained CNN, with its own ASL training pipeline behind it.

Mostly working in Go and Python these days.

---

<p>
  <a href="https://www.linkedin.com/in/jonatanlevin/"><img src="https://img.shields.io/badge/LinkedIn-Yonatan%20Levin-0A66C2?logo=linkedin&logoColor=white" alt="LinkedIn"></a>
</p>
