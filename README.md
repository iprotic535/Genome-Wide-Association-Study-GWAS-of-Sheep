# Genome-Wide-Association-Study-GWAS-of-Sheep
# Differential Gene Expression Analysis

## Overview
This repository encompasses a detailed RNA-seq analysis project aimed at uncovering differentially expressed genes (DEGs) due to specific treatment conditions. Leveraging robust statistical tools in R, including DESeq2, and methodologies from bioinformatics, this project provides insights into the molecular dynamics triggered by experimental treatments.

## Project Objectives
- To discern the variations in gene expression elicited by distinct treatments.
- To pinpoint genes that exhibit significant upregulation or downregulation post-treatment.
- To elucidate the biological implications of these expression changes by conducting pathway analyses.

## Analytical Methods Employed
### Data Normalization
Utilizing size factors, we normalized the sequencing data to mitigate discrepancies in library sizes across samples. This crucial step ensures that the variations in gene expression observed are attributable to biological differences rather than technical biases.

### Estimating Dispersion
We employed DESeq2's robust model to estimate dispersion, which quantifies the variability of gene expression across samples. This measure is vital for assessing the reliability of observed expression changes.

### Principal Component Analysis (PCA)
PCA was executed to scrutinize the variability among samples and to identify predominant sources of variation, offering a visual confirmation of the impact of treatments on gene expression.

### Differential Expression Analysis
Using the powerful DESeq2 package, we conducted a thorough differential expression analysis. We employed adjusted p-values to determine the statistical significance of observed changes in gene expression between different treatment groups.

## Key Findings
- **PCA Outcomes**: The PCA plot revealed a distinct segregation of samples based on treatment groups, underscoring the profound impact of the treatments on gene expression profiles.
- **Differentially Expressed Genes**: We identified 2,187 genes as differentially expressed with an adjusted p-value threshold of 0.05, and 2,751 with a threshold of 0.10.
- **Visualizations**: The MA and Volcano plots provided a graphical representation of the DEGs, emphasizing genes with significant fold changes and robust statistical support.
- **Heatmap Visualization**: We also crafted a heatmap for genes with a -log10(padj) greater than 20, which showcased clusters of genes with similar expression patterns, highlighting their potential shared biological functions.

## Detailed Figures
![Dispersion Plot](https://github.com/iprotic535/Genome-Wide-Association-Study-GWAS-of-Sheep/blob/main/images/dispersions.png)
*Figure 1: Dispersion plot illustrating the variability in gene expression among samples.*

![PCA Plot](https://github.com/iprotic535/Genome-Wide-Association-Study-GWAS-of-Sheep/blob/main/images/pca.png)
*Figure 2: PCA plot demonstrating the separation of samples based on treatment groups.*

![MA Plot](https://github.com/iprotic535/Genome-Wide-Association-Study-GWAS-of-Sheep/blob/main/images/MA.png)
*Figure 3: MA plot displaying log fold changes against the average of normalized counts.*

![Volcano Plot](https://github.com/iprotic535/Genome-Wide-Association-Study-GWAS-of-Sheep/blob/main/images/Volcano.png)
*Figure 4: Volcano plot showcasing log2 fold changes plotted against -log10 adjusted p-values.*

![Heatmap](https://github.com/iprotic535/Genome-Wide-Association-Study-GWAS-of-Sheep/blob/main/images/Heatmap.png)
*Figure 5: Heatmap of significant genes, depicting clustering based on expression patterns and highlighting potential biological processes influenced by treatments.*

## Repository Structure

## Execution Instructions
Detailed instructions on how to perform the analysis are available in the `/scripts` directory, which include a list of necessary libraries and commands for executing the scripts.

## Contact Information
For further details or inquiries about collaborations, please reach out to [email@domain.com](mailto:email@domain.com).

## Acknowledgements
We express our gratitude to all the team members and collaborators who have contributed to the success of this project, providing valuable insights and support.
