# Financial Disclosure Agent: Personal Design and Review Notes

**Publication scope:** newly written, high-level notes from my design work. This is not a release of the team implementation or a claim of sole authorship of it.

## Problem

The local Mirae Asset competition workspace studies how an agent can answer questions from supplied financial disclosures while retaining evidence for values, reporting periods, accounting scope, and corrections. The event's individual publication terms and team implementation rights have not been fully reconciled.

## Ideas I explored

I explored separating document interpretation, source-grounded facts, numerical calculation, and final answer generation. The purpose was to make a plausible answer insufficient on its own: values and their context needed a traceable source, and missing or ambiguous evidence needed an explicit unresolved state. These are recorded design decisions, not a claim that all deployed answers met the design. [MIRAE-4](EVIDENCE.md#mirae-4)

Another part of the approach was preserving original and corrected document versions rather than silently replacing evidence. I treated a structured record passing a schema check as a different claim from that record having the right financial meaning.

## Agent-assisted review

A local review record describes coding-agent inspection of draft questions against source context after structural checks had passed. The review identified semantic problems and sent the work back to generation-rule repair rather than treating the draft as approved evaluation data. The general lesson is that machine checks and agent semantic review answer different questions. [MIRAE-5](EVIDENCE.md#mirae-5)

The report explicitly distinguishes agent opinions from human approval. It does not establish a certified gold set or independently validated service quality.

## Limits and material kept private

Team-serving implementation, detailed internal evaluation results, source documents, generated questions, deployment practices, and team-owned code are not published here. This account covers personal design and review ideas; it does not claim a final submission result, a successfully deployed system, or independent authorship of team work.
