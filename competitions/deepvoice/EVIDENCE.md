# Evidence and Limits

Review date: October 24, 2026. These are local source-snapshot references, not links to distributed source assets. The source records are excluded from this documentation release. SHA-256 identifies the exact bytes inspected; it does not prove authorship, factual correctness, or independent reproducibility. Historical measurements were read from the listed record unless a direct JSON inspection is stated.

## VOICE-1

- Record: `Daycon/deepvoice-236749/README.md`
- Evidence type: status.
- SHA-256: `bca1bdd175bad4f7839f725711ecbe92547851e239434fa0766cf29231b356ad`
- What it supports: Dated project status: experiments ended and a later platform score remains unresolved.

## VOICE-2

- Record: `Daycon/deepvoice-236749/research/2026-09-29/lb-gap-001/a_replay_result.md`
- Evidence type: historical-measurement-report.
- SHA-256: `e1af94ac061688941769ceb5d5067dea3528eff7f86dced692f4538e45cc2196`
- What it supports: Historical D06 paired-measurement report, lines 5–24. S0 FILE: 640 rows; strict VOICE: 160; conditional MUSIC: 480. Its methods reference a hashed selector, fresh outputs, d06_evaluate.py, and a metrics artifact. Source audio and remote artifacts were not fetched or re-scored for this review.

## VOICE-3

- Record: `Daycon/deepvoice-236749/docs/RECORDS.md`
- Evidence type: protocol.
- SHA-256: `6806758a7c66b5115214550f046b85739f8fed260abdd1b67f4a1ac2bf49c734`
- What it supports: Question-to-run evidence protocol; protocol existence does not establish universal adherence.

## VOICE-4

- Record: `Daycon/deepvoice-236749/docs/AGENT_START.md`
- Evidence type: routing.
- SHA-256: `0cdbc3692d0261c8981b0993131042700ab8e7c46889d2dd7e570677bb72961a`
- What it supports: Task routing to experiment, record, and remote-operation instructions.

## VOICE-5

- Record: `Daycon/deepvoice-236749/server-archives/shared/docs/lee/T120_MUSIC_RESULTS_20260927.md`
- Evidence type: archived-music-experiment-report.
- SHA-256: `88e590a9f6f6fa1e97b20bc3cc4ee5692059e937442542108c9de5f835899197`
- What it supports: Personal music-head experiments and internal-to-platform reversal; supports the problem/approach account, not a normal platform gain.

## VOICE-6

- Record: `Daycon/deepvoice-236749/server-archives/shared/docs/lee/T120_MUSIC_RESULTS_20260928.md`
- Evidence type: archived-music-experiment-report-with-later-corrections.
- SHA-256: `1125971058545bfb2cb23e4b76b1b612da0fbbdaff159d11bee385d461c70736`
- What it supports: Stem normalization, gates and preprocessing comparisons. Later corrections override early inferred gains; special probes and estimates are not normal submission measurements.

## VOICE-7

- Record: `Daycon/deepvoice-236749/research/2026-09-28/prep-lee/t4_license/PREP_20260928_provenance_t152n.md`
- Evidence type: package-component-and-contribution-audit.
- SHA-256: `565376a48e57287bf1725820bec60dd407e196e1500f1c7cad237636a2ba34ef`
- What it supports: Team package components and recorded contribution attribution, including lee MuQ linear and gated-attention heads. Includes inactive components; package inclusion does not establish causal contribution or resolved upstream licensing.

## VOICE-8

- Record: `Daycon/deepvoice-236749/research/2026-09-29/score-push-001/ledger/20260929T0015KST.md`
- Evidence type: historical-team-platform-ledger.
- SHA-256: `75a5215ca9f57bdd9576a81e7636198c93c06a3cdf6c359efa571e7434028f2c`
- What it supports: Historical team ledger distinguishes normal T152n score 0.8542020688 from special probes and estimates. Normal submission ID is unknown; the platform was not independently queried for this review.

## VOICE-9

- Record: `Daycon/deepvoice-236749/research/2026-09-29/lb-gap-001/drift_probe.md`
- Evidence type: controlled-numerical-drift-diagnosis.
- SHA-256: `c4a3b35bd921d8f49eee69904b81329f831b63171272cb1af600f5c0e26310be`
- What it supports: Controlled cross-host drift diagnosis on three audio inputs: same decoded inputs and weights, cuDNN TF32 toggle, maximum 527-output difference 0.109247 to 5.96e-7. No accuracy or full-dataset conclusion.

## VOICE-10

- Record: `Daycon/deepvoice-236749/artifacts/distribution/closeout-20261001/dist.nosync/pkg_t152_r4/script_fv.py`
- Evidence type: archived-variant-imports.
- SHA-256: `c729a9bf7788546c24c7e36bac99bfc9c1893d62e7440ce60a0abb6cba998873`
- What it supports: Imports and implementation dependencies in an archived fv variant. This is not proof of the exact normal T152n submission script or successful execution of every imported component.

## Verification scope

The review inspected source files and selected recorded results. It did not rerun model training, official submissions, hidden evaluation, or remote processes. Repository-level work is not proof that every component was individually authored by me. Final competition rankings remain unverified unless separately established.
