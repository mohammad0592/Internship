# Task 04 Results

## Task Scope

- Task ID: `task-04`
- Model: `BPR`
- Dataset: Amazon Electronics (`amazon`)
- Environment: Google Colab (GPU — CUDA)
- Colab notebook: [Open in Colab](https://colab.research.google.com/drive/1zoG-qIQw7SwEzScaJ09t1HyNrhcKqp5u#scrollTo=qfTY61Lry_AA)

## Configuration

```python
run_recbole(
    model='BPR',
    dataset='amazon',
    config_dict={
        "epochs": 80,
        "train_batch_size": 8192,
        "learning_rate": 0.0003,
        "embedding_size": 256,
        "reg_weight": 1e-6,
        "train_neg_sample_args": {"uniform": 2},
        "stopping_step": 10,
        "topk": [10, 20],
        "metrics": ["Recall", "MRR", "NDCG", "Hit", "Precision"],
        "min_user_inter_num": 5,
        "min_item_inter_num": 5,
        "eval_args": {
            "split": {"RS": [80, 10, 10]},
            "group_by": "user",
            "order": "RO",
            "mode": "uni100"
        },
        "eval_batch_size": 131072,
        "eval_step": 5,
        "worker": 8
    }
)
```

## Runs

### Run `bpr-amazon-2026-04-29-20-26-44`

- Date: `2026-04-29`
- Primary metric: `MRR@10`
- Best valid: `MRR@10 = 0.3174`
- Test: `MRR@10 = 0.3187`

**Validation metrics:**

| Metric | @10 | @20 |
|---|---:|---:|
| `recall` | 0.5550 | 0.6800 |
| `mrr` | 0.3174 | 0.3260 |
| `ndcg` | 0.3687 | 0.4009 |
| `hit` | 0.5708 | 0.6943 |
| `precision` | 0.0592 | 0.0365 |

**Test metrics:**

| Metric | @10 | @20 |
|---|---:|---:|
| `recall` | 0.5565 | 0.6816 |
| `mrr` | 0.3187 | 0.3272 |
| `ndcg` | 0.3701 | 0.4022 |
| `hit` | 0.5724 | 0.6959 |
| `precision` | 0.0593 | 0.0366 |

**Artifacts:**

- Log: `log/BPR/amazon/BPR-amazon-Apr-29-2026_20-26-44-d45172.log`
- Checkpoint: `saved/task-04/` — [Download from Google Drive](https://drive.google.com/drive/folders/1WJl1ok6tqBZucVllqSPvcPOlDx0lKnFc)
- TensorBoard: `log_tensorboard/task-04/`
