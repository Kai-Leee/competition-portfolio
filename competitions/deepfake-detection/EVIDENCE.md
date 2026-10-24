# Evidence and Limits

Reviewed on October 24, 2026. Source records remain outside this repository. Paths below refer to the original workspaces rather than distributed files. SHA-256 identifies the inspected bytes; it does not prove authorship, factual correctness, or independent reproducibility.

## DEEPFAKE-1

- Record: `AIContest/deepfake/deepfake/task.md`
- Evidence type: inspected-inference-implementation.
- SHA-256: `a1ee3bdd57816a40a6d253a475a8b997a26d57ef1983a5319ac555daf1d52c1f`
- Supports and limits: Inspected inference code embedded in the local Markdown artifact, approximately lines 179–327: face detection/cropping, video-frame sampling, CPU preprocessing, GPU classifier execution, averaging probabilities, fallback label, and ordered output writing. Implementation inspection is not a successful-run receipt.

## DEEPFAKE-2

- Record: `AIContest/deepfake/deepfake/task.ipynb`
- Evidence type: notebook-state.
- SHA-256: `fcf0c097bbb2ba2c28f1a7bd34e38af1f72b8b052cb29e403d377ebfbc023abc`
- Supports and limits: Saved notebook metadata and output types were parsed without copying cell output. Partial execution state is present; it does not establish a completed inference run or accepted submission.

## DEEPFAKE-3

- Record: `AIContest/deepfake/deepfake/task(less_cpu_intensive_ver).ipynb`
- Evidence type: alternative-notebook-state.
- SHA-256: `75f947e2c4e78885d93665c9523108f03783b3fd1a42e8bbe6c29689fd03d9e2`
- Supports and limits: An alternative notebook is labeled as less CPU-intensive. No saved executed-cell/output state was established in this snapshot. No speed improvement is asserted.

## Review boundary

No training, inference, official submission, remote process, or performance benchmark was rerun for this account. Coding-agent attribution is stated only when the records identify it. General methodological descriptions do not grant redistribution rights to the excluded code, data, model, supplied template, or team material.
