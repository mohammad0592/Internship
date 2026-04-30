# Saved Models — Task 03

Model checkpoints from local training runs on `ml-100k`.

| File | Run | Size |
|---|---|---|
| `BPR-Apr-26-2026_21-37-30.pth` | `bpr-ml100k-2026-04-26-21-37-30` | 1.93 MB |
| `BPR-Apr-26-2026_21-31-48.pth` | `bpr-ml100k-2026-04-26-21-31-47` | 1.93 MB |

## How to Load

```python
import torch

checkpoint = torch.load('BPR-Apr-26-2026_21-37-30.pth', map_location='cpu')
```
