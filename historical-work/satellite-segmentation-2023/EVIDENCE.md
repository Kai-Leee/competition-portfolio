# Evidence and Limits

Reviewed on October 24, 2026. Source records remain outside this repository. Paths below refer to the original workspaces rather than distributed files. SHA-256 identifies the inspected bytes; it does not prove authorship, factual correctness, or independent reproducibility.

## SATELLITE-1

- Record: `Daycon/sw2023/runner.py`
- Evidence type: implementation.
- SHA-256: `7eb0e039cffcb5d22cd84775cd2db822c944a8e3f81ec00515565d07ff7864ea`
- Supports and limits: Runner inspection: model selection, loader, binary-segmentation loss, optimizer, and learning-rate schedule. A dataset-splitting TODO is present. The exact competition identity and original authorship are not established.

## SATELLITE-2

- Record: `Daycon/sw2023/main.ipynb`
- Evidence type: notebook-state.
- SHA-256: `5f7c6a1462f0c1452b48b6abd12043bbba30df754e8995b7b9a642f2c7af1199`
- Supports and limits: Saved notebook state includes error/interruption outputs, including IndexError, KeyboardInterrupt, and NameError. This is not evidence of a clean end-to-end run; raw outputs are not distributed.

## SATELLITE-3

- Record: `Daycon/sw2023/utils/dataloader.py`
- Evidence type: implementation.
- SHA-256: `a980826124fe54a03a515ba78ad20777977938ffc538cf0dc40e6b3dbc2ebf9d`
- Supports and limits: Dataset-loading implementation associates images and masks and uses mask decoding/preprocessing. Source existence is not proof that every validation or augmentation path was correct.

## Review boundary

No training, inference, official submission, remote process, or performance benchmark was rerun for this account. Coding-agent attribution is stated only when the records identify it. General methodological descriptions do not grant redistribution rights to the excluded code, data, model, supplied template, or team material.
