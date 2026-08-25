# MAP
This repository contains the source code and example data for the computational analyses described in:

> Colocalomics: digitalization of intercellular messengers and identification of barrier-crossing subtypes for precision diagnosis

The code implements the computational framework for single EV digitalization, machine learning-based classification, parameter optimization, and diagnostic performance evaluation.

## Overviewhttps://github.com/yifeijiangHIM/MAP/blob/main/README.md

The analysis pipeline consists of the following major steps:

1. EV digitization and establishment of a multi-dimensional grid
2. Classification of EV subpopulations, and assign them to the grid based on marker expression profiles
3. Generating a volcano plot and identify EV subgroups with disease relevance
4. For EV subgroups with AUCs above threshold, optimize grid boundaries (marker expression ranges) to further improve the diagnostic performances.
6. Generation of computational results, including the expression profile, P values and fold of change of the EV subgroups.

A simplified workflow is:

1.Input EV data
2.EV digitalization
3.EV subpopulation identification
4.Volcano plot analysis   
5.Marker-range optimization based on ROC/AUC 
6.Results and figures


## Repository Structure
main/
│
├── README.md
├── LICENSE
├── CITATION.cff

├── code/
│   ├── MAP_ESCC.m
│   └── MAP_AD.m

├── demo/
│   ├── ESCC data.zip
│   └── AD data.zip

└── results/
│   └── example_results/
│   ├── ESCC EV list.doc
│   └── ESCC volcano plot.fig
│   ├── AD EV list.doc
│   └── AD volcano plot.fig
