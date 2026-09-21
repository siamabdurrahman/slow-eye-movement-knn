# Slow Eye Movement Detection with K Nearest Neighbours

Research code and data for classifying slow eye movement events using a K-nearest-neighbours (KNN) workflow in Python.

[![Preprint](https://img.shields.io/badge/TechRxiv-10.36227%2Ftechrxiv.176704421.12448344-1f6feb)](https://doi.org/10.36227/techrxiv.176704421.12448344)
![Python](https://img.shields.io/badge/Python-3.x-3776AB)
![Research](https://img.shields.io/badge/Type-Research%20Project-6f42c1)

## Research objective

This undergraduate research project investigates whether KNN can distinguish slow-eye-movement and non-slow-eye-movement signal samples. The repository preserves the dataset split, exploratory scripts, model evaluation, and a small Tkinter interface used during development.

## Repository contents

| File | Purpose |
| --- | --- |
| `SEMs Senior.py` | Original signal visualisation and KNN evaluation workflow |
| `Data Display KNN.py` | Consolidated plots and comparison of K values from 1 to 25 |
| `GUI.py` | Desktop interface for loading MATLAB files, training KNN, and reporting accuracy |
| `Train_x.mat`, `Train_y.mat` | Training features and labels |
| `test_x.mat`, `test_y.mat` | Evaluation features and labels |

## Method overview

1. Load feature matrices and labels from MATLAB `.mat` files.
2. Inspect representative signals visually.
3. Train KNN classifiers across a range of neighbourhood sizes.
4. Compare accuracy, macro precision, macro recall, and macro F1.
5. Report the selected five-neighbour model and visualise metric sensitivity to `k`.

## Reproducing the analysis

Create a Python environment and install:

```bash
pip install numpy scipy matplotlib scikit-learn
```

The original analysis scripts contain local Windows paths retained for research provenance. Before running them, replace those paths with the location of the four `.mat` files in your clone. Alternatively, use `GUI.py` and select the repository folder when prompted.

```bash
git clone https://github.com/siamabdurrahman/Research-on-Slow-Eye-Movement-Based-on-KNN-Algorithm.git
cd Research-on-Slow-Eye-Movement-Based-on-KNN-Algorithm
python GUI.py
```

> The GUI login screen is a demonstration interface and does not implement authentication.

## Research output

A. R. Siam, “Slow Eye Movement Detection Using K-Nearest Neighbour Classification,” *TechRxiv*, 2025. [https://doi.org/10.36227/techrxiv.176704421.12448344](https://doi.org/10.36227/techrxiv.176704421.12448344)

Machine-readable citation metadata is provided in `CITATION.cff`.

## Scope and limitations

This repository documents an academic prototype. Its original fixed train/evaluation split and path-dependent scripts should be modernised before comparative or production use. Results should be interpreted within the supplied dataset and experimental design.

## Author

**Abdur Rahman Siam**  
Research interests: explainable AI, multimodal sensing, digital health, privacy-preserving machine learning, and IoT security.

- [ORCID](https://orcid.org/0009-0002-5904-9477)
- [LinkedIn](https://www.linkedin.com/in/abdur-rahman-siam-86a705353)
