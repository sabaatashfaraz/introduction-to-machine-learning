# Course Project — Hidden Markov Anomaly Detection

**Title:** *Hidden Markov Anomaly Detection: From OC-SVM to Structured Sequence Models*

**Course:** Introduction to Machine Learning, Sharif University of Technology  
**Instructor:** Prof. Sajjad Amini  
**Term:** Spring 2026  
**Team:** Pantea Farhadi, Anahita Ardakanian, and Saba Atashfaraz

## Research question

When does a sequence-aware anomaly detector improve over a fixed-vector anomaly detector such as a One-Class Support Vector Machine (OC-SVM)?

The project studies the difference between point-wise anomalies and anomalies that are expressed through temporal order, transitions, or latent sequence structure.

## Methodology

The project develops a progression from a classical one-class baseline to a simplified Hidden Markov Anomaly Detection (HMAD) pipeline:

1. **OC-SVM baseline:** represent each sequence as a fixed-length vector (for example, global summary statistics, flattened observations, or window-based summaries), standardize features, and learn a one-class decision boundary.
2. **Markov chains and HMMs:** model latent state transitions and state-dependent observation emissions.
3. **Viterbi decoding:** infer a likely hidden-state path for each observed sequence.
4. **Joint sequence features:** combine hidden-state transition counts with state-dependent emission summaries.
5. **Simplified HMAD training:** alternate between hidden-state inference, HMM parameter updates, and OC-SVM fitting on the inferred joint features.
6. **Evaluation:** compare OC-SVM and HMAD using ROC-AUC and other classification metrics across different anomaly contamination settings.

This is a course-level simplified HMAD implementation; it should not be confused with a claim to reproduce every detail of the original HMAD research algorithm.

## Experimental domains

The final report and notebooks cover:
- Synthetic Gaussian sequences.
- CIC-IDS2017 network intrusion data.
- Vestas V52 wind-turbine SCADA data.
- Continual Wind Energy time-series data.
- DNA-like sequence data.
- MIT-BIH Arrhythmia ECG data.

The project includes dataset-specific notebooks and a cross-dataset comparison notebook. Raw datasets are not bundled; see `data/README.md`.

## Notebooks

| Notebook | Experiment |
|---|---|
| `01-synthetic-sequence-baseline.ipynb` | Initial synthetic sequence experiments |
| `02-synthetic-harder-configuration.ipynb` | Harder synthetic configuration |
| `03-synthetic-alternative-configuration.ipynb` | Alternative synthetic configuration |
| `04-cicids2017-network-intrusion.ipynb` | Network intrusion sequences |
| `05-vestas-v52-wind-turbine.ipynb` | Wind turbine SCADA sequences |
| `06-continual-wind-energy.ipynb` | Continual wind energy data |
| `07-dna-sequence-anomaly-detection.ipynb` | DNA sequence experiments |
| `08-mit-bih-ecg-anomaly-detection.ipynb` | MIT-BIH ECG experiments |
| `09-cross-dataset-comparison.ipynb` | Cross-domain comparison |

## Report

The final team report is available at [`report/ML_project_final_report.pdf`](report/ML_project_final_report.pdf).

The report discusses where sequence-aware modeling helped and where a static OC-SVM baseline remained competitive. In particular, it highlights that model performance depends on the anomaly structure: temporal dynamics can matter for network and industrial sequences, while localized morphological deviations may favor static feature-based detection.

## Reproducibility and limitations

- The notebooks were copied from the supplied project archive and personal student IDs were removed.
- Dataset files are not bundled. Their expected filenames and folder layout are documented in `data/README.md`.
- The notebooks have not been re-executed during repository packaging.
- Reported numerical results are those recorded in the submitted team report; they have not been independently reproduced during packaging.
- Some experiments depend on external datasets and the WFDB package for MIT-BIH records.
