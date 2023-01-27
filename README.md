# Characterization of B cell differentiation into regulatory plasmocytes through single cell RNA sequencing.

Repository containing the scripts written to analyze the scRNAseq data on *in vitro* activated B cells presented in the publication:

B. Manfroi & V.D. Dang, "Induced regulatory B cells stably expressing IL-10 cure CNS autoimmunity by targeting microglia", 2023

Activated B cells can regulate immunity through interleukin(IL)-10 production. The differentiation of IL-10-producing B cells and their development for cell therapy have been limited by the lack of a protocol to efficiently generate these cells. To overcome this limitation, we performed a high-throughput screen and identified small molecules enabling the induction of quasi-pure and stable IL-10-producing B cells. These B cells cured recipient mice from experimental autoimmune encephalomyelitis within a few days upon administration at the peak of disease. Their therapeutic effect involved their accumulation in the central nervous sytem of treated mice, required IL-10 receptor signaling in microglia and was independent of their interaction with CD4+ T cells. This study reports the generation of induced regulatory B cells (iBregs) for therapy against inflammatory diseases. 

## How to reproduce the figures of the publication

The raw data used for this scRNAseq analysis is stored on GEO : https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE219282.

The scripts presented here lead to the figures S10, S12B, S13A, S14, S15, and S16 of the associated publication.

More precisely :
- [0-kb_count_matrices.ipynb](0-kb_count_matrices.ipynb) > Count matrices are generated from raw data.
- [1-QC.ipynb](1-QC.ipynb) > Quality control steps performed to exclude poor quality cells and genes. Figures S10A and S10B, S13A can be produced at this step using a scanpy framework. S12B was produced using a Seurat framework.
- [4-Differential.ipynb](4-Differential.ipynb) > Differential expression analysis comparing various cell subsets, notably N6-treated *versus* DMSO-treated B cells
- 
-
-
-

## A more complete analysis of the dataset

