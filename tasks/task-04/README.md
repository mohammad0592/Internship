# Task 04

Training a recommender system on a real-world large-scale dataset: **Amazon Electronics**.

## Why Colab?

The Amazon Electronics dataset is significantly larger than `ml-100k`.
Local training was performed in **Google Colab** to leverage GPU resources.

## Colab Notebook

[Open in Google Colab](https://colab.research.google.com/drive/1zoG-qIQw7SwEzScaJ09t1HyNrhcKqp5u#scrollTo=qfTY61Lry_AA)

## What the Notebook Does

1. Downloads the Amazon Electronics dataset via RecSysDatasets
2. Converts the dataset into RecBole format
3. Trains the model using RecBole
4. Saves results and metrics

## Model & Dataset

- Model: `BPR`
- Dataset: Amazon Electronics (`amazon`)
- Framework: RecBole
- Environment: Google Colab (GPU — CUDA)

## Related Artifacts

- Results: `docs/tasks/task-04-results.md`
- Saved model: `saved/task-04/README.md`
