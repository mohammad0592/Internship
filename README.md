# Recommender Systems — Learning Experiments

Experiments in recommender systems using RecBole, covering multiple tasks and datasets.

## Repository Structure

```
code/
├── tasks/                  # One folder per task
│   ├── task-03/            # Local training on ml-100k
│   │   ├── run.py
│   │   └── README.md
│   └── task-04/            # Colab training on Amazon Electronics
│       └── README.md
├── colab/                  # Colab notebooks
├── docs/
│   ├── results.md          # Master summary table (all tasks, all runs)
│   ├── tasks/              # Detailed results per task
│   │   ├── task-03-results.md
│   │   └── task-04-results.md
│   ├── comparisons/        # Cross-task comparisons
│   └── templates/
│       └── experiment-template.md
├── log/                    # Training logs
│   └── BPR/
├── log_tensorboard/        # TensorBoard runs
├── saved/                  # Model checkpoints
│   ├── task-03/            # Tracked in git (small)
│   └── task-04/            # Stored on Google Drive (748 MB)
├── run.py
└── requirements.txt
```

## Setup

```bash
pip install -r requirements.txt
```

## Tasks

| Task | Dataset | Model | Environment | Results |
|---|---|---|---|---|
| task-03 | ml-100k | BPR | Local | [results](docs/tasks/task-03-results.md) |
| task-04 | Amazon Electronics | BPR | Google Colab | [results](docs/tasks/task-04-results.md) |
