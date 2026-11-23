Genetic diversity and population structure of Turkish bread wheat cultivars
===========================================================================

Data and analysis results for the study "Assessment of Genetic Diversity, Population Structure, and Core Collection Design in Turkish Bread Wheat (*Triticum aestivum* L.) Cultivars Using DArTseq-Derived SNP Markers".

The panel consists of 317 Turkish bread wheat cultivars genotyped with the DArTseq platform. After quality control, the data set contains 22,346 SNP markers and 18,652 SilicoDArT presence/absence markers.

Data
----

| File | Content |
| --- | --- |
| `data/cultivars.csv` | The 317 cultivars: sample ID, variety name, genetic cluster (C1 to C5), registration year, growth habit, providing institution, and country of origin |
| `data/Supplementary_Data_S1_SNP_genotype_matrix.csv` | SNP genotype matrix, 22,346 markers (rows) by 317 cultivars (columns), with chromosome and sub-genome of each marker |
| `data/Supplementary_Data_S2_SilicoDArT_matrix.csv` | SilicoDArT presence/absence matrix, 18,652 markers (rows) by 317 cultivars (columns) |
| `data/Supplementary_Data_S3_SNP_marker_information.csv` | SNP marker information: chromosome, physical position (bp), sub-genome, call rate, expected heterozygosity (He), polymorphism information content (PIC), and minor allele frequency (MAF) |

Coding

- SNP genotypes: 0 = homozygous for the reference allele, 1 = heterozygous, 2 = homozygous for the SNP allele, NA = missing.
- SilicoDArT markers: 1 = present, 0 = absent, NA = missing.
- Sample IDs (`Genotype1`, `Genotype100`, ...) are the column headers of the two matrices and link all files to `data/cultivars.csv`.
- In the marker files, NA in the chromosome and position columns marks markers without an assigned chromosome position.
- In `data/cultivars.csv`, NA marks cultivars without a registration year.

Results
-------

| File | Content |
| --- | --- |
| `results/tables/` | Tables 1 to 7 and Supplementary Tables S2 to S6 of the manuscript in CSV format |
| `results/pca_scores.csv` | Scores of the 317 cultivars on the first five principal components |
| `results/genomic_relationship_matrix.csv` | Genomic relationship matrix (317 by 317) |
| `results/admixture/admixture_cv_error.csv` | ADMIXTURE cross-validation error for K = 1 to 10 |
| `results/admixture/admixture_Q_K2.csv` to `admixture_Q_K10.csv` | ADMIXTURE ancestry proportions of each cultivar for K = 2 to 10 |
| `results/structure_evanno.csv` | STRUCTURE mean log-likelihood and Evanno delta K for K = 1 to 10 |
| `results/dapc_cross_validation.csv` | DAPC cross-validation accuracy by number of retained principal components |
| `results/fst_outlier_markers.csv` | The 221 FST outlier markers among clusters C1 to C3, with allele frequencies per cluster and chromosome assignment |
| `results/per_chromosome_diversity.csv` | Marker number and diversity statistics for each of the 21 chromosomes |
| `results/genome_wide_summary.csv` | Global FST, linkage-disequilibrium-based effective population size, and linkage disequilibrium summary values |
| `results/allele_frequency_spectrum.csv` | Folded allele-frequency spectrum in ten MAF classes |
| `results/core_collection_50.csv` | The 50-cultivar core collection in order of selection |
| `results/temporal_diversity_by_era.csv` | Genetic diversity by registration era |
| `results/temporal_cluster_by_decade.csv` | Number of cultivars per genetic cluster and registration decade |
| `results/temporal_registration_year_by_cluster.csv` | Registration year summary for each genetic cluster |

All files are comma-separated text in UTF-8 encoding.

License
-------

The data and results in this repository are released under the Creative Commons Attribution 4.0 International License (CC BY 4.0). The full text is given in the `LICENSE` file.
