Reproducibility package for the manuscript  
“Protein embeddings reveal a continuous molecular landscape of host adaptation in waterfowl parvoviruses”

This package contains all input data, analysis scripts, and configuration files needed to regenerate Figures 1–5 of the main text. The main analyses can be rerun using the included data, scripts, and Conda environment definition.

For transparency and reuse, we also provide the core analysis scripts (Python, shell, and PyMOL; see the `Scripts/` directory), which document how each panel was generated and can serve as starting points for related work.

Directory overview
------------------

- `Figure1/` – Phylogenetic analysis (VP1 multiple sequence alignment, maximum-likelihood tree, and host colour mapping).
- `Figure2/` – UMAP visualisation of ESM VP1 embeddings.
- `Figure3/` – Cluster-distance calculations and k-nearest-neighbour host prediction analysis.
- `Figure4_5/` – AlphaFold-predicted VP1 structures, loop (residues 300–420) analyses, and APBS electrostatic potential inputs.
- `Fold/` – AlphaFold Server output for VP1 models from the GPV, transition, and MDPV lineages (top 5 models, JSON metadata, MSAs, and templates).
- `Scripts/` – Core analysis scripts used to generate the figures (Python, shell, and PyMOL).
- `environment.yml` – Conda environment used for all analyses.

All files are provided in open, platform-independent formats (`.csv`, `.tsv`, `.pdb`, `.cif`, `.in`, `.yml`, `.py`, `.sh`, `.pml`, `.json`).

How to run the analyses
-----------------------

1. Create and activate the Conda environment:

   ```bash
   conda env create -f environment.yml
   conda activate GPV_repro

2. Refer to each Figure*/ folder (and the Scripts/ directory where appropriate) for the input data and example commands corresponding to the manuscript figures.
