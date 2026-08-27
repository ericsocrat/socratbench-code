# Limitations

- Three tasks from one repository are too small and narrow for general model ranking.
- Results depend on one physical machine, local quantization, serving configuration, and an 8 GB GPU.
- Each model received one valid attempt per task; this measures observed pass@1-like behavior, not best-of-N potential.
- Task-specific public and hidden denominators differ and cannot be pooled into one accuracy percentage.
- Hidden verification improves resistance to overfitting but limits what can be disclosed publicly.
- Timeout behavior mixes model speed, local offload constraints, planning, and tool-use efficiency.
- M07's Round-1 results are a separately frozen late-entry extension, not part of the original six-model execution order.
- M05/C10 is policy-derived from preserved evidence after a candidate-caused scoring error and must retain that label.
- Two Round-2 evidence records contain stale internal plan-reference labels; verified hashes bind the correct v9/v10 plan bytes. This is a documentation caveat, not a result-integrity defect.

## Safe conclusion

These are 21 observed outcomes from three tasks in one repository on one local machine. They are not a population estimate or a general coding leaderboard.
