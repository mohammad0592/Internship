# Recommender Learning Experiments

This is a learning repository for running and documenting recommender-system experiments.

The goal is to keep three things clear:

1. What code was run.
2. What configuration was used.
3. What results were produced.

## Current Baseline

- Framework: `RecBole`
- Script: `tasks/task-03/run.py`
- Model: `BPR`
- Dataset: `ml-100k`
- Task ID: `task-03`

## Repository Structure

```
code/
├── tasks/                  # One folder per task, contains code + task README
│   ├── task-03/
│   │   ├── run.py
│   │   └── README.md
│   └── task-XX/            # Future tasks go here
├── docs/
│   ├── results.md          # Master summary table (all tasks, all runs)
│   ├── tasks/              # Detailed results per task
│   │   └── task-03-results.md
│   ├── comparisons/        # Cross-task comparison files go here
│   └── templates/
│       └── experiment-template.md
├── log/                    # Raw logs, organized by model (tracked by git)
│   └── BPR/
├── log_tensorboard/        # TensorBoard runs, organized by task (git-ignored)
│   └── task-03/
├── saved/                  # Model checkpoints, organized by task (git-ignored)
│   └── task-03/
├── run.py                  # Compatibility launcher → delegates to current task
└── requirements.txt
```

## Setup

```bash
pip install -r requirements.txt
```

## Run Baseline

```bash
python tasks/task-03/run.py
```

Compatibility command:

```bash
python run.py
```

## Documentation Workflow (For Every New Experiment)

1. Run the experiment script.
2. Save/keep the generated log file in `log/`.
3. Add one row to `docs/results.md` with:
   - run id/date
   - task/model/dataset
   - primary validation metric
   - primary test metric
   - log path
4. Add/update `docs/tasks/task-XX-results.md` for task-specific details.
5. If the run is important, add a full section using `docs/templates/experiment-template.md`.

## Commit And Push Per Task

Use task-prefixed commits so history is clearly separated:

```bash
git add .
git commit -m "task-03: baseline BPR run + docs update"
git push origin main
```

Optional task tag:

```bash
git tag task-03-baseline-2026-04-26
git push origin task-03-baseline-2026-04-26
```

## Naming Convention (Recommended)

- Script: `run_<task>.py` (example: `run_bpr_lr_sweep.py`)
- Log file: `<task>-<dataset>-<date>_<time>.log`
- Run id: `<task>-<dataset>-<timestamp>`
