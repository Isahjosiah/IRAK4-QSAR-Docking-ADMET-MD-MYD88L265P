# IRAK4-QSAR-Docking-ADMET-MD-MYD88L265P
Integrated QSAR, Docking, Pharmacokinetics, and Molecular Dynamics Approach for Designing IRAK4 Inhibitors Against MYD88^L265P-Driven Diffuse Large B-Cell Lymphoma

This repository contains all data and scripts necessary to reproduce the QSAR descriptor processing and molecular docking workflows for IRAK4 inhibitors in the context of the MYD88^L265P mutation, as described in the manuscript.

## Data

All files necessary to reproduce the QSAR workflow and descriptor calculations are included:

- `training_set_descriptors.csv` : Preprocessed and normalized descriptors for the training set (80% of molecules).  
- `test_set_descriptors.csv` : Preprocessed and normalized descriptors for the test set (20% of molecules).  
- `All_Padel_Descriptor_Output.csv` : Raw descriptor values calculated with PaDEL-Descriptor.  
- `Data_Pretreatment_Output.csv` : Details of preprocessing, including descriptor removal due to constant values, high correlation, or high variance inflation factor (VIF).  
- `Normalization_Output.csv` : Normalized descriptor values used in QSAR modeling.  
- `raw_sdfs.zip` : Original 33 SDF files for all molecules, allowing full reproduction of descriptor calculations and downstream analyses.  
- `Supplementary_Table_1.docx` : Detailed docking results for compounds with lower binding scores than the benchmark inhibitor ND-2158, including binding affinities, hydrogen-bond interactions, and hydrophobic contacts.

## Scripts

- `docking_pipeline.ipynb` : Complete Python notebook for molecular docking workflow.

## Reproducibility

All QSAR preprocessing, normalization, and train-test splitting were performed according to the steps documented above. With the included raw SDF files, processed CSVs, and Supplementary Table 1, all descriptor calculations and docking workflows can be independently reproduced.
