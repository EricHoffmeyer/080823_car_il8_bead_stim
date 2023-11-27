# B7H3 CAR T vs B7H3 CAR T + CXCR2 bulk RNAseq analysis

This repository contains the code and some results associated with the B7H3 CAR T + CXCR2 bulk RNAseq experiment.

Breifly, two types of CAR T cells were created:
  B7H3 CAR T cells
  B7H3 CAR T cells + CXCR2 ("BC2") - same CAR as the other, but an extra protein included in the plasmid

These two CAR T cells were submitted to three conditions:
  No stimulation
  B7H3 bead stimulation
  IL-8 cytokine stimulation

The cells were then collected for bulk RNAseq to compare the CAR T cells against each other for each stimulation.

## Folders

The main repository contains R markdown files detailing the analysis of the mapped reads.

Files folders in the repository contain:

### preprocessing scripts
The bash files used to run FastQC and STAR mapping on the cluster server

### genetonic_results
CSV files containing the pathway enrichment results when comparing BC2 vs B7H3 CAR T cells for a given stimulation. Rdata files containing the DESeq object, results object, GeneTonic topgo object, and annotation object. Everything needed to run the GeneTonic browser function

### plots
Initial plots generated after DESeq2 results were put into GeneTonic.

### deseq_results
Gene list csv files detailing the results of the DESeq2 comparisons.

2023_10_09_results
Plots that were a result of 2023_10_09_final_figures.Rmd and 2023_10_23_plot_adjustments.Rmd
There were many iterations of these files, as many small tweaks were made to make plots for publication. So not all plots may have their original code in the markdown files. See subfolders for more recent plots that are reflected in the code.

