# Results

## Headline

One of 21 observed official model-task outcomes passed its frozen hard gate.

| Model | C08 | C09 | C10 | Observed record | Timeouts |
|---|---:|---:|---:|---:|---:|
| M01 — GPT-OSS 20B | FAIL | FAIL | FAIL | 0 PASS / 3 FAIL | 0 |
| M02 — GLM-4.7-Flash | FAIL | FAIL | FAIL | 0 PASS / 3 FAIL | 2 |
| M03 — North Mini Code 1.0 | FAIL | FAIL | FAIL | 0 PASS / 3 FAIL | 1 |
| M04 — Ornith 1.5 9B | FAIL | FAIL | PASS | 1 PASS / 2 FAIL | 2 |
| M05 — Laguna XS 2.1 | FAIL | FAIL | FAIL | 0 PASS / 3 FAIL | 1 |
| M06 — Qwen3-Coder 30B | FAIL | FAIL | FAIL | 0 PASS / 3 FAIL | 1 |
| M07 — IBM Granite 4.2 8B | FAIL | FAIL | FAIL | 0 PASS / 3 FAIL | 3 |

## Task outcomes

| Task | Models | PASS | FAIL | Timeout | Normal completion |
|---|---:|---:|---:|---:|---:|
| C08 | 7 | 0 | 7 | 5 | 2 |
| C09 | 7 | 0 | 7 | 3 | 4 |
| C10 | 7 | 1 | 6 | 2 | 5 |

## Interpretation

- Ornith 1.5 9B is the only model with an observed full PASS, on C10.
- No model passed C08 or C09.
- Model size did not determine success on this hardware: Qwen3-Coder 30B did not pass any of the three tasks.
- Completion was not equivalent to correctness. Several normal completions still failed verification.
- Ten outcomes timed out, including every Granite task.

These are 21 observed outcomes from three tasks in one repository on one local machine. They are not a population estimate or a general coding leaderboard.
