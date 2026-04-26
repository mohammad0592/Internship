# Results Index

This is the **master summary table** across all tasks and runs.
For detailed results of each task, see `docs/tasks/task-XX-results.md`.
For cross-task comparisons, see `docs/comparisons/`.

## Summary Table

| Run ID | Date | Task | Model | Dataset | Primary Valid Metric | Primary Test Metric | Best Epoch | Details |
|---|---|---|---|---|---:|---:|---:|---|
| `bpr-ml100k-2026-04-26-21-37-30` | 2026-04-26 | `task-03` | BPR | ml-100k | `MRR@10 = 0.3893` | `MRR@10 = 0.4895` | 50 | [task-03](tasks/task-03-results.md) |
| `bpr-ml100k-2026-04-26-21-31-47` | 2026-04-26 | `task-03` | BPR | ml-100k | — | — | 50 | [task-03](tasks/task-03-results.md) |

## How To Add New Runs

1. Run the experiment and save the log in `log/`.
2. Add one row to the summary table above.
3. Add full details in `docs/tasks/task-XX-results.md`.
4. For cross-task comparisons, create a file in `docs/comparisons/`.
