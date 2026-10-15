# Ryan J. Gurganious

**AI systems engineer | Agentic AI · ML infrastructure · Edge AI/RISC-V · Research software**

I build AI and research software whose results can be checked by compilers, tests, hardware, and reproducible evidence. **Open to engineering opportunities** in AI systems, ML infrastructure, inference, edge AI, and research software.

[LinkedIn](https://www.linkedin.com/in/ryan-gurganious-41190597/) · [Email](mailto:darthceltic1985@gmail.com)

## Selected work

- **[Determinex](https://github.com/DarthCeltic/Determinex)** — Open-source, local-first multi-agent coding system that checks generated work against configured compiler and test suites. A pass supports only those checks, not general correctness. [AGPL-3.0-or-later](https://github.com/DarthCeltic/Determinex/blob/main/LICENSE).
- **[ARGUS](https://github.com/Cinder-Covenant/ARGUS)** — Provenance-aware workbench for Herculaneum CT research workflows, including data, geometry, rendering, and reproducibility tools.
- **[Herculaneum Scroll Tools](https://github.com/DarthCeltic/herculaneum-scroll-tools)** — Tools for dual-energy ink-contrast analysis and cross-scan registration.

## Awards

- **Winner, Most Validated Model Ports** — AIFoundry × OpenHW CORE-ET Hackathon, 2026: 16 model variants across 15 families. Also placed **5th** for Llama 3.2 1B at 13.68 tok/s on ET-SoC1. [Organizer recap](https://blog.aifoundry.org/p/the-people-the-drama-the-kernels).
- **Excellent Award, Agentic AI track** — AMD AI DevMaster, 2026. [AMD recap](https://www.amd.com/en/developer/resources/technical-articles/2026/lessons-from-the-amd-devmaster-hackathon.html).
- **$250 Progress Prize — Single-pass Hecate** — Vesuvius Challenge, September 2026. The official results jointly credit Ryan Gurganious / @DarthCeltic85 and Daine Ball / @Clexious, and describe single-pass prediction with about 35% speedup. [Official results](https://scrollprize.org/winners).
- **$250 Progress Prize — VC3D agent-bridge fixes** — Vesuvius Challenge, August 2026. The official results credit Ryan Gurganious for enabling the bridge to start Lasagna with the selected volume and to handle large segment downloads without false missing reports. [Official results](https://scrollprize.org/winners).

## Selected upstream contributions

The links below are individual public contributions by Ryan Gurganious; they do not imply ownership of the upstream projects.

- **AIFoundry/OpenHW:** [YOLO register-allocation improvement (#61)](https://github.com/aifoundry-org/hf-hackathon/pull/61), plus [Q8_0 kernel optimizations (#115)](https://github.com/aifoundry-org/hf-hackathon/pull/115) and [(#155)](https://github.com/aifoundry-org/hf-hackathon/pull/155).
- **ScrollPrize/Villa:** [Resolve the active volume's Lasagna dataset (#1439)](https://github.com/ScrollPrize/villa/pull/1439), [handle stalled large HTTP transfers (#1440)](https://github.com/ScrollPrize/villa/pull/1440), and [add ARGUS to community projects (#1896)](https://github.com/ScrollPrize/villa/pull/1896).

## Public evidence index

- **Hecate runtime evidence.** The official award page reports about 35% speedup for the September single-pass change. Separately, a versioned measurement draft in the public Cinder-Covenant/ARGUS repository (prepared for upstream review) records: one 16×256×256 PHerc0139 paired-output field at 9.6 µm on a GTX 1660 Ti, with 35.01% lower median process time and bitwise-equal outputs. The larger timing comparison had thermal pauses. These are workload-specific runtime results, not whole-scroll performance, ink-accuracy, unread-scroll generalization, or 2.4 µm validation. [Official results](https://scrollprize.org/winners) · [versioned measurement draft and limits](https://github.com/Cinder-Covenant/ARGUS/blob/18cbbd3e079cf6cfb6278c8c9afdc7a5b773d37a/docs/september_2026/hecate/PUBLIC_REVIEW_DRAFT.md) · [machine-readable measurement](https://github.com/Cinder-Covenant/ARGUS/blob/18cbbd3e079cf6cfb6278c8c9afdc7a5b773d37a/docs/september_2026/hecate/PUBLIC_MEASURED_RESULT_20260930.json) · [Hecate discussion](https://huggingface.co/scrollprize/hecate/discussions/1).
- **VC3D agent bridge.** The August award recognizes interface and large-download fixes. The public result does not claim a scroll-reading or ink-accuracy outcome. [Official results](https://scrollprize.org/winners).
- **Determinex.** Source and release limits are in the [repository](https://github.com/DarthCeltic/Determinex); the [end-to-end demo](https://youtu.be/eI_AE5k_yv8) and [walkthrough](https://youtu.be/-RR2YlUERfQ) show the workflow. Compiler or test passes establish the checks actually run, not general correctness. Benchmark numbers retain their stated task sets, artifacts, and hardware.
- **ARGUS.** Built by DarthCeltic and clexious under Cinder Covenant. The [public run guide](https://github.com/Cinder-Covenant/ARGUS/blob/main/docs/PUBLIC_RUN.md) includes the offline `python -m argus demo` route. The release ships no detector and makes no unread-scroll, ink, readability, or prize-result claim. [Source](https://github.com/Cinder-Covenant/ARGUS) · [claim limits](https://github.com/Cinder-Covenant/ARGUS/blob/main/PUBLIC_CLAIMS_AND_LIMITS.md).

## Technical focus

Agent verification · model/runtime integration · inference performance · RISC-V/VPU optimization · scientific computing · CT-volume workflows · reproducible research software

## Earlier career

Before moving into software and AI systems work, I spent 17 years at the Social Security Administration in claims adjudication, staff training, and labor leadership—work grounded in evidence, privacy, and high-consequence service delivery.

