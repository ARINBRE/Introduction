# AR-INBRE Research Computing Introduction

Welcome to the central hub for the **Arkansas IDeA Network of Biomedical Research Excellence (AR-INBRE)** research computing resources. This document serves as the main catalog, providing a clear overview of the Repos for educational modules available within the ARINBRE GitHub.

---

## Quick Start Navigation

Use the links below to quickly access our essential introductory guides for working with the AR-INBRE tools on HPC and cloud environments:

* **[Linux Command](linux-intro.md):** Essential shell commands for navigating, managing files, and working in a bioinformatics or HPC environment.
* **[Conda Environment Guide](conda-intro.md):** Learn how to manage software dependencies and create reproducible environments for all AR-INBRE pipelines.

---

## Repository Catalog

The following table summarizes all 7 core repositories, their primary purpose, and the key technologies they utilize. Click on any link to access the repository directly.

| Repository Name | Primary Focus | Description | Link |
| :--- | :--- | :--- | :--- |
| **Proteome-Quantification** | **Proteomics Secondary Analysis** | R, TMT10plex, Statistical Analysis | [Go to Repo](https://github.com/ARINBRE/Proteome-Quantification) |
| **Biomedical-Imaging-Analysis-using-AI-ML-Approaches** | **AI/ML Image Analysis** | Deep Learning (Neural Networks), Python, Computer Vision | [Go to Repo](https://github.com/ARINBRE/Biomedical-Imaging-Analysis-using-AI-ML-Approaches) |
| **GeneMicroarrays** | **Gene Microarray Analysis** | R, Jupyter, GEO Query, Affymetrix | [Go to Repo](https://github.com/ARINBRE/GeneMicroarrays) |
| **DEanalysis using DESeq2** | **RNA-Seq Count Analysis** | R (DESeq2), Bioconductor | [Go to Repo](https://github.com/ARINBRE/DEanalysis_DESeq2) |
| **PCA** | **Dimensionality Reduction** | R, Jupyter, Visualization | [Go to Repo](https://github.com/ARINBRE/PCA) |
| **DNAmethylation** | **Epigenetic Analysis** | R, Illumina 450k/EPIC, Bioconductor | [Go to Repo](https://github.com/ARINBRE/DNAmethylation) |
| **RNAseq** | **RNA-Seq Pipeline & Analysis** | Nextflow, R (EdgeR/Limma), Jupyter, HPC, Slurm, Bash | [Go to Repo](https://github.com/ARINBRE/RNAseq) |

---

## Detailed Module Overviews

### 1. Proteome-Quantification

* forked from NIGMS/Proteome-Quantification
* **Purpose:** Secondary analysis of Mass Spectrometry-based Proteomics data in R.
* **Scope:** This module outlines the essential steps in analyzing proteomics data, focusing on differential abundance. It assumes a simple experimental design (e.g., two conditions) using TMT10plex multiplex design with MS3 data acquisition.
* **Key Learnings:** You will gain a strong understanding of mass spectrometry and statistical terminology for data preprocessing, normalization, and differential abundance analysis using **R**.
* **Note:** This resource was forked from NIGMS/Proteome-Quantification and developed by UAMS for the NIH NIGMS Sandbox project.

### 2. Biomedical-Imaging-Analysis-using-AI-ML-Approaches

* forked from NIGMS/Biomedical-Imaging-Analysis-using-AI-ML-Approaches
* **Purpose:** Machine Learning educational module for cloud-based biomedical image analysis.
* **Motivation:** Addresses the need for advanced data analysis tools, specifically Artificial Intelligence (AI) and Deep Learning, to identify complex, hidden patterns in multidimensional data (e.g., images).
* **Technology Focus:** **Deep Learning**—the utilization of neural networks for tasks such as:
    * Cancer detection
    * Cell and tissue segmentation
    * Particle tracking
* **Module Content:** The course covers generating and training a neural network, manipulating datasets, applying the trained network to new data, and quantifying its performance.
* **Accessibility:** This module is available for both **AWS** and **Google Cloud**.
* **Cost Estimate:** The entire module is designed to cost approximately **$1.00** to run, assuming all resources are correctly terminated upon completion.
* **Video:** [Watch this Introduction Video to learn more about the module.](https://youtu.be/-5GHSZABDLk)

### 3. Gene Affymetrix Processing and Analysis

* **Purpose:** This educational module demonstrates the steps needed to download raw microarray files from the Gene Expression Omnibus (GEO) repository, ensure quality control by filtering out biased samples, process data (background correction, between samples normalization, and probe summarization), perform differential expression (DE) analysis, and generate visualizations.
* **Motivation:** Both R code and the same R code executed within a Jupyter Notebook supported by a conda environment are available. The modeule uses the GSE15641* series downloaded from GEO. The dataset has clear cell renal cell carcinoma (ccRCC) samples and normal controls, among other groups of samples.

### 4. DEanalysis using DESeq2

* **Purpose:** This educational module demonstrates the steps needed to perform differential expression (DE) analysis using Bioconductor package DESeq2. The analysis applies to integer count matrices generated from RNA-seq data.
* **Motivation:** The module was conducted using R version 4.4.2 in a Jupyter Notebook with R kernel. The associated Anaconda environment for the Jupyter Notebook is provided in file 'environment_R_4.4.2.yaml'. If you run the R code, ensure the proper version is installed on your machine along with the required libraries. To install Bioconductor packages, packge BiocManager is required. 

### 5. Principal Componenet Analysis

* **Purpose:** Principal Component Analysis (PCA) is a dimensionality reduction method, often used to create visualizations of high-dimensional data such as gene expression or DNA methylation datasets with thousands of features (e.g. genes).
* **Motivation:** The module was conducted using R version 4.4.2 in a Jupyter Notebook with an R kernel. The associated Anaconda environment for the Jupyter Notebook is provided in file 'environment_R_4.4.2.yaml'. The primary objective of this module is to demonstrate the use of PCA to visualize high-dimensional gene expression data by creating a two-dimensional scatter plot that shows sample distribution in a 2D space representing the first two principal components. 

### 6. DNAmethylation_ArrayAnalysis

* **Purpose:** This educational module demonstrates the steps needed to process raw files generated by Illumina's Infinium beadchip array 450k (or the 850k EPIC chip) and perform differential methylation analysis at the probe level. 
* **Motivation:** The workflow uses R and Bioconductor packages and includes downloading raw data files from the Gene Expression Omnibus (GEO) repository. Both R code and the same R code within a Jupyter Notebook environment are available.

### 7. RNASeq

* **Purpose:** A comprehensive collection of resources for performing RNA-Sequencing analysis, ranging from upstream HPC pipeline execution to downstream differential expression analysis in R.
* **Workflow Scope:** This repository bridges the gap between raw data processing on a supercomputer and statistical analysis on a local machine or server.
* **Key Files & Components:**
    * **`RNAseq_Bash_Notes.docx`:** The essential guidebook. It contains detailed notes and commands for executing the upstream **Nextflow pipelines** on a High-Performance Computing (HPC) cluster. It guides users through the initial heavy processing (alignment, quantification) before moving to analysis.
    * **`RNASeq_EdgeR_100124.ipynb`:** A Jupyter Notebook focused on differential gene expression analysis using the **EdgeR** statistical package. This is a primary workflow for identifying significantly changed genes.
    * **`RNASeq_EdgeR_limmaVoom_Example.ipynb`:** An alternative analysis workflow demonstrating the **limma-voom** method. This allows users to compare results or choose the statistical approach best suited for their data distribution.
    * **`RNASeq_Fall22v2.ipynb`:** A versioned notebook (likely from the Fall 2022 workshop cycle) serving as a standard reference or educational walkthrough for the analysis pipeline.
* **Key Technologies:** Nextflow, Jupyter Notebooks, R, and Bash (HPC interaction) for parllelization.

---

Let us learn bit about Linux [Next Page &rarr;](linux-intro.md)
