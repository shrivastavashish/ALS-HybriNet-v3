# ALS-HybriNet v3

Research implementation of **A Hybrid Deep Learning Framework for AI Driven Molecular Diagnostics in Rare Diseases Detection**, using amyotrophic lateral sclerosis (ALS) and the public GSE168714 cohort as the case study.

## Implemented framework

- 1-D CNN for family-ordered baseline miRNA patterns
- Masked GRU for genuine longitudinal miRNA sequences
- Availability-aware attention fusion
- Patient-level splitting and fold-specific preprocessing
- Five-fold cross-validation repeated three times
- Frozen held-out evaluation, six conventional baselines and architecture ablation
- Gradient SHAP, patient-level attribution and attention analysis

## Study data

- 356 baseline participants: 253 ALS and 103 controls
- 1,838 shared miRNAs
- 22 ALS patients with longitudinal profiles of up to four visits
- 284 development participants and 72 held-out test participants
- 512 miRNAs selected independently inside each training fold

## Headline results

- Repeated CV ROC-AUC: **0.8624 ± 0.0133**
- Repeated CV PR-AUC: **0.9481**
- Held-out ROC-AUC: **0.9057** (95% CI 0.830–0.965)
- Held-out PR-AUC: **0.9660**
- Held-out F1-score: **0.8478**
- Held-out MCC: **0.6145**

## Repository contents

- `ALS_MultiOmics_CNN_RNN_Attention.ipynb` — executed research notebook
- `index.html` — ALS-HybriNet 360 research application

## Research application

[Open ALS-HybriNet 360](https://als-hybrinet-360.mkushawaha.chatgpt.site)

This repository presents research evidence and model-analysis outputs. Clinical use would require independent external cohorts, prospective validation, governance and regulatory review.
