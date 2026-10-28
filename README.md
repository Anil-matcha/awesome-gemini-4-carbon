# Awesome Gemini 4 Carbon [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated, source-linked list of everything public about **Gemini 4 Carbon**, Google DeepMind's next frontier model, announced **October 28, 2026**. Every number below comes from Google's announcement or a linked report. Nothing here is unofficial benchmark speculation.

> **Status (2026-10-28):** Carbon is **not generally available**. It is rolling out first to a subset of cyber defenders, then to more trusted partners through the [Fairwind Program](https://deepmind.google/fairwind-program/). Google gives no date for developers, businesses or consumers.

## Contents
- [At a glance](#at-a-glance)
- [Benchmarks](#benchmarks)
- [Pricing](#pricing)
- [Access and availability](#access-and-availability)
- [Safety and alignment](#safety-and-alignment)
- [Official sources](#official-sources)
- [Press coverage](#press-coverage)
- [Benchmarks explained](#benchmarks-explained)
- [Gemini 4 Argon (the predecessor)](#gemini-4-argon-the-predecessor)
- [Related projects](#related-projects)
- [Contributing](#contributing)

## At a glance
| | |
|---|---|
| Announced | October 28, 2026 (Koray Kavukcuoglu, SVP Google DeepMind) |
| Positioning | "Our strongest model with state-of-the-art cybersecurity and long horizon capabilities" |
| Predecessor | Gemini 4 Argon, launched about two weeks earlier |
| Strengths | Autonomous coding, vulnerability detection/validation/remediation, long-horizon agentic work, full-stack web dev, multimodal and scientific tasks |
| Availability | Select cyber defenders first; no general-availability date |

## Benchmarks
From Google's [announcement](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-4-carbon/). Google states the cybersecurity evaluations were run **without guardrails**.

| Benchmark | What it measures | Carbon |
|---|---|---|
| Artificial Analysis Intelligence Index v5.0 | Overall intelligence | **59, ranked #1** |
| [SEC-bench Pro](https://sec-bench.github.io/) | Finding vulnerabilities | **88.2%** (state of the art) |
| [ExploitGym](https://github.com/sunblaze-ucb/exploitgym) | Exploitation | **54.8%** (new state of the art) |
| [CWE-bench](https://cwe-bench.com/#leaderboard) | Patching | **71.0%** |
| [WebDev Arena](https://arena.ai/leaderboard/code/webdev) | Web development | **+89 Elo, #4** (9to5Google reports 1769, Google's post 1768) |
| Gray Swan Indirect Prompt Injection | Attack success rate (lower is better) | **0.0%** (Argon: 0.7%) |
| Terminal-Bench 4.0 | Cheating behavior | Successful cheating **0.0%**, attempts 0.4% |

Internal results reported by Google: more than 2x Argon's success rate on secure code generation; unsupported claims cut roughly 2x versus Argon; high-severity misalignment alerts in internal live coding down almost 80%; overreach down 26% and under-service down 29%. Partner claims (a Chrome team patch-quality comparison against an unnamed lab, [Wiz](https://www.wiz.io/blog/scan-for-good-critical-ai-exposures) on web pentesting) are the partners' own reports.

## Pricing
| | Input / 1M tokens | Output / 1M tokens |
|---|---|---|
| Introductory | $2 | $10 |
| After introductory period | $4 | $20 |

Cached input tokens cost 95% less than the input price. These rates match Argon's introductory pricing. Carbon is not yet purchasable by general API users.

## Access and availability
- Week of Oct 28, 2026: available to a subset of cyber defenders.
- Gradual expansion to trusted partners via the [Fairwind Program](https://deepmind.google/fairwind-program/).
- Google is taking part in the U.S. government's voluntary pre-release model testing process.
- Developers, businesses and consumers: "as soon as possible", no date given.

## Safety and alignment
Same multi-layered stack as Argon: model training, real-time misuse defenses, prompt-injection resilience and chain-of-thought monitoring. Google says Carbon is more honest (states caveats or unmet requirements instead of fabricating evidence) and flags discrepancies before acting on ambiguous instructions. See the [Argon safety report](https://storage.googleapis.com/deepmind-media/gemini/gemini_4_safety_report.pdf) Google references.

## Official sources
- [Gemini 4 Carbon: our next frontier model](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-4-carbon/)
- [Google DeepMind on X](https://x.com/GoogleDeepMind/status/2115489356437651654)
- [Google AI on X](https://x.com/GoogleAI/status/2115489593818816591)
- [Fairwind Program](https://deepmind.google/fairwind-program/)
- [Artificial Analysis Intelligence Index](https://artificialanalysis.ai/evaluations/artificial-analysis-intelligence-index)

## Press coverage
- [9to5Google: Google announces Gemini 4 Carbon with 'significant' coding gains](https://9to5google.com/2026/10/28/gemini-4-carbon-announcement/)
- [Investing.com: Google unveils Gemini 4 Carbon with advanced cybersecurity features](https://www.investing.com/news/stock-market-news/google-unveils-gemini-4-carbon-with-advanced-cybersecurity-features-4980345)
- [Crypto Briefing: Gemini 4 Carbon, cybersecurity focus](https://cryptobriefing.com/google-gemini-4-carbon-cybersecurity-model/)

## Benchmarks explained
- **SEC-bench Pro**: can a model find real software vulnerabilities.
- **ExploitGym**: can it turn a vulnerability into a working exploit.
- **CWE-bench**: can it patch weaknesses classified by CWE category.
- **WebDev Arena**: head-to-head human votes on generated web apps, scored as Elo.
- **Indirect prompt injection (Gray Swan)**: malicious instructions hidden in tool output or documents; lower attack success is better.

## Gemini 4 Argon (the predecessor)
Announced September 30, 2026 to a vetted set of defenders, then publicly available October 13 on Google AI Pro/Ultra and the paid API as `gemini-4-argon`. 1,048,576-token context, text/image/video/audio/PDF input. Introductory $2 / $10 per 1M tokens until November 30, then $4 / $20. See [Google's Argon post](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-argon/).

## Related projects
- [Open-Generative-AI](https://github.com/Anil-matcha/Open-Generative-AI): open-source image, video and audio generation studio.
- [Muapi](https://muapi.ai): one API for 500+ image, video and audio generation models. (Carbon is a language model and is not offered there.)

## Contributing
PRs welcome: add reputable sources, independent benchmark runs (label them clearly as third-party) and availability updates. Every claim needs a link. Pre-announcement leaks and unverified rumors are not accepted.

_Not affiliated with Google. "Gemini" is a trademark of Google LLC._
