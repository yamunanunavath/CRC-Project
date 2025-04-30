# Early Detection of Colorectal Cancer Using Microbiome-Based Machine Learning Biomarker

## Overview

This project aims to demonstrate the potential of using the human gut microbiome as a diagnostic tool for the early detection of colorectal cancer (CRC). By analyzing metagenomic stool sequencing data from both CRC patients and healthy individuals, this project explores the use of machine learning techniques to identify microbial biomarkers that may help stratify patients and detect CRC at an early stage.

## Project Objectives

- **Data Collection**: The project uses metagenomic stool sequencing data (SRR31649983) from CRC and healthy patients, which has been processed and analyzed using Kraken2 for taxonomic profiling.
- **Data Processing**: Species-level abundance profiles were harmonized, and taxonomic distributions at both the species and phylum levels were visualized.
- **Modeling**: A **Random Forest classifier** was implemented to identify potential microbial biomarkers for CRC detection. Additionally, machine learning models such as **Support Vector Machines (SVM)** were trained on the data to assess predictive performance.
- **Key Findings**: Key predictive species such as **Faecalibacterium prausnitzii** and **Enterocloster bolteae** were identified as top contributors to CRC classification.

## Data

The data used in this project consists of metagenomic stool sequencing data obtained from CRC patients and healthy individuals. The data is available from the NCBI database and has been processed using Kraken2 to profile species-level abundance.

## Methodology

1. **Taxonomic Profiling**: Kraken2 was used for species-level taxonomic classification of the stool samples.
2. **Data Preprocessing**: The species-level abundance data was processed and harmonized for downstream analysis.
3. **PCA Analysis**: Principal Component Analysis (PCA) was used to reduce dimensionality and visualize the data.
4. **Clustering**: K-means clustering was performed to identify distinct groups within the data.
5. **Modeling**:
   - **Random Forest Classifier**: This was used to identify important microbial features for CRC classification.
   - **SVM Classifier**: A Support Vector Machine was implemented to further evaluate the model's performance.
6. **Statistical Analysis**: One-way ANOVA, Kruskal-Wallis tests, and Tukey HSD post-hoc tests were applied to validate differences between clusters.

## Key Results

- **Important Biomarkers**: Faecalibacterium prausnitzii and Enterocloster bolteae were identified as potential biomarkers for CRC detection.
- **Model Accuracy**: Both Random Forest and SVM models achieved high classification accuracy, emphasizing the potential of microbiome-based biomarkers in detecting CRC at an early stage.
- **Clustering**: K-means clustering successfully grouped CRC patients and healthy individuals based on microbial features.

## Technologies Used

- **Kraken2**: For taxonomic profiling.
- **Random Forest**: For feature selection and classification.
- **Support Vector Machines (SVM)**: For classification and model comparison.
- **R**: The main programming language used for data analysis and visualization.
- **ggplot2**: For data visualization.
- **caret**: For machine learning model training and tuning.

## Installation

To run the analysis locally, follow these steps:

1. Clone this repository:
   ```bash
   git clone https://github.com/yamunanunavath/CRC-Project.git
   ```

2. Install the necessary R packages:
   ```R
   install.packages(c("ggplot2", "dplyr", "caret", "randomForest", "cluster", "factoextra"))
   ```

3. Load the data and run the analysis scripts in the `Rmd` files.

## Future Work

- **Multi-Omics Integration**: Future work could involve integrating other omics data (such as genomics and transcriptomics) to improve the predictive power of the classifier.
- **Clinical Validation**: The next step is to validate these microbial biomarkers in a clinical setting to assess their real-world applicability.
- **Broader Datasets**: Extending the analysis to include more diverse datasets from different populations will be critical to ensure generalizability.

## Conclusion

This project demonstrates the feasibility of using microbiome-based classifiers for the early detection of colorectal cancer. By identifying key microbial species that are associated with CRC, this project lays the groundwork for developing non-invasive diagnostic tools that can improve early detection and patient outcomes.


## Acknowledgements

- Thanks to the contributors and researchers who provided the metagenomic data for this project.
- Special thanks to the tools and packages such as Kraken2, R, ggplot2, and caret that made the analysis possible.

