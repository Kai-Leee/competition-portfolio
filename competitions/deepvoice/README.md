# DeepVoice Detection

## Challenge

The [DeepVoice competition](https://dacon.io/competitions/official/236749/overview/description) concerns generated audio and the presence of speech and music. My workspace evaluated multiple output heads and investigated discrepancies between internal evaluation and platform results.

## Work I carried out

A recorded paired evaluation compared two candidates on the same input bytes and IDs. The historical D06 report gives the following internal measurements; these were read from the report, not rerun for this portfolio. [VOICE-2](EVIDENCE.md#voice-2)

| Internal diagnostic | Evaluated rows | T152n EER | Candidate A EER |
|---|---:|---:|---:|
| S0 file authenticity | 640 | 0.134167 | 0.125000 |
| Strict speech authenticity | 160 | 0.075000 | 0.075000 |
| Conditional music authenticity | 480 | 0.175000 | 0.179167 |

The file head improved on that exposed diagnostic panel, while the music head worsened. The report also found drift between historical cached outputs and fresh outputs. I therefore do not interpret the comparison as an independently established generalization gain or an improved platform score.

## How coding agents were used

I structured the records around a research question and a decision, linked to the existing experiment's configuration, metrics, provenance, and receipt. Agent entry points distinguish experiment work, record maintenance, and remote operations. This preserves the difference between a request, a plan, an execution, and a verified answer. [VOICE-3](EVIDENCE.md#voice-3) [VOICE-4](EVIDENCE.md#voice-4)

## Status and limits

The project records the end of competition experiments on September 30, 2026. A later candidate's normal platform score remains unresolved in the repository status. Internal metrics do not fill that gap. Source independence and post-run identity limitations are preserved in the underlying report. [VOICE-1](EVIDENCE.md#voice-1)
