# The Shape of the Microbiome: From Geometry to Biology

Topological Data Analysis of the human gut microbiome using **PCoA**, **Persistent Homology**, **Mapper**, and microbial gradients to explore its relationship with cardiometabolic health.

## Overview

This project studies whether the human gut microbiome is better represented as discrete groups, known as enterotypes, or as a continuous biological structure.

Using microbiome data from Colombian adults, we analyzed the global geometry and topology of the microbiome and evaluated whether this structure was more strongly associated with dietary variables or cardiometabolic health.

## Main Research Questions

- Does the gut microbiome organize into separated groups or as a continuum?
- Which variables better explain this structure: diet or cardiometabolic profile?
- Which bacterial genera characterize the healthier and more altered regions of the continuum?

## Methods

The analysis includes:

- Bray-Curtis distance
- CLR transformation
- Principal Coordinates Analysis (PCoA)
- Persistent Homology
- Mapper algorithm
- Moran’s I and alignment scores
- Differential analysis between Mapper extremes
- Spearman correlations between bacterial genera
- Microbial Gradient index

## Main Findings

- The microbiome did not behave as clearly separated enterotypes, but as a continuous structure.
- `met_score` was the variable most strongly aligned with the Mapper structure.
- The lower end of the continuum was associated with healthier cardiometabolic profiles and genera such as:
  - *Akkermansia*
  - *Oscillospira*
  - *Methanobrevibacter*
- The higher end was associated with more altered cardiometabolic profiles and genera such as:
  - *Prevotella*
  - *Escherichia*
  - *Haemophilus*
- PCoA visualizations, Spearman correlations, Mapper coloring, and the Microbial Gradient were consistent with the same interpretation.

## Repository Structure

```text
.
├── microbiome_topological_analysis.ipynb
├── Topological_Data_Analysis_of_the_Human_Gut_Microbiome.pdf
└── Datos/
    ├── microbio_selected.meta
    ├── microbio_selected.otus
    └── microbio_selected.taxonomy
