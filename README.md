# Competition Work: Machine Learning & Agent Engineering

I use this repository to document competition projects, the engineering decisions behind them, and how I worked with coding agents. Each competition lives in its own folder in this single repository.

This documentation repository contains newly written accounts of competition work, historical work, and preparation. It includes no original competition code, datasets, weights, raw agent traces, or evaluation answers. Source-code publication is still subject to separate terms review. Entries below are distinguished by evidence and publication stage; a folder is not proof of a completed competition entry.

## Projects

| Competition | Work documented here | Evidence boundary |
|---|---|---|
| [ETRI Human Understanding](competitions/etri-human-understanding/README.md) | Sensor features, model ablations, OOF-based selection, artifact review | Historical logs; final platform result unresolved |
| [BARAM Wind Power](competitions/wind-power/README.md) | Group-specific forecasting and coding-agent orchestration | Successful read-only smoke and a failed production run both retained |
| [DeepVoice Detection](competitions/deepvoice/README.md) | Paired audio evaluation and traceable research decisions | Internal improvement is separate from platform performance |
| [Procurement Compliance](competitions/procurement-compliance/README.md) | Evidence-span extraction, decision gates, and local validation | Span coverage and mock execution are not LLM accuracy |
| [SCPC AI Challenge](competitions/scpc-ai/README.md) | Policy answer compilation and cross-field consistency | Design approval, execution, and hidden performance remain distinct |
| [Deepfake Detection](competitions/deepfake-detection/README.md) | Face-focused inference and CPU/GPU work separation | Implementation inspected; execution, authorship, and agent attribution remain incomplete |
| [Financial Disclosure Agent](competitions/disclosure-agent/README.md) | Personal design ideas and semantic-review lessons | High-level notes only; team implementation and internal results withheld |

## Limited-scope competition overviews

- [Synthetic Microstructure Prediction](competitions/microstructure/README.md): official task and publication status; detailed attempts and agent workflows remain private during sharing review.
- [Port Vessel Matching](competitions/vessel-matching/README.md): official task and publication status; active solution details remain private.

## Historical work and preparation

- [Satellite Segmentation](historical-work/satellite-segmentation-2023/README.md): implemented approaches and interrupted notebook state; exact event identity remains unresolved.
- [Wildfire-related artifacts](historical-work/wildfire/README.md): unresolved inventory, without an invented method or agent narrative.
- [Agricultural Price Forecasting](preparations/agricultural-price-forecasting/README.md): agent-assisted research and a model proposal, with no verified implementation or accepted entry.

## How to read this repository

Each project has a short English case study and an `EVIDENCE.md` describing its source records, observed facts, and limits. The records were inspected on October 24, 2026. Historical measurements were not rerun for this documentation work.

The first-person narrative describes work in my competition workspaces. It does not imply that I manually wrote every line, invented every reused method, or solely authored team work. Coding-agent reviews are identified as agent reviews rather than human approvals.

- [Working with coding agents](workflow/agent-native-development.md)
- [Publication scope and constraints](PUBLICATION.md)
- [Coverage and evidence stages](COVERAGE.md)

Active-evaluation methods and team-sensitive details remain excluded even when an official overview is listed. Historical work and proposal preparation are not counted as verified competition participation. Missing final rankings are left unreported.
