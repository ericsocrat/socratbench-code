# SocratBench Code v0.2 — cross-round publication package

Seven local models were evaluated on three repository tasks under a 65,536-token context target, 1,800-second task budget, network-disabled Docker isolation, and one valid attempt per model/task.

The central result is simple: **one full PASS across 21 observed official model-task outcomes**. Ornith 1.5 9B passed C10; no model passed C08 or C09.

These are 21 observed outcomes from three tasks in one repository on one local machine. They are not a population estimate or a general coding leaderboard.

## Package map

- `report.html` — portable reader-facing report.
- `PUBLICATION_BRIEF.md` — recommended story and release sequence.
- `METHODS.md`, `RESULTS.md`, `LIMITATIONS.md`, `PROVENANCE.md` — evidence and caveats.
- `X_STORY_NOTES.md`, `X_DRAFTS.md` — owner-review drafts; nothing was posted.
- `cross-round-results.*`, `model-task-matrix.csv`, `model-summary.csv`, `task-summary.csv` — public datasets.
- `publication-assets/` — seven 2400×1350 PNG/SVG graphics.
- `qa/` — numeric, visual, and leakage checks.

## Result matrix

| Model | C08 | C09 | C10 | Observed record | Timeouts |
|---|---:|---:|---:|---:|---:|
| M01 — GPT-OSS 20B | FAIL | FAIL | FAIL | 0 PASS / 3 FAIL | 0 |
| M02 — GLM-4.7-Flash | FAIL | FAIL | FAIL | 0 PASS / 3 FAIL | 2 |
| M03 — North Mini Code 1.0 | FAIL | FAIL | FAIL | 0 PASS / 3 FAIL | 1 |
| M04 — Ornith 1.5 9B | FAIL | FAIL | PASS | 1 PASS / 2 FAIL | 2 |
| M05 — Laguna XS 2.1 | FAIL | FAIL | FAIL | 0 PASS / 3 FAIL | 1 |
| M06 — Qwen3-Coder 30B | FAIL | FAIL | FAIL | 0 PASS / 3 FAIL | 1 |
| M07 — IBM Granite 4.2 8B | FAIL | FAIL | FAIL | 0 PASS / 3 FAIL | 3 |
