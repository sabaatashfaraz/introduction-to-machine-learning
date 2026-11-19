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

## Getting started

### 1. Clone the repository

```bash
git clone https://github.com/<YOUR_GITHUB_USERNAME>/introduction-to-machine-learning.git
cd introduction-to-machine-learning
```

### 2. Create a Python environment

Python 3.10 or 3.11 is a reasonable starting point. Some assignments use different frameworks, so installing dependencies per assignment is recommended.

**Windows**
```powershell
python -m venv .venv
.venv\Scripts\activate
```

**macOS / Linux**
```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 3. Install the dependencies for the notebook you want to run

For example, Homework 1:

```bash
python -m pip install --upgrade pip
pip install -r requirements/homework-01.txt
jupyter lab
```

Use the matching requirements file for the other assignments. The top-level `requirements.txt` combines all dependencies, including PyTorch and WFDB, and may be unnecessarily large if you only want to run one notebook.

### 4. Run the notebook

Open the relevant `.ipynb` file in JupyterLab or GitHub's notebook viewer. Read the README in that assignment's folder first; some notebooks require local datasets that are not bundled.

## Dependencies

The coursework uses a combination of:
- Python, NumPy, Pandas, SciPy
- Matplotlib and Seaborn
- scikit-learn
- PyTorch and torchvision
- NetworkX
- WFDB for the MIT-BIH ECG experiment

See the `requirements/` directory for assignment-specific dependencies.

## Data and reproducibility

Input datasets are not included by default. Some files were absent from the uploaded materials; others are course-provided, derived from external benchmarks, or subject to third-party terms. Each assignment and the course project include a data README documenting expected filenames and paths.

The notebooks are preserved as submitted coursework, with student IDs and personal contact details removed from public-facing copies. They have not been re-executed during packaging, so paths and dependency versions may need adjustment in a fresh environment.

## Academic integrity, licensing, and attribution

This is a personal coursework portfolio, not an official course repository. No open-source license is included because the coursework prompts, starter materials, and datasets may have separate rights and redistribution conditions. Review the course policy and dataset licenses before making the repository public. See [SHARING_AND_ACADEMIC_INTEGRITY.md](SHARING_AND_ACADEMIC_INTEGRITY.md).

The final course project is team work and is attributed to all three authors named in the report.

---

**Topics:** Bayesian Inference · Optimization · Regression · Statistical Learning · Neural Networks · Kernel Methods · Clustering · Sequence Modeling · Anomaly Detection
