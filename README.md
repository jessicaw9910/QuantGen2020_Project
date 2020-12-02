# Genome-Wide Association Analysis of Subset of Data from gEUVADIS Consortium

**The experiment:** Among the recent large scale human genomics resources is Genetic European Variation in Health and Disease (gEUVADIS) - see the following links for relevant descriptions and information:

[http://www.internationalgenome.org/data-portal/data-collection/geuvadis/](http://www.internationalgenome.org/data-portal/data-collection/geuvadis/)
[https://www.nature.com/articles/nature12531](http://www.internationalgenome.org/data-portal/data-collection/geuvadis/)

with a samples from 4 different European populations (5 populations total). Each of these individuals were part of the 1000 Genomes project and their genomes were sequenced and analyzed to identify SNP geno- types. For expression profiling, lympoblastoid cell lines (LCL) were generated from each sample and mRNA levels were quantified through RNA sequencing.

Each of these gene expression measurements may be thought of as a phenotype and one can do a GWAS analysis on each individually, which is called an 'expression Quantitative Trait Locus' or 'eQTL' analysis, an unnecessarily fancy name for a GWAS when the phenotype is gene expression!

What you have been provided is a small subset of these data that are publicly available. Specifically, you have been provided 50,000 of the SNP genotypes for 344 samples from the CEU (Utah residents with European ancestry), FIN (Finns), GBR (British) and, TSI (Toscani) population.

For these same individuals, you have also been provided the expression levels of five genes. You have also been provided information on the population and gender of each of these individuals, and information regarding the position of each gene and SNP in the genome.

**The data:** These have been provided to you in five total files: `phenotypes.csv`,`genotypes.csv`, `covars.csv`, `gene info.csv`, `SNP info.csv`.
+ `phenotypes.csv` contains the phenotype data for 344 samples and 5 genes.
+ `genotypes.csv` contains the SNP data for 344 samples and 50000 genotypes.
+ `covars.csv` contains the population origin and gender information for the 344 samples.
+ `gene info.csv` contains information about each gene that was measured. The 'chromosome' column indicates the chromosome where the gene is located, 'start' marks the position in the chromosome where the region of the gene begins and 'end' marks the position where the region ends, 'symbol' contains the common gene name of the measured transcript and 'probe' contains the ids of the trancripts that match with the column names of the phenotype data.
+ `SNP info.csv` contains the additional information on the genotypes and has four columns. The 1st column contains the chromosome number of each SNP, the 2nd column contains the physical
position of the SNP on the chromosome, the 3rd column contains the abbreviation used to the 'rsID' = the name of each SNP in order.

**The assignment:** Your GWAS assignment is to find the position of as many causal polymorphisms as possible for the five expressed genes using the data (note that each 'hit' will potentially indicate an eQTL). You may/should use any and as many analysis approaches as you think that are useful to accomplish this goal. In your report, you will need to describe in detail what you did, why you did it, and describe results in a manner that your  'non-statistical' collaborator will be able to understand, e.g. explain your terms, provide interpretations, etc.