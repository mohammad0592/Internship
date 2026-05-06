# Task 05 Results

## Task Scope

- Task ID: `task-05`
- Dataset: Amazon Electronics (`amazon`)
- Models: NeuMF, LightGCN, SASRec, ItemKNN, DeepFM
- Environment: Google Colab (GPU — CUDA)
- Colab notebook: [Open in Colab](https://colab.research.google.com/drive/1cqy5GHZyBcjA_non-lwXrlZ0SvEmBN8e#scrollTo=rqhpcBURVriJ)

---

## Model 1 — NeuMF

### Run `neumf-amazon-2026-04-30-15-35-22`

- Date: `2026-04-30`
- Primary metric: `MRR@10`
- Best valid: `MRR@10 = 0.2857`
- Test: `MRR@10 = 0.2869`

**Validation metrics:**

| Metric | @10 | @20 |
|---|---:|---:|
| `recall` | 0.5035 | 0.6170 |
| `mrr` | 0.2857 | 0.2935 |
| `ndcg` | 0.3329 | 0.3620 |
| `hit` | 0.5190 | 0.6321 |
| `precision` | 0.0536 | 0.0330 |

**Test metrics:**

| Metric | @10 | @20 |
|---|---:|---:|
| `recall` | 0.5046 | 0.6186 |
| `mrr` | 0.2869 | 0.2947 |
| `ndcg` | 0.3341 | 0.3633 |
| `hit` | 0.5204 | 0.6336 |
| `precision` | 0.0537 | 0.0331 |

**Artifacts:**

- Log: `log/NeuMF/NeuMF-amazon-Apr-30-2026_15-35-22-1a3724.log`
- Checkpoint: `saved/task-05/` — [Download from Google Drive](https://drive.google.com/drive/folders/1VsE6D2fZWdVtQRbxhi2RVXW3I6AjTsAs)
- TensorBoard: `log_tensorboard/task-05/`

---

## Model 2 — LightGCN

### Run `lightgcn-amazon-2026-05-05-17-43-04`

- Date: `2026-05-05`
- Primary metric: `MRR@10`
- Best valid: `MRR@10 = 0.3320`
- Test: `MRR@10 = 0.3340`

**Validation metrics:**

| Metric | @10 | @20 |
|---|---:|---:|
| `recall` | 0.5823 | 0.7092 |
| `mrr` | 0.3320 | 0.3407 |
| `ndcg` | 0.3865 | 0.4192 |
| `hit` | 0.5983 | 0.7236 |
| `precision` | 0.0618 | 0.0379 |

**Test metrics:**

| Metric | @10 | @20 |
|---|---:|---:|
| `recall` | 0.5839 | 0.7103 |
| `mrr` | 0.3340 | 0.3427 |
| `ndcg` | 0.3885 | 0.4210 |
| `hit` | 0.5999 | 0.7249 |
| `precision` | 0.0620 | 0.0379 |

**Artifacts:**

- Log: `log/LightGCN/LightGCN-amazon-May-05-2026_17-43-04-62a802.log`
- Checkpoint: `saved/task-05/` — [Download from Google Drive](https://drive.google.com/drive/folders/1VsE6D2fZWdVtQRbxhi2RVXW3I6AjTsAs)
- TensorBoard: `log_tensorboard/task-05/`

---

## Model 3 — SASRec

### Run `sasrec-amazon-2026-05-05-22-11-21`

- Date: `2026-05-05`
- Primary metric: `MRR@10`
- Best valid: `MRR@10 = 0.2311`
- Test: `MRR@10 = 0.2184`

**Validation metrics:**

| Metric | @10 | @20 |
|---|---:|---:|
| `recall` | 0.4353 | 0.5452 |
| `mrr` | 0.2311 | 0.2386 |
| `ndcg` | 0.2790 | 0.3068 |
| `hit` | 0.4367 | 0.5467 |
| `precision` | 0.0437 | 0.0274 |

**Test metrics:**

| Metric | @10 | @20 |
|---|---:|---:|
| `recall` | 0.4087 | 0.5158 |
| `mrr` | 0.2184 | 0.2258 |
| `ndcg` | 0.2632 | 0.2903 |
| `hit` | 0.4090 | 0.5162 |
| `precision` | 0.0409 | 0.0258 |

**Artifacts:**

- Log: `log/SASRec/SASRec-amazon-May-05-2026_22-11-21-adf152.log`
- Checkpoint: `saved/task-05/` — [Download from Google Drive](https://drive.google.com/drive/folders/1VsE6D2fZWdVtQRbxhi2RVXW3I6AjTsAs)
- TensorBoard: `log_tensorboard/task-05/`

---

## Model 4 — ItemKNN

### Run `itemknn-amazon-2026-05-01-08-34-50`

- Date: `2026-05-01`
- Primary metric: `MRR@10`
- Best valid: `MRR@10 = 0.0612`
- Test: `MRR@10 = 0.0628`

**Validation metrics:**

| Metric | @10 | @20 |
|---|---:|---:|
| `recall` | 0.2605 | 0.4756 |
| `mrr` | 0.0612 | 0.0753 |
| `ndcg` | 0.1064 | 0.1597 |
| `hit` | 0.2608 | 0.4762 |
| `precision` | 0.0261 | 0.0238 |

**Test metrics:**

| Metric | @10 | @20 |
|---|---:|---:|
| `recall` | 0.2656 | 0.4858 |
| `mrr` | 0.0628 | 0.0772 |
| `ndcg` | 0.1088 | 0.1633 |
| `hit` | 0.2657 | 0.4859 |
| `precision` | 0.0266 | 0.0243 |

**Artifacts:**

- Log: `log/ItemKNN/ItemKNN-amazon-May-01-2026_08-34-50-08ac86.log`
- Checkpoint: `saved/task-05/` — [Download from Google Drive](https://drive.google.com/drive/folders/1VsE6D2fZWdVtQRbxhi2RVXW3I6AjTsAs)
- TensorBoard: `log_tensorboard/task-05/`

---

## Model 5 — DeepFM

### Run `deepfm-amazon-2026-05-06-08-56-21`

- Date: `2026-05-06`
- Primary metric: `AUC`
- Best valid: `AUC = 0.6810`
- Test: `AUC = 0.6844`

> **Note:** DeepFM ran in CTR/rating-prediction mode, so it reports `AUC` and `LogLoss` instead of ranking metrics like `MRR` and `Recall`. It is not directly comparable to the other four models in the summary table below.

**Validation metrics:**

| Metric | Value |
|---|---:|
| `auc` | 0.6810 |
| `logloss` | 0.7723 |

**Test metrics:**

| Metric | Value |
|---|---:|
| `auc` | 0.6844 |
| `logloss` | 0.7711 |

**Artifacts:**

- Log: `log/DeepFM/DeepFM-amazon-May-06-2026_08-56-21-bfdf72.log`
- Checkpoint: `saved/task-05/` — [Download from Google Drive](https://drive.google.com/drive/folders/1VsE6D2fZWdVtQRbxhi2RVXW3I6AjTsAs)
- TensorBoard: `log_tensorboard/task-05/`

---

## Summary Comparison

> Rankings metrics only. DeepFM used a different evaluation mode (CTR) and is excluded from this table — see its section above for its AUC and LogLoss results.

| Model | Valid MRR@10 | Test MRR@10 | Valid NDCG@10 | Test NDCG@10 | Valid Recall@10 | Test Recall@10 |
|---|---:|---:|---:|---:|---:|---:|
| LightGCN | 0.3320 | 0.3340 | 0.3865 | 0.3885 | 0.5823 | 0.5839 |
| NeuMF | 0.2857 | 0.2869 | 0.3329 | 0.3341 | 0.5035 | 0.5046 |
| SASRec | 0.2311 | 0.2184 | 0.2790 | 0.2632 | 0.4353 | 0.4087 |
| ItemKNN | 0.0612 | 0.0628 | 0.1064 | 0.1088 | 0.2605 | 0.2656 |
| DeepFM | — | — | — | — | — | — |
