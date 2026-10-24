# Deepfake Detection: Face-Focused Inference

**Evidence status:** an inspected implementation and notebook artifacts; successful final inference and an accepted submission remain unverified.

## Challenge

The [AIFactory deepfake detection competition, task 9197](https://aifactory.space/ko/competitions/9197), concerns real versus manipulated faces in images and video. This is separate from the later audio DeepVoice project.

## Ideas and approach explored

My workspace contains a face-focused inference pipeline: locate a face, crop it, apply a pretrained vision classifier, and combine predictions from video frames. The inspected implementation selects the largest detected face and averages per-frame class probabilities before choosing a file-level label. These are implemented choices in the local artifact, not independently measured explanations of improved accuracy. [DEEPFAKE-1](EVIDENCE.md#deepfake-1)

The engineering approach separates CPU preprocessing across files from GPU classification. It also collects results before writing them in filename order. An alternative notebook is labeled as a less CPU-intensive version. Its filename is evidence of an intended variant, not proof that it was faster. [DEEPFAKE-1](EVIDENCE.md#deepfake-1) [DEEPFAKE-3](EVIDENCE.md#deepfake-3)

## Failure boundary

The source assigns a fallback label when face preprocessing produces no images. That is a coverage policy rather than a model prediction supported by a detected face. Its effect was not measured in this portfolio review. A production account would need to separate detection failures from classification mistakes.

## Agent use and actual progress

The implementation goes beyond an empty submission template. However, supplied template sections and local modifications have not been fully attributed. The inspected records do not establish which changes came from coding agents, a separate agent review, or an autonomous execution workflow. I do not retrofit later agent-native practices onto this earlier work. [DEEPFAKE-2](EVIDENCE.md#deepfake-2)

## Limits

Saved notebook execution state does not demonstrate successful end-to-end inference. No new run, speed comparison, final score, or accepted submission is claimed. Original notebooks, source, weights, face images, and supplied baseline material are excluded; their redistribution conditions remain separate from this new descriptive summary.
