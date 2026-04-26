# Task 03 Results

## Task Scope

- Task ID: `task-03`
- Model: `BPR`
- Dataset: `ml-100k`
- Script: `tasks/task-03/run.py`
- Compatibility script: `run.py`

## Runs

### Run `bpr-ml100k-2026-04-26-21-37-30`

- Best epoch: `50`
- Best valid: `MRR@10 = 0.3893`
- Test: `MRR@10 = 0.4895`
- Log: `log/BPR/BPR-ml-100k-Apr-26-2026_21-37-30-c13701.log`

### Run `bpr-ml100k-2026-04-26-21-31-47`

- Best epoch: `50`
- Best valid: `MRR@10 = 0.3893`
- Test: run was interrupted after epoch 61 — no final test evaluation was printed
- Valid metrics at epoch 50:
  - `recall@10`: 0.2085
  - `mrr@10`: 0.3893
  - `ndcg@10`: 0.2302
  - `hit@10`: 0.7402
  - `precision@10`: 0.1583
- Log: `log/BPR/BPR-ml-100k-Apr-26-2026_21-31-47-c13701.log`

## Task 03 Git Tracking

- Recommended commit title: `task-03: baseline BPR run + docs update`
- Push target: `origin/main`
