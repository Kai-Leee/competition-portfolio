# Evidence and Limits

Review date: October 24, 2026. These are local source-snapshot references, not links to distributed source assets. The source records are excluded from this documentation release. SHA-256 identifies the exact bytes inspected; it does not prove authorship, factual correctness, or independent reproducibility. Historical measurements were read from the listed record unless a direct JSON inspection is stated.

## PPS-1

- Record: `contest/pps-compliance/docs/runs.md`
- Evidence type: historical-measurement-log.
- SHA-256: `3e2e2108a6c00e4d4ef18d2c86d401538bd1191f836a9ee053d5596d56b02258`
- What it supports: Historical log, lines 49–64. Recorded method: scripts/measure_spans.py 9000; coverage denominator 54 development evidence cases. Earlier attempts were 51/54 and 48/54; final recorded coverage 53/54. check_gates.py measures development-label removals; mock execution and scorer self-check are separate checks. None was rerun for this portfolio.

## PPS-2

- Record: `contest/pps-compliance/src/pps/spans.py`
- Evidence type: implementation.
- SHA-256: `dcd265deb58eedcee1c0e0d532a994f40ab3470ba30f1bd1441bd5e44fb60711`
- What it supports: AST inspection confirms qualification_section, keyword_windows, build_spans, and render implementations.

## PPS-3

- Record: `contest/pps-compliance/src/pps/rules.py`
- Evidence type: implementation.
- SHA-256: `1315419cb7bda88b0796f9c504632a94f52be7ceb6e851ecf80d410cbdc1f233`
- What it supports: AST inspection confirms gates and apply implementations; it does not prove LLM execution or unseen-case safety.

## Verification scope

The review inspected source files and selected recorded results. It did not rerun model training, official submissions, hidden evaluation, or remote processes. Repository-level work is not proof that every component was individually authored by me. Final competition rankings remain unverified unless separately established.
