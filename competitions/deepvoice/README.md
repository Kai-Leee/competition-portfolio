# DeepVoice Detection

## Problem

The [DeepVoice competition](https://dacon.io/competitions/official/236749/overview/description) concerns generated audio and the presence of speech and music. The working pipeline produced five outputs: file, voice, and music authenticity, plus voice and music presence.

Mixtures made this difficult: vocals could obscure the music signal, while silence and low-energy stems could destabilize a music detector. I investigated representations and preprocessing that matched this structure.

## My contribution within the team pipeline

The component audit attributes MuQ linear and gated-attention multiple-instance learning heads to my work. Archived reports under my working directory document music-head and preprocessing experiments. [VOICE-5](EVIDENCE.md#voice-5) [VOICE-6](EVIDENCE.md#voice-6) [VOICE-7](EVIDENCE.md#voice-7)

The complete system was team work. It combined source separation, specialist authenticity detectors, presence detection, ensembles, and postprocessing. I do not claim sole authorship or isolate my contribution from its aggregate score.

| Difficulty | Approach investigated or used | What the records support |
|---|---|---|
| Speech and music overlap | Use MelBand-RoFormer separation and task-specific music heads rather than relying only on mixed-audio features. | Separation and specialist heads are recorded team-package components. Their isolated platform contribution was not established. |
| A stronger representation may not transfer | Extract frozen MuQ features; compare a linear head with gated-attention aggregation over segments. | My heads are identified in the audit. Raw-audio music-head gains on internal proxies failed to transfer to platform probes. |
| Quiet stems and channel preprocessing | Test silence/low-energy gates, conditional stem loudness normalization, and channel averaging choices. | Reports record the comparisons. Candidate estimates and special probe scores do not establish a normal submission gain. |
| Duration and pooling affect clip-level decisions | Examine segment aggregation and length-conditioned calibration in the surrounding ensemble. | These mechanisms are recorded in the package. The later candidate changed multiple components, so its effect cannot be assigned to one mechanism. |

The practical lesson was to treat representation quality, preprocessing, calibration, and evaluation alignment as separate hypotheses. A lower proxy EER was insufficient evidence to adopt a replacement. [VOICE-5](EVIDENCE.md#voice-5) [VOICE-6](EVIDENCE.md#voice-6) [VOICE-7](EVIDENCE.md#voice-7)

## Measured outcome and its boundary

The historical D06 report compares freshly evaluated T152n and candidate A on the same input bytes and IDs. These measurements were read from the report, not rerun for this portfolio. [VOICE-2](EVIDENCE.md#voice-2)

| Internal diagnostic | Evaluated rows | T152n EER | Candidate A EER | Interpretation |
|---|---:|---:|---:|---|
| S0 file authenticity | 640 | 0.134167 | 0.125000 | Lower EER on this panel. |
| Strict speech authenticity | 160 | 0.075000 | 0.075000 | Unchanged. |
| Conditional music authenticity | 480 | 0.175000 | 0.179167 | Higher EER; a regression. |

This was an exposed diagnostic panel, not an independent generalization test. Cached outputs also differed from fresh outputs. The result supports a specific paired comparison, not a universal improvement or a proven platform gain.

The team ledger records T152n's normal five-output platform score as **0.8542020688**. This is a historical team-reported result; its submission ID is unknown in the ledger. I did not independently revalidate the receipt. [VOICE-8](EVIDENCE.md#voice-8)

The later candidate's normal platform score and final rank remain unverified. Estimates and nonstandard probes are excluded from performance claims. Experiments ended on September 30, 2026. [VOICE-1](EVIDENCE.md#voice-1) [VOICE-8](EVIDENCE.md#voice-8)

## Numerical reproducibility work

A controlled drift probe checked identical decoded inputs and weights across hosts. On three audio inputs, disabling cuDNN TF32 reduced the recorded maximum absolute difference in PANNs 527-output vectors from 0.109247 to 5.96e-7. [VOICE-9](EVIDENCE.md#voice-9)

This diagnoses numerical reproducibility on those three inputs. It does not establish an accuracy improvement, a full-dataset guarantee, or adoption of that configuration in the final package.

## How I used coding agents

I organized work around a question, a bounded task, and a decision linked to a run's configuration, metrics, provenance, and receipt. Entry points separate experiment work, record maintenance, and remote operations. [VOICE-3](EVIDENCE.md#voice-3) [VOICE-4](EVIDENCE.md#voice-4)

Paired replay and review helped challenge score claims, including assumptions that proxy gains could simply be added to platform results. Protocols and reviewed runs do not prove universal adherence. [VOICE-2](EVIDENCE.md#voice-2) [VOICE-8](EVIDENCE.md#voice-8)

## Tools and publication scope

The inspected variant uses Python, PyTorch, torchaudio, librosa, NumPy, and safetensors. The audit identifies MuQ, MelBand-RoFormer, PANNs, and other specialists. Included components were not active in every variant. [VOICE-7](EVIDENCE.md#voice-7) [VOICE-10](EVIDENCE.md#voice-10)

[Tool roles and verification limits](../../TOOLS.md) distinguish implementation evidence from execution. Original scripts, weights, audio, submission packages, and raw agent traces are excluded from this release.
