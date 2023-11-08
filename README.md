# Differential Gene Expression Analysis in Candida tropicalis

This repository contains data and analysis scripts for the differential gene expression analysis of Candida tropicalis under two conditions: control/untreated and ISO-treated.

## 1 Differential Gene Expression Analysis

The analysis of differentially expressed genes (DEGs) was performed using read counts obtained from RNA-sequencing data. 
We employed the EdgeR package within the R environment for this purpose.

### Dataset
The dataset includes two stages of Candida tropicalis:
- Stage A: Control/untreated samples
- Stage B: ISO-treated samples

### Criteria for significance
- Log2-fold change (Log2FC) > 1
- False discovery rate (FDR) < 0.05

### Categorization of DEGs
- UP: DEGs with Log2FC > 1 and significant p-values
- DN: DEGs with Log2FC < -1
- NC: Genes with p-values > 0.05 (no significant change)

## 2 Functional Enrichment Analysis for DEGs

We conducted a functional enrichment analysis on the set of 186 DEGs using Gene Set Enrichment Analysis (GSEA) based on Gene Ontology (GO) terms.

### Methodology
- Filtered out GO terms with p-values > 0.05
- Adjusted p-values using the Benjamini and Hochberg method

### Gene Sets
- UP: Upregulated genes
- DN: Downregulated genes

### Tools Used
- ShinyGO v0.77 based on the Candida tropicalis genome from STRING-db

### Accessing Data
For more information on functional enrichment and detailed results, visit the ShinyGO website for Candida tropicalis: [ShinyGO Candida tropicalis](http://bioinformatics.sdstate.edu/go) (accessed on 10 May 2023).

## Data and Analysis Scripts

The raw data and analysis scripts used for this study are available in this repository. Navigate to the respective directories for access to the files.

## Citation
If you use the data or analysis protocols from this repository, please cite the original source.

## Contact
For any further queries or requests for collaboration, please submit n issue in this repository or contact the repository maintainers directly.
