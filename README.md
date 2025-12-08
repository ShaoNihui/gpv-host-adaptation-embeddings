Reproducibility Package
for the manuscript:
"Protein embeddings reveal a continuous molecular landscape of host adaptation in waterfowl parvoviruses"

This package contains all input data, analysis scripts, and configuration files required to reproduce Figures 1–5 of the main text.
No additional custom code is required; all analyses can be reproduced using the included data, scripts, and environment definition.  
For transparency and reuse, we also provide the main analysis scripts (Python, shell, and PyMOL scripts; see the Scripts/ directory), which document exactly how each panel was generated and can be adapted as starting points for related work.

Directory overview:
-------------------
Figure 1  - Phylogenetic analysis (VP1 maximum-likelihood tree and host color mapping)
Figure 2  - UMAP visualization of ESM protein embeddings
Figure 3  - Cluster distance and host prediction analysis
Figure 4–5 - AlphaFold-predicted VP1 structures, loop analyses, and APBS electrostatic potential inputs
Scripts   - Core analysis scripts used to generate the figures (Python, shell, PyMOL)
environment.yml - Complete Conda environment used for all analyses

All files are organized in open, platform-independent formats (.csv, .tsv, .pdb, .cif, .in, .yml, .py, .sh, .pml).

To reproduce analyses:
1. Create the Conda environment:
   conda env create -f environment.yml
   conda activate GPV_repro

2. Refer to each Figure folder (and the Scripts/ directory where appropriate) for input data and commands corresponding to the manuscript figures.
