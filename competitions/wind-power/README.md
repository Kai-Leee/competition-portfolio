# BARAM 2026: Wind Power Forecasting

## Challenge

[BARAM 2026](https://dacon.io/competitions/official/236727/overview/description) predicts hourly generation for three wind-power groups from weather forecasts. The competition objective combines forecast accuracy with a settlement-related measure.

## Work I carried out

I organized group-specific modeling, error analysis, and candidate comparison around fixed data availability, validation splits, baselines, and adoption criteria. The workspace records direct tabular models, physical response ideas, sequence approaches, and ensembles. Comparisons are meaningful only within compatible evaluation conditions. [WIND-4](EVIDENCE.md#wind-4)

The engineering work made an experiment a tracked lifecycle: register a hypothesis, search prior work, define an execution plan, claim the work, run shared training/evaluation, then record completion or failure. This let coding agents work against an explicit contract instead of a loosely remembered conversation. [WIND-4](EVIDENCE.md#wind-4)

## How coding agents were used

The orchestration implementation separates provider stages, edit scope, and verification commands. An archived read-only smoke run contains successful Codex and Claude verification stages, both with return code zero and no recorded changed paths or scope violations. [WIND-1](EVIDENCE.md#wind-1) [WIND-2](EVIDENCE.md#wind-2)

A separate production execution has `success=false` and an unsuccessful implementation stage. I retain this failure rather than describing the workflow as fully successful autonomous research. A successful smoke test and an experiment's terminal result are different evidence. [WIND-3](EVIDENCE.md#wind-3)

## Limits

The inspected records do not establish a universal productivity gain, a cost reduction, or a production success rate. The final competition rank and final submission score have not been verified for this portfolio.
