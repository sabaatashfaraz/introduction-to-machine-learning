# Homework 1 — Bayesian Inference and Probabilistic Models

This notebook explores probabilistic inference and classical machine-learning ideas through a set of small implementation problems.

## Topics
- Bayesian updating for Bernoulli observations with a Beta prior.
- Beta–Binomial updating when only aggregate counts are observed.
- Maximum-likelihood (ML) and maximum-a-posteriori (MAP) estimation for a discrete distribution.
- Multivariate Gaussian modeling, missing-value imputation, and Hinton-diagram visualization.
- Decision-tree classification and decision-surface visualization.
- Linear-Gaussian sensor fusion using means, covariances, and precision matrices.
- Bayesian networks and conditional-independence structure.
- Missing-token prediction using statistical language models (unigram, bigram, and trigram).

## Notebook
`homework_01.ipynb`

The notebook reports the following held-out missing-token accuracies for its n-gram comparison: unigram 0.0000, bigram 0.2640, and trigram 0.2160. These are the results recorded in the notebook, not independently rerun during repository packaging.

## Input files
The original notebook references files under `datasets/` and `dataset/`, including:
- `p1_1.json`, `p1_3.json`
- `p1_5_animal_species.csv`, `p1_5_test.csv`
- `p1_6_sensor_data.npz`
- `causal_stock_data.csv`
- `p3_train.json`, `p3_test.json`
- `p1_4_train.npz`, `p1_4_test_missing.npz`, `p1_4_test_full.npz`

These source files were not included in the uploaded notebook and are not bundled here. See `datasets/README.md`.
