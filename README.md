# Single-Cell Analysis of Osimertinib Resistance

## Overview

Osimertinib is a third-generation EGFR inhibitor used to treat
EGFR-mutant non-small cell lung cancer. However, drug persistence
and acquired resistance remain major challenges.

This project uses single-cell RNA sequencing to investigate
transcriptional changes during progressive osimertinib exposure
in PC9 lung cancer cells.

## Dataset

Dataset: GSE247684

The dataset contains 4,208 cells across untreated, dose-escalation,
adapted, and acute drug-treatment conditions.

## Analysis

- Quality control and preprocessing with Scanpy
- Highly variable gene selection
- PCA and UMAP
- Leiden clustering
- Pathway scoring
- Differential expression
- Pathway enrichment
- Adaptation score
- Machine-learning analysis

## Results

Results will be summarized here.

## Tools

Python, Scanpy, AnnData, pandas, NumPy, scikit-learn, gseapy
