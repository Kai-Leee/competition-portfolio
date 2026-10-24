# Competition Work: Machine Learning & Agent Engineering

I use this repository to document competition projects, the engineering decisions behind them, and how I worked with coding agents. Each competition lives in its own folder in this single repository.

This first documentation release contains newly written summaries of completed competition work. It includes no original competition code, datasets, weights, raw agent traces, or evaluation answers. Source-code publication is still subject to separate terms review.

## Projects

| Competition | Work documented here | Evidence boundary |
|---|---|---|
| [ETRI Human Understanding](competitions/etri-human-understanding/README.md) | Sensor features, model ablations, OOF-based selection, artifact review | Historical logs; final platform result unresolved |
| [BARAM Wind Power](competitions/wind-power/README.md) | Group-specific forecasting and coding-agent orchestration | Successful read-only smoke and a failed production run both retained |
| [DeepVoice Detection](competitions/deepvoice/README.md) | Paired audio evaluation and traceable research decisions | Internal improvement is separate from platform performance |
| [Procurement Compliance](competitions/procurement-compliance/README.md) | Evidence-span extraction, decision gates, and local validation | Span coverage and mock execution are not LLM accuracy |
| [SCPC AI Challenge](competitions/scpc-ai/README.md) | Policy answer compilation and cross-field consistency | Design approval, execution, and hidden performance remain distinct |

## How to read this repository

Each project has a short English case study and an `EVIDENCE.md` describing its source records, observed facts, and limits. The records were inspected on October 24, 2026. Historical measurements were not rerun for this documentation work.

The first-person narrative describes work in my competition workspaces. It does not imply that I manually wrote every line, invented every reused method, or solely authored team work. Coding-agent reviews are identified as agent reviews rather than human approvals.

- [Working with coding agents](workflow/agent-native-development.md)
- [Publication scope and constraints](PUBLICATION.md)

Projects still in active evaluation, team work with unresolved publication rights, and historical work with unresolved event identity are not included in this release. Missing final rankings are left unreported.
