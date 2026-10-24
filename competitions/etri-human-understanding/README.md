# ETRI Human Understanding

## Challenge

The [5th ETRI Human Understanding AI Competition](https://dacon.io/competitions/official/236690/overview/description) predicts human-state outcomes from lifelog and sensor records. My workspaces approached the task through probability prediction at the subject-and-day level.

## Work I carried out

I explored a progression from metadata-only logistic regression to daily sensor aggregates, subject-relative features, and model ablations with LightGBM and CatBoost. The experiment log then records more targeted sleep and behavior features. Some additions worsened validation, so the narrative is about controlled feature investigation rather than an uninterrupted sequence of improvements. [ETRI-1](EVIDENCE.md#etri-1)

A later selection report compares a CV-best candidate, a calibrated fallback, a conservative target-wise OOF policy, and a train-all refit. It explicitly says that selection reused existing outputs and was not a new validation experiment. I keep candidate selection separate from a successful platform submission. [ETRI-2](EVIDENCE.md#etri-2)

## How coding agents were used

The project separated a competition-leader review role from implementation work. A concrete review record checks that metrics, manifests, fold scores, submission checks, logs, and an exit-status file were collected before drawing a conclusion. This is evidence of an artifact-based review workflow; it does not establish that every historical task followed the same process. [ETRI-3](EVIDENCE.md#etri-3)

## Limits

Several local workspaces represent branches of the same investigation. Their splits and scores must not be collapsed into a single improvement curve. The final submission, final ranking, and the canonical lineage across all branches remain unresolved. Individual sensor records and subject-level examples are excluded.
