# Dataset README

## Dataset Used
**Scikit-learn Digits Dataset** (`sklearn.datasets.load_digits`)

## How the Dataset is Obtained
The dataset is loaded directly via scikit-learn's built-in `load_digits()` function. No manual downloads or external files are needed — it ships with the scikit-learn package.

## Description
- **Samples:** 1,797 images of handwritten digits (0–9)
- **Features:** 64 (each image is 8×8 grayscale pixels, flattened)
- **Pixel range:** 0–16 (integer valued)
- **Classes:** 10 (digits 0 through 9)

## How it is Used
The dataset is used in `task_2_1.ipynb` through `task_3_2.ipynb` as a toy testbed for evaluating arc-cosine kernels from the paper "Kernel Methods for Deep Learning" (Cho & Saul, NIPS 2009). The data is:
1. Normalized to [0, 1] using MinMaxScaler
2. Split into train (55%), validation (15%), and test (30%) sets with stratified sampling
3. Random seed = 42 for reproducibility
