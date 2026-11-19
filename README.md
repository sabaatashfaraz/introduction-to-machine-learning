# Introduction to Machine Learning — Coursework Portfolio

A collection of individual coursework notebooks and a team course project completed for **Introduction to Machine Learning** at **Sharif University of Technology, Department of Electrical Engineering**.

This repository is organized as a learning portfolio: it starts with probabilistic inference and optimization, progresses through regression, discriminant analysis, neural networks, kernel methods, and clustering, and concludes with a sequence-anomaly-detection project using Hidden Markov models.

**Author:** Saba Atashfaraz  
**Course:** Introduction to Machine Learning  
**Institution:** Sharif University of Technology  
**Term:** 1404–2 / Spring 2026

---

## Coursework at a glance

| Work | Main topics |
|---|---|
| [Homework 1 — Bayesian Inference](assignments/01-bayesian-inference-and-probabilistic-models/) | Beta–Bernoulli and Beta–Binomial inference, ML/MAP estimation, multivariate Gaussian imputation, decision trees, sensor fusion, Bayesian networks, n-gram language models |
| [Homework 2 — Optimization](assignments/02-optimization-and-constrained-learning/) | Saddle-point optimization, gradient and Newton methods, Armijo–Goldstein line search, KL divergence, Cholesky parameterization, KKT conditions, exterior penalty methods |
| [Homework 3 — Regression & Generative Models](assignments/03-regression-and-generative-models/) | Linear regression, gradient descent, Ridge/Lasso, LDA/QDA, generative modeling, KL divergence, moment matching, heteroskedastic regression, Bayesian inverse problems |
| [Homework 4 — Neural Networks & Kernels](assignments/04-neural-networks-and-kernel-methods/) | NumPy MLP, gradient checking, CNNs, convolution mechanics, SVM kernels, Gram matrices, Gaussian Process Regression, Nyström approximation, active sampling |
| [Homework 5 — PCA & Clustering](assignments/05-dimensionality-reduction-and-clustering/) | Data preprocessing, standardization, PCA, explained variance, K-Means, elbow method, hierarchical clustering |
| [Course Project — Hidden Markov Anomaly Detection](course-project/) | OC-SVM, Markov chains, HMMs, Viterbi decoding, sequence-aware features, simplified HMAD, cross-domain anomaly detection |

## Course project

The team project, **“Hidden Markov Anomaly Detection: From OC-SVM to Structured Sequence Models,”** investigates when modeling latent temporal structure improves anomaly detection over a fixed-vector one-class baseline.

The work compares OC-SVM and a simplified HMAD pipeline across synthetic sequences and several application domains, including network intrusion, wind-turbine telemetry, wind-energy time series, DNA sequences, and ECG signals.

**Team authors:** Pantea Farhadi, Anahita Ardakanian, and Saba Atashfaraz.

- [Project overview and notebooks](course-project/README.md)
- [Final project report (PDF)](course-project/report/ML_project_final_report.pdf)

## Repository structure

```text
.
├── README.md
├── requirements.txt
├── requirements/
│   ├── homework-01.txt
│   ├── homework-02.txt
│   ├── homework-03.txt
│   ├── homework-04.txt
│   ├── homework-05.txt
│   └── course-project.txt
├── .gitignore
├── DATASETS.md
├── SHARING_AND_ACADEMIC_INTEGRITY.md
├── assignments/
│   ├── 01-bayesian-inference-and-probabilistic-models/
│   ├── 02-optimization-and-constrained-learning/
│   ├── 03-regression-and-generative-models/
│   ├── 04-neural-networks-and-kernel-methods/
│   └── 05-dimensionality-reduction-and-clustering/
└── course-project/
    ├── README.md
    ├── data/
    ├── notebooks/
    └── report/
```


**Topics:** Bayesian Inference · Optimization · Regression · Statistical Learning · Neural Networks · Kernel Methods · Clustering · Sequence Modeling · Anomaly Detection
