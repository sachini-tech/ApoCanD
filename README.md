# ApoCanD: Database of Human Apoptotic Proteins in the Context of Cancer

Welcome to the official repository for ApoCanD, a dedicated database of human apoptotic proteins compiled in the context of cancer. This resource is designed to support researchers working in the fields of apoptosis biology, cancer genomics, and anticancer drug discovery.

Database URL: https://webs.iiitd.edu.in/raghava/apocand/index.php

## Citation

Kumar, R., & Raghava, G. P. S. (2016).
ApoCanD: Database of human apoptotic proteins in the context of cancer.
Scientific Reports, 6, 20797. https://doi.org/10.1038/srep20797


## About the Database

ApoCanD is a dedicated database of 82 human apoptosis proteins curated specifically in the context of cancer. It addresses the critical gap left by earlier resources such as DataBase, which lacked genomic information essential for understanding the function of apoptosis proteins in cancer. ApoCanD consolidates mutation data, expression profiles, copy-number variation, gene essentiality, and structural information into a single, user-friendly platform.

The database integrates information from:

* Cancer genomics repositories (CCLE, COSMIC)
* Normal variation data (1000 Genome Project)
* Gene essentiality resource (COLT-Cancer)
* Structural databases (PDB, Pfam, Superfamily)
* Post-translational modification resource (dbPTM)


## Key Features

Curated Dataset

* 82 human apoptosis proteins
* 33,525 total mutations (cancer cell lines + tumour samples)
* 1,368 mutations filtered from CCLE across 947 cancer cell lines
* 32,157 mutations from COSMIC tumour and cell line data

Genomic Coverage

* Mutation data from CCLE and COSMIC
* Copy number variation from Affymetrix SNP 6.0 arrays
* Gene expression data from Affymetrix U133 plus arrays (RMA normalized)
* Normal variants from 1000 Genome Project for comparative benchmarking

Gene Essentiality Data

* shRNA dropout profiles from COLT-Cancer (~16,000 genes)
* Data across 72 breast, ovarian, and pancreatic cancer cell lines
* GARP score and P-value for each gene per cell line

Rich Annotations
Each entry includes:

* Cellular location, pathway, chromosomal location, and protein family
* Tertiary structure (experimental from PDB + modeled using HH-suite and Modeller)
* Structural domains (233 Pfam domains and 139 Superfamily domains)
* Sequence alignments (wild-type, CCLE mutants, COSMIC mutants, homologues)
* Sequence profiles (HMM and PSSM)
* Post-translational modifications (phosphorylation, acetylation, ubiquitylation)


## Overview

ApoCanD provides experimentally and computationally derived data along with:

* Mutation frequency and cancer vs. normal variant benchmarking
* Gene expression and copy number variation profiles
* Gene essentiality across cancer cell lines
* Modeled and experimental tertiary structures
* Structural domain annotations (Pfam and Superfamily)
* Sequence alignments and evolutionary trees
* Cancer sensitivity prediction for sequence variants
* Cross-references (UniProt, DeathBase, PDB, PubChem, ChEMBL)


### Structure Prediction

Structures were obtained or predicted using:

* PDB (experimental crystal structures — available for 61 of 82 proteins)
* HH-suite 2.0.16 (template-based homology modeling)
* Modeller 9.13 (comparative structure modeling)
* Jmol applet (online visualization with PDB download option)


### Data Retrieval Tools

* **Simple Search** — Query by keyword: protein name, cellular location, pathway, domain, or family
* **Advanced Search** — Multi-field search using AND/OR logical operators across cellular location, pathway, and family
* **BLAST** — Sequence similarity search against all 82 apoptosis protein sequences
* **Alignment** — Align query sequences against wild-type, CCLE mutants, COSMIC mutants, or 1000 Genome variants; visualized via Jalview with conservation, quality, and consensus information
* **Cancer Sensitivity** — Predict whether a sequence variant is a cancer-sensitive mutation or a normal variation, based on HMM profile similarity scores (HMMER suite)
* **Browse** — By protein, chromosomal location (Circos plot), mutation source, and genomic features (mutation frequency, expression, CNV)
* **Pathway** — Interactive apoptosis pathway diagram (intrinsic and extrinsic) linked to individual protein summary pages


### Key Findings

* TP53 is the most frequently mutated apoptosis protein in cancer (~1,158× more mutated than in normal samples)
* MYD88 is the second most mutated (~100×), a known target in cancer therapy
* Major mutation type is substitution (30,957 out of 33,525 total mutations)
* XIAP is over-expressed and SMAC/DIABLO is under-expressed across many cancer cell lines


### Limitations

* Discrepancies may exist between CCLE and COSMIC mutation datasets due to differences in computational protocols (e.g., dbSNP filtering, cell line passaging)
* Gene essentiality data currently covers only 72 breast, ovarian, and pancreatic cancer cell lines
* Quantitative structure-activity relationship (QSAR) models for drug design are planned for future integration


## Applications

* Identifying mutational hotspots and drug targets in the apoptosis pathway
* Machine learning model training for anticancer drug response prediction
* Cancer subtype-specific drug sensitivity analysis
* Biomarker discovery using apoptosis pathway genomics
* Structure-based design of targeted anticancer therapies
* Functional impact prediction of amino acid substitutions


## Contact & Authors

Prof. Gajendra P. S. Raghava
EMAIL: raghava@iiitd.ac.in
http://webs.iiitd.edu.in/raghava/

Developed at:
 IIIT Delhi


## License

This database is distributed under the
Creative Commons Attribution License (CC BY 4.0)


## Acknowledgements

We acknowledge all database and software authors whose resources were used in the construction of ApoCanD.
