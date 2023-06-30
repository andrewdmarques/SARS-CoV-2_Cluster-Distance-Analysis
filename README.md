# Cluster Distance Analysis

This code performs cluster distance analysis using SNP differences between genomes. It reads in mutation data, genome metadata, and outbreak information to calculate and visualize the distances between different clusters.

## Prerequisites

- R programming language
- `readxl` and `plotly` libraries

## Getting Started

1. Install the required libraries by running the following commands in your R environment:
   ```R
   install.packages("readxl")
   install.packages("plotly")

## Usage

1. **Data Files:** Download the following data files and place them in the same directory as the code file:
   - Mutation data file: "2023-04-12_mutations.xlsx"
   - Genome metadata file: "2023-04-12_genomeMetaData.xlsx"
   - Outbreak information file: "2021-10-28_defining-outbreaks-by-vsp.csv"

2. **Environment Setup:** Open the code file in an R environment or RStudio.

3. **Run the Code:** Execute the code to perform cluster distance analysis and generate heatmaps of SNP differences.

## Code Explanation

The code consists of the following main sections:

### Define Functions

This section defines two functions:

- `distance_of_snp`: Calculates the number of SNP differences between two clusters.
- `make_distance_matrix`: Creates a distance matrix for the number of SNP differences between clusters.

### Make Heatmap Function

This section defines the `make_heatmap` function, which generates a heatmap visualization of the distance matrix using the plotly library.

### Perform Cluster Distance Analysis

This section performs cluster distance analysis for different outbreaks and generates heatmaps:

- The code reads in the data files using the `read_excel` and `read.csv` functions.
- The `make_distance_matrix` function is called for each outbreak, generating a distance matrix of SNP differences.
- The `make_heatmap` function is called to visualize each distance matrix as a heatmap.

## Results

The code generates heatmaps showing the SNP differences between different clusters for each outbreak. The heatmaps provide insights into the genetic distance between clusters and help identify relationships and similarities.
