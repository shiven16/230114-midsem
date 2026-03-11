# Dataset Description

## Overview

The experiments in this project use a synthetic dataset generated using the `make_blobs` function from the `scikit-learn` library. This dataset is used to simulate clustering scenarios suitable for evaluating Gaussian Mixture Models and the constrained clustering method proposed in the paper.

The dataset is generated programmatically inside the notebooks and therefore no external dataset files are required.

---

## Dataset Generation

The dataset is generated using the following code:

```python
from sklearn.datasets import make_blobs

X, y_true = make_blobs(
    n_samples=300,
    centers=3,
    cluster_std=5.0,
    random_state=42
)