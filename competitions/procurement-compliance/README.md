# Public Procurement Compliance Monitoring

## Challenge

The [procurement compliance competition](https://dacon.io/competitions/official/236754/overview/description) asks a fixed-model pipeline to identify checklist violations and return supporting text. The [competition rules](https://dacon.io/competitions/official/236754/overview/rules) constrain model use and permitted materials.

## Work I carried out

I implemented evidence selection as qualification-section extraction plus keyword windows, followed by rendering of the selected spans. Decision gates and their application are implemented separately. These components exist in the inspected source; their existence alone does not establish successful fixed-model inference. [PPS-2](EVIDENCE.md#pps-2) [PPS-3](EVIDENCE.md#pps-3)

The historical development log records span-coverage iterations of 51/54, then 48/54, then 53/54 annotated evidence cases. The regression exposed how a seemingly cleaner extraction rule could lose relevant context. This is evidence-span coverage on development cases, not the language model's macro-F1. [PPS-1](EVIDENCE.md#pps-1)

The same log records decision gates incorrectly removing positive development labels, followed by changes that eliminated those observed removals. It does not prove safety or improvement on unseen notices.

## How coding agents were used

The workspace made the task explicit through a rulebook, separate span and gate modules, local checks, and an append-only measurement log. This provided concrete implementation and verification targets for coding-agent work. The reviewed material does not establish a separately executed multi-agent reviewer pipeline, so I do not claim one.

## Limits

The logged mock run checked output format. Scoring the labels against themselves checked the scorer. Neither is a measured model score. GPU inference time, final platform accuracy, and a final ranking remain unverified in this review.
