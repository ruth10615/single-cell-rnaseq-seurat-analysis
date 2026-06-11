# Expression of pain-related genes in transcriptomics databases
From March to July 2024, I completed an internship at the CNRS laboratory GPCRs, Pain and Inflammation under the supervision of Dr. Frédéric Simonin in France.
The research team investigates the role of various G protein-coupled receptors (GPCRs) in the development of pain and inflammation, as well as the mechanisms regulating GPCR signaling from the cell surface to intracellular compartments.
The laboratory focuses on two major receptor/ligand families, RF-amide peptides and CXCL12/CXCR4 signaling pathways. Using both pharmacological approaches (agonists and antagonists) and genetic models (knockout mouse lines), the team aims to better understand the specific roles of these receptors in the modulation of nociception and opioid-induced analgesia.

## Objective
In this project, the goal is to investigate the expression of these genes in an available transcriptomics database to better understand the dynamics of cellular heterogeneity and gene expression in pain conditions.
The specific objectives are: (1) identify the cell types or clusters, (2) to obtain
expression data from single-cell/nucleus RNA-seq, (3) to determine the percentage of each cell type that expresses the genes of interest, and (4) to gather data on the list of genes expressed in each cell type/cluster.

## Tools
R, Seurat, Bioconductor, dplyr, ggplot2, Matrix, gdata

## Dataset
RNA-seq data analysis of pain-related research
a) Russ et al. 2021
b) Matson et al. 2022
c) Fan et al. 2023
e) Yadav et al. 2023

## Methodology
- Loading of data to Seurat object
- Addition of metadata
- Normolization and scaling
- Dimentionality reduction
- Clusterign
- UMAP plot generation
- Marker identification
- Differential expression calculation

## Key Results
	•	With this project on single cell RNA-seq data from Fan et al. study, I could show that the morphine receptor OPRM1 is expressed mainly in neurons, and in both excitatory and inhibitory neurons.
	•	The RF-amide receptors are expressed in fewer cells than OPRM1, and each receptor has a distinct cell expression profile
	•	CXCR4 gene is expressed in the lumbar site, with an increase in expression in the Microglia 2 cluster on 30-days after injury. In Matson et al. study, it was discovered that the gene expression profile of "activated microglia A" strongly resembled a signature recently observed in postnatal microglia that can promote repair from spinal cord injury. We can speculate that CXCR4 in Microglia-2 is involved in this process on 30-days following injury in these microglia
	•	Critical analysis. at each stage post injury, data from only one sample were available and statistical analysis could not be performed

## What I learned
	•	Single cell RNA-sequencing is an effective tool for studying the heterogeneity of cells or genes expression in physiological and pathological conditions. 
	•	The rapid development of AI not only makes it easier to use these tools but also makes data analysis more comprehensive. 
	•	This project primarily studies data on monkeys. In the future, it may be possible to analyze data on mice, humans, or other species, and in different pain conditions.
