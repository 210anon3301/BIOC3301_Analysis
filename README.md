# BIOC3301_Analysis

Respository containing Bash comand line scripts for the metagenomic analysis of soil samples, as part of the UCL BIOC3301 Biochemistry Course.
Scripts were run remotely on Cirrus, a HPC based in Edinburgh, via a Mac desktop computer.

# Scripts used for analysis
# Computing alpha and beta diversities

split_libraries_fastq.pbs

> Demultiplexes fastq sequencing data

pick_de_novo_otus.pbs

> Creates a biom OTU table which may be used in further analysis.

corediv_3000.pbs

> Analysis programme producing various data, including alpha and beta diversities, taxonomy, and OTU counts.


# Creating OTU Heatmap

compute_core_microbiome.pbs

> Uses OTU table from pick_de_novo_otus.pbs to find core OTUs

otu_heatmap.pbs

> Creates a heatmap using the core OTUs. This gives a measure of beta diversity.


# Producing ANOSIM Statistics

all scripts in anosim folder

> Performs a statistical test on beta diversity data to find metadata that may be significant.
