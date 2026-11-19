# Homework 4 — Neural Networks and Kernel Methods

This assignment compares neural-network architectures and kernel-based methods across tabular, image, and regression tasks.

## Problem 1 — Multilayer Perceptron
- Load and explore a real tabular dataset.
- Establish a linear baseline.
- Implement an MLP from scratch with NumPy.
- Perform gradient checking.
- Compare activation functions, initialization strategies, and regularization.

## Problem 2 — Convolutional Neural Networks
- Study convolution, padding, stride, and receptive fields.
- Build PyTorch data loaders for handwritten-digit images.
- Compare a flattened MLP with a small CNN.
- Design a stronger CNN under a parameter budget.
- Perform error analysis and robustness tests under distribution shift.

## Problem 3 — Kernel Methods
- Construct and inspect Gram matrices and positive-semidefinite properties.
- Compare linear, polynomial, and RBF SVM kernels.
- Fit Gaussian Process Regression models to the diabetes dataset.
- Explore scalability and approximate kernels with Nyström features.
- Explore active sampling with a Gaussian Process.

## Notebook
`homework_04.ipynb`

## Data
The uploaded archive included processed splits derived from scikit-learn's breast-cancer, digits, wine, and diabetes datasets. They are not copied into this repository; see `data/README.md` for the original file inventory and sources.
