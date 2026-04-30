# Saved Models — Task 04

Model checkpoint from Colab training on Amazon Electronics dataset.

| File | Run | Size | Location |
|---|---|---|---|
| `BPR-Apr-29-2026_20-27-04.pth` | `bpr-amazon-2026-04-29-20-26-44` | 748 MB | Google Drive |

## Download

[Download from Google Drive](https://drive.google.com/drive/folders/1WJl1ok6tqBZucVllqSPvcPOlDx0lKnFc)

## How to Load

```python
import torch

checkpoint = torch.load('BPR-Apr-29-2026_20-27-04.pth', map_location='cpu')
```
