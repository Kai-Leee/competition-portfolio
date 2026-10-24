# Tools and What Their Use Establishes

This index records each tool's role and the evidence for its use. An import proves an implementation dependency; a proposal proves intent. Neither establishes a successful run. Execution claims rely on the linked historical records.

## Modeling and implementation

| Project | Tools or components | Recorded role and verification boundary |
|---|---|---|
| [ETRI](competitions/etri-human-understanding/EVIDENCE.md) | Python, NumPy, LightGBM, CatBoost | Feature/model experiments and out-of-fold comparisons. Baseline dependencies are inspected; historical logs support ablations. Final platform performance remains unresolved. [TOOLS-ETRI](#tools-etri) |
| [Wind power](competitions/wind-power/EVIDENCE.md) | Python training/evaluation pipeline, CatBoost, experiment registry | Shared comparisons and experiment lifecycle. Registry ideas are not all completed successful runs. |
| [DeepVoice](competitions/deepvoice/EVIDENCE.md) | Python, PyTorch, torchaudio, librosa, NumPy, safetensors; MuQ, MelBand-RoFormer, PANNs | Audio preparation, frozen features, learned heads, separation, presence detection. Variant imports and the component audit have different scopes; inactive components are not claimed as contributors. |
| [Procurement compliance](competitions/procurement-compliance/EVIDENCE.md) | Python span extraction and rule gates; vLLM adapter | Local evidence selection and output checks are recorded. An implemented vLLM interface does not establish successful fixed-model GPU inference. [TOOLS-PPS](#tools-pps) |
| [SCPC AI](competitions/scpc-ai/EVIDENCE.md) | Python, structured JSON, deterministic compiler | Policy-answer construction and cross-field checks. Hidden performance remains unverified. |
| [Deepfake detection](competitions/deepfake-detection/EVIDENCE.md) | PyTorch, Transformers, dlib, OpenCV, Pillow, multiprocessing | Inspected face/frame preparation and classifier implementation. Complete execution and speed gains remain unverified. |
| [Satellite segmentation](historical-work/satellite-segmentation-2023/EVIDENCE.md) | PyTorch, Albumentations, OpenCV, run-length encoding | Historical segmentation notebooks. Interrupted execution does not establish a completed result or exact event identity. |
| [Agricultural forecasting](preparations/agricultural-price-forecasting/EVIDENCE.md) | Proposed Jev integration and forecasting candidates | Research/preparation only. API integration and model execution were not verified. |

Microstructure and vessel-matching solution tools remain outside this public account during sharing review. Wildfire artifacts do not support a tool or method narrative.

## Coding-agent workflow

| Project | Tool or mechanism | What was observed |
|---|---|---|
| Wind power | Codex and Claude provider stages | Both succeeded in one archived read-only verification smoke. A separate production implementation run failed. These records do not establish a general success rate. |
| DeepVoice | Agent entry points, question/run records, replay and review artifacts | Task routing and evidence-linked work are documented. Provider identity and independent scoring are not asserted for every run. |
| ETRI / procurement / SCPC | Role instructions, rulebooks, explicit implementation/review targets | Workspace structures support the workflow. Their existence does not prove universal adherence or autonomous completion. |
| Financial disclosure | Agent-assisted source/semantic review | Review lessons are documented at high level. Team implementation, detailed traces, and internal metrics remain withheld. |

## Portfolio curation tools

File discovery used `fd`; text inspection used `rg`; code-structure inspection used `sg`. Context-mode processed records into bounded summaries. SHA-256 fingerprints identify the source snapshots.

`git`, GitHub CLI (`gh`), Markdown link checks, and Gitleaks support publication verification. These checks address repository contents and release integrity; they do not validate historical model results or settle all redistribution rights.

For the separately authorized local cleanup, `dust`, process inspection, and `lsof` narrowed deletion to unused pip download caches. Active environments and experiment payloads were retained. Local paths and the deletion receipt remain private.

## Additional source fingerprints

Paths identify excluded source snapshots, not distributed files. Hashes do not prove authorship or successful execution. Review date: October 24, 2026.

### TOOLS-ETRI

- Record: `Daycon/ETRI/scripts/train_baseline.py`
- SHA-256: `10593e6a8bee687cf2a29a35592f4c19e84f1bfc1343b07e6455718df77b4907`
- Supports: Python/NumPy and model dependencies in the inspected implementation. Execution claims rely on separate logs in the ETRI case.

### TOOLS-PPS

- Record: `contest/pps-compliance/src/pps/llm.py`
- SHA-256: `edcdf6282e7cd554d33087f7aed0743b29a45806c1724c8697aebb557c56c123`
- Supports: implemented model-client/vLLM adapter; successful GPU execution was not established.
