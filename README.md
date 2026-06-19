# The Shape of the Microbiome: From Geometry to Biology

Topological Data Analysis of the human gut microbiome using **PCoA**, **Persistent Homology**, **Mapper**, and microbial gradients to explore its relationship with cardiometabolic health.

## Overview

This project investigates whether the human gut microbiome is better represented as discrete groups, known as enterotypes, or as a continuous biological structure.

Using microbiome data from Colombian adults, we analyzed the global geometry and topology of the microbiome and evaluated whether this structure was more strongly associated with dietary variables or cardiometabolic health indicators.

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
- Moran's I
- Alignment analysis
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
  - *Christensenella*
  - *Propionispora*
- The higher end was associated with more altered cardiometabolic profiles and genera such as:
  - *Prevotella*
  - *Escherichia*
  - *Haemophilus*
  - *Enterobacter*
- PCoA visualizations, Spearman correlations, Mapper coloring, and the Microbial Gradient consistently supported the same biological interpretation.

## Repository Structure

```text
.
├── microbiome_topological_analysis.ipynb
├── Topological_Data_Analysis_of_the_Human_Gut_Microbiome.pdf
└── Datos/
    ├── microbio_selected.meta
    ├── microbio_selected.otus
    └── microbio_selected.taxonomy
```

## Data

The project uses three primary files:

- `microbio_selected.meta` → clinical, demographic, and dietary metadata.
- `microbio_selected.otus` → microbiome abundance table.
- `microbio_selected.taxonomy` → taxonomic classification of OTUs.

## Tools and Libraries

Main Python libraries used:

- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `scipy`
- `scikit-learn`
- `networkx`
- `kmapper`

## Authors

- Felipe de Jesús Damián Rodríguez
- Gabriela Marissa Mosquera Orellana
- Kira Darián Gómez Pantoja

**Tecnológico de Monterrey**

## Faculty Advisor

Juan Felipe Carmona González

## Course

Geometry and Topology for Data Science

## Date

June 2026

## Disclaimer

This is an academic research project. The results are exploratory and show associations rather than causal relationships.
