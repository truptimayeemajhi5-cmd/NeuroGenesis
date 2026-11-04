# NeuroGenesis: Comparative Single-Cell Manifold Embedding

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.placeholder.svg)](https://zenodo.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/)
[![Scanpy](https://img.shields.io/badge/Scanpy-1.11.5-brightgreen.svg)](https://scanpy.readthedocs.io/)

A reproducible single-cell transcriptomics pipeline benchmarking the homeostatic lineage restriction of canonical neurodegenerative susceptibility loci (*TYROBP*, *APOE*, *HLA-DRA*, *FTL*) across circulating peripheral mononuclear cells and hippocampal neurogenic niches.

---

## Deliverables & Repository Structure

* **`Comparative_SingleCell_Manifold_Benchmarking.pdf`**: Complete research manuscript detailing baseline lineage benchmarking, methodology, study limitations, and formal literature citations.
* **`NeuroGenesis.ipynb`**: End-to-end executable pipeline detailing quality control, dispersion-based feature selection, neighborhood graph construction, Leiden community detection, and log-normalized differential expression analysis.
* **`environment.yml`**: Conda environment specification detailing all package dependencies and versions for reproducible execution.

---

## Scientific Scope & Core Findings

1. **Innate Immune Signaling Hubs (*TYROBP*):** Selective baseline co-enrichment within peripheral $CD14^+$ monocytes and resident microglia, establishing conserved myeloid receptor signaling across physiological barriers.
2. **Lipid Metabolism Compartmentalization (*APOE* / *Apoe*):** Strict localization to hippocampal astrocytes and radial glia-like progenitors, serving as a non-pathological baseline control.
3. **Continuous Neurogenic Trajectories:** Resolution of neurogenic transit-amplifying lineages (*nIPC* to *Dcx*+ neuroblasts) alongside mature granule neurons via Leiden community graph partitioning.

---

## Datasets & Accession

* **Peripheral Mononuclear Cells (PBMC):** Healthy donor reference dataset (2,638 cells) sourced via 10x Genomics (`sc.datasets.pbmc3k()`).
* **Hippocampal Dentate Gyrus:** Postnatal murine neurogenic niche dataset (2,930 cells) sourced via scVelo (`scv.datasets.dentategyrus()`).

---

## Installation & Environment Setup

Clone this repository and create the conda environment:

```bash
git clone [https://github.com/truptimayeemajhi5-cmd/NeuroGenesis.git](https://github.com/truptimayeemajhi5-cmd/NeuroGenesis.git)
cd NeuroGenesis
conda env create -f environment.yml
conda activate neuro_drylab
jupyter lab NeuroGenesis.ipynb
@article{majhi2026neurogenesis,
  title={Comparative Single-Cell Manifold Embedding Benchmarks Baseline Lineage Restriction of Neurodegenerative Risk Adapters Across Peripheral and Hippocampal Atlases},
  author={Majhi, Truptimayee},
  year={2026},
  url={[https://github.com/truptimayeemajhi5-cmd/NeuroGenesis](https://github.com/truptimayeemajhi5-cmd/NeuroGenesis)}
}

