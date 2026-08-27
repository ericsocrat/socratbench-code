# Methods

## Environment

- Local supervised benchmark on one Windows 11 machine.
- Intel Core i9-9900K; 32 GB system RAM.
- NVIDIA RTX 3070 Ti with 8 GB VRAM.
- Local Ollama model tags listed in the datasets.
- Hermes Agent candidate runner with fresh per-run state.

## Candidate protocol

- 65,536-token context target.
- 1,800-second candidate coding budget per task.
- One valid official attempt per model/task.
- Network disabled.
- Writable candidate workspace in Docker.
- Candidate-visible tools limited to `clarify`, `process`, `terminal`, and `todo`.
- Zero candidate skills.
- Hidden verification remained controller-only.

## Tasks and scoring

- Round 1: C08 and C09.
- Round 2: C10.
- Official outcomes use each task's frozen hard-gate contract.
- Public and hidden check counts are shown only within their own task; raw counts are not pooled across different denominators.
- Infrastructure-invalid pre-score launches do not count as model-quality outcomes.
- Failed models are not secondarily ranked unless an existing frozen rule permits it.

## Special cases

- M01's valid replacements are used; excluded pre-score incidents remain part of the audit trail.
- M07 entered Round 1 through a separately frozen, technically comparable late-entry extension.
- M05/C10 is a valid terminal policy-derived FAIL after a candidate-caused SQL scoring error; no new attempt or inference was created during adjudication.
- M06's unavailable `search_files` and `read_file` calls were denied; those capabilities were not exposed.
