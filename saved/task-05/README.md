# Saved Models — Task 05

Model checkpoints from Colab training on Amazon Electronics dataset.
All files are stored on Google Drive due to size.

[Download from Google Drive](https://drive.google.com/drive/folders/1VsE6D2fZWdVtQRbxhi2RVXW3I6AjTsAs)

| File                             | Model    | Status  |
| -------------------------------- | -------- | ------- |
| `NeuMF-Apr-30-2026_15-35-41.pth` | NeuMF | trained |
| `LightGCN-May-05-2026_17-43-28.pth` | LightGCN | trained |
| `SASRec-May-05-2026_22-11-25.pth` | SASRec | trained |
| `ItemKNN-May-01-2026_08-35-28.pth` | ItemKNN | trained |
| `DeepFM-May-06-2026_08-56-42.pth` | DeepFM | trained |

## How to Load

```python
import torch

checkpoint = torch.load('NeuMF-Apr-30-2026_15-35-41.pth', map_location='cpu')
```
