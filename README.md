# Competition Portfolio — Machine Learning & Agent Engineering

I work on machine learning competitions and the engineering systems that make experiments inspectable. This portfolio connects each problem to my approach, the evidence it produced, and how I used coding agents.

Across these projects, I learned to turn an experiment into a reviewable decision: define the comparison, preserve its artifacts, investigate failures, and separate a promising idea from a verified result.

## Selected work

Outcomes below come from inspected historical records. They were not rerun for this portfolio. Each case links to an evidence index with source fingerprints and verification limits.

| Project | Problem and approach | Observed result | Coding-agent practice |
|---|---|---|---|
| [DeepVoice Detection](competitions/deepvoice/README.md) | Detect generated audio in speech/music mixtures. Investigated stem-based music heads, MuQ features, aggregation, and preprocessing. | On a matched 640-row panel, FILE EER fell from 0.134167 to 0.125000. The 480-row music diagnostic worsened. This is not a verified platform gain. | Question-to-run records, bounded tasks, paired replay, and review of score claims. |
| [BARAM Wind Power](competitions/wind-power/README.md) | Forecast generation by group. Compared tabular, physical-response, sequence, and ensemble ideas under shared evaluation contracts. | Recorded Codex and Claude read-only verification stages succeeded. A separate production implementation run failed; final forecast score remains unverified. | Experiment registry, ownership claims, provider stages, edit scope, and verification commands. |
| [ETRI Human Understanding](competitions/etri-human-understanding/README.md) | Model human state from sensor features using feature/model ablations and out-of-fold selection. | Historical training/comparison artifacts support the workflow. Final platform score and rank remain unresolved. | Role-based instructions and artifact review; recorded comparisons rather than a claimed productivity gain. |
| [Procurement Compliance](competitions/procurement-compliance/README.md) | Find violations and supporting spans. Separated evidence extraction from decision gates and model inference. | Development span coverage changed 51/54 → 48/54 → 53/54. This measures evidence retrieval, not model macro-F1. | Explicit rulebook, modular targets, local checks, and an append-only measurement log. |
| [SCPC AI Challenge](competitions/scpc-ai/README.md) | Compile policy answers consistently across interdependent fields using deterministic rules. | Design and implementation records are inspectable. Hidden-set performance and final rank are unverified. | Task rules became explicit implementation and review criteria; approval and execution remain separate. |
| [Deepfake Detection](competitions/deepfake-detection/README.md) | Focus video inference on faces; separate CPU frame preparation from GPU classification. | Implementation is present. Completed inference, speed gains, and accepted submission are unverified. | Agent involvement cannot be established from inspected notebooks. |
| [Financial Disclosure Agent](competitions/disclosure-agent/README.md) | Connect claims to sources; distinguish valid structure from valid meaning. | Personal design ideas and review lessons are documented. Team implementation and internal performance are withheld. | Semantic review supplements schema checks; agent review is not human approval. |

## How my use of coding agents developed

The records show a progression in how I made work explicit. These are documented practices, not a controlled comparison of agent productivity. The stages describe evidence patterns rather than a strict chronology across every project.

| Practice | What changed | Evidence |
|---|---|---|
| Preserve the experiment | Keep feature choices, validation splits, model comparisons, and outputs available for review. | [ETRI](competitions/etri-human-understanding/README.md) |
| Give agents an execution contract | Register hypotheses, claim work, constrain edits, and define verification before execution. | [Wind power](competitions/wind-power/README.md) |
| Tie conclusions to runs | Link questions and decisions to configuration, metrics, provenance, and receipts; replay candidates on matching inputs. | [DeepVoice](competitions/deepvoice/README.md) |
| Review what a result means | Distinguish retrieval coverage, output validity, semantic correctness, and measured model performance. | [Procurement](competitions/procurement-compliance/README.md), [disclosure agent](competitions/disclosure-agent/README.md) |

[Workflow details](workflow/agent-native-development.md) · [Tools and their actual roles](TOOLS.md)

## Preparation, historical artifacts, and restricted cases

These entries have different evidence boundaries. A folder does not establish a completed or accepted competition entry.

| Entry | Available evidence | Unresolved or withheld |
|---|---|---|
| [Agricultural Price Forecasting](preparations/agricultural-price-forecasting/README.md) | Agent-assisted research and a modeling proposal. | Implementation, performance, and accepted entry are unverified. |
| [Satellite Segmentation](historical-work/satellite-segmentation-2023/README.md) | Historical segmentation notebooks, including interrupted execution. | Exact event identity and completed results are unresolved. |
| [Wildfire-related artifacts](historical-work/wildfire/README.md) | Local inventory only. | Event identity, approach, results, and agent involvement are unresolved. |
| [Synthetic Microstructure Prediction](competitions/microstructure/README.md) | Official task overview. | Detailed attempts, results, and agent workflows remain private during sharing review. |
| [Port Vessel Matching](competitions/vessel-matching/README.md) | Official task overview. | Active solution details remain private. |

## Scope and attribution

This single repository contains newly written documentation. Original code, datasets, weights, raw agent traces, evaluation answers, and restricted team material are excluded. Source-code publication needs a separate terms review.

First-person accounts describe my work within competition workspaces. They do not imply sole authorship of team systems or original invention of reused methods. Missing rankings are left unreported. Review date: October 24, 2026.

[Publication constraints](PUBLICATION.md) · [Coverage and evidence stages](COVERAGE.md)
