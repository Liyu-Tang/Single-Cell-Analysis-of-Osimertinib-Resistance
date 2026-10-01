# Single-Cell Analysis of Osimertinib Resistance

## Overview

Osimertinib is a targeted therapy used to treat EGFR-mutant lung cancer, but cancer cells can develop drug persistence and acquired resistance during treatment. Understanding the transcriptional changes associated with this adaptation may help identify genes and biological pathways involved in resistance.

In this project, I used single-cell RNA sequencing data from PC9 lung cancer cells exposed to increasing concentrations of osimertinib. The dataset includes untreated control cells, cells collected across progressive dose-escalation conditions, cells adapted to 1.2 µM osimertinib (T1.2), and cells exposed acutely to 1.2 µM osimertinib (P1.2).

I analyzed how gene expression and biological pathway activity change as cells adapt to increasing drug concentrations. Differential expression and pathway analyses were used to identify transcriptional features shared between persistent and adapted cells.

Finally, I used machine learning to distinguish untreated (C) cells from fully adapted (T1.2) cells based on gene expression. Rather than predicting clinical treatment response, the model was used to investigate whether intermediate treatment and acute persister cells increasingly resemble the transcriptional state of fully adapted cells. This provides a way to explore potential molecular features associated with the transition from drug sensitivity toward persistence and acquired resistance.

## Dataset

Dataset: GSE247684 from GEO DataSets 

## Analysis
### Quality control and preprocessing with Scanpy
  Using the dataset from GEO DataSets, AnnData Object was created and normalizing the logarithmize. 
### Highly variable gene selection
The top 2000 highly variable genes are pretty concentrated. 
### PCA and UMAP
From the PCA, orig.ident which is the types of cell samples, control, T1.2 etc are pretty even mixed, and the mitochondria percentage count are also spread evenly. 
From the UMAP, all the cell samples depending on orig.ident are cluster mostly invidually, and the percentage of mitochondria in the samples are also expressive in every cluster. 
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
