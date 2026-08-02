# Ryan G · `DarthCeltic`

I build systems where **a compiler decides, not a model.**

[![AIFoundry Hackathon](https://img.shields.io/badge/%F0%9F%8F%86%201st%20Place-Most%20Validated%20Model%20Ports-brightgreen?style=for-the-badge)](https://github.com/aifoundry-org/hf-hackathon)
[![Llama 3.2 1B](https://img.shields.io/badge/5th-Fastest%20Llama%203.2%201B-blue?style=for-the-badge)](https://github.com/aifoundry-org/hf-hackathon)

**🏆 1st Place — Most Validated Model Ports**, AIFoundry × OpenHW CORE-ET Hackathon 2026
(16 variants across 15 model families, validated on real **ET-SoC1** RISC-V silicon).
Also placed **5th — Fastest Llama 3.2 1B**. Prize: an ET-SoC1 development board.

---

### 🔭 Determinex — a coding agent that is never its own judge

[![License](https://img.shields.io/badge/license-AGPL--3.0--or--later-blue)](https://github.com/DarthCeltic/Determinex/blob/main/LICENSE)
[![Repo](https://img.shields.io/badge/source-DarthCeltic%2FDeterminex-black?logo=github)](https://github.com/DarthCeltic/Determinex)

Most AI coding tools ask a model whether its own answer is good. Determinex never does.
A real compiler or a real test suite is the only oracle, which has a consequence most agent
architectures don't have: correctness comes from sampling **K** candidates and verifying each,

```
P(correct) = 1 − (1 − p)^K
```

so accuracy is bounded by **GPU batch throughput**, not by model quality. Measured on an AMD
Radeon (ROCm 7.2.1 / vLLM): **28.7 → 739.9 aggregate tok/s from K=1 to K=32, for 1.21× the
wall clock.** Same GPU, same model. The agent gets more correct because the GPU batches better.

It also publishes where it *stops* working — `p = 1.000` (saturated, K buys nothing),
`p = 0.490` (the productive middle: 99.54% at K=8), `p = 0.000` (no K helps). Reporting the
floor is the unusual part.

---

### 🛠 Open-source contributions

**[aifoundry-org/hf-hackathon](https://github.com/aifoundry-org/hf-hackathon)** — kernel and
model-port work for **ET-SoC1** RISC-V AI silicon:

| PR | What |
|---|---|
| [#155](https://github.com/aifoundry-org/hf-hackathon/pull/155) | `smolvlm2_500m_video`: hoist Q8_0 dot horizontal reduce |
| [#115](https://github.com/aifoundry-org/hf-hackathon/pull/115) | `smolvlm2_500m_video`: hoist redundant vector-mask CSR ops |
| [#111](https://github.com/aifoundry-org/hf-hackathon/pull/111) | `smolvlm2_500m_video`: vector-mask CSR hoist |
| [#113](https://github.com/aifoundry-org/hf-hackathon/pull/113) | CI: wire SmolVLM2-500M-Video as a week-2 track |
| [#61](https://github.com/aifoundry-org/hf-hackathon/pull/61) | YOLO: unbind accumulator registers from the frame |

Every one merged, measured on real silicon.

---

### 🧠 What I actually care about

- **Verification over vibes.** A check must never report an outcome it did not establish.
- **Publishing the floor.** A benchmark number that cannot survive a provenance audit is
  worth less than a zero that can — which is why Determinex reports **0/200** on
  ProgramBench after an audit retracted 62 of 67 earlier "solves."
- **Local-first.** Your source should not have to leave your machine to get good help.

📫 darthceltic1985@gmail.com
