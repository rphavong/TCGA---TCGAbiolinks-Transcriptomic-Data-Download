This R code extracts RNA-seq data of sex chromosome genes of interest from The Cancer Genome Atlas (TCGA) using TCGAbiolinks R package. 
From the sex chromosome genes of interest RNA-seq in TPM, we inferred sex chromosome complements by a determined low, intermediate and high threshold based on their TPM counts. 
Similarly, within the TCGA cancer resourse, several cancer studies contain samples of the same patient where a normal sample was taken denoted as "Solid Tissue Normal" and the tumor denoted as "Primary Tumor". 
Samples that contained "Solid Tissue Normal" were matched to their respective "Primary Tumor" sample based on their matching "cases.submitter_id", from which sex chromosome genes of interest were compared between Solid Tissue Normal to respective Primary Tumor.
It is good to note that samples that contained repeated cases for the same patient, such as repeated Solid Tissue Normal or Primary Tumor samples were excluded. 
