---
title: "ENHPATHY - Hands-on: Analyzing single-cell data"
author: "Vincent Gardeux"
date: "April 6th 2022"
output:
  rmarkdown::html_document:
    highlight: pygments
    toc: true
    toc_depth: 3
    fig_width: 5
    keep_md: yes
editor_options: 
  chunk_output_type: console
---



## Introduction

This course covers the standard analysis of a single-cell RNA-seq dataset using the Seurat pipeline.
It follows to some extent the ["standard tutorial from Seurat"](https://satijalab.org/seurat/articles/pbmc3k_tutorial.html), which we encourage the readers to consult when they want to dive more into single-cell data analyis.

In this course, we will use an example data set consisting of 7,000 cells from the ["Fly Cell Atlas"](https://flycellatlas.org/) repository. These cells all come from the **Body** part, which was dissociated as a whole and sequenced using 10x Genomics technology over 10 batches, mixing males and females.

This set of 7,000 cells was carefully selected/filtered from the original **Body dataset** that consists of 96,926 cells. They belong to *a certain number* of differently annotated cell types.

The goal of this exercise session is to:

1. Find out how many cell types there are in the data set
2. Annotate the cell types using FlyEnrichr (https://maayanlab.cloud/FlyEnrichr/)

## Step 1: Loading the data and create a Seurat object

To be able to run the Seurat pipeline, you need to create a Seurat object in R.
This step mainly depends on the format of the data you have, to start with. For example:

1. If coming from GEO, or other repositories, it could be in ".txt", ".tsv", ... i.e. in a TEXT format
2. If coming from single-cell repositories, it could be in .loom or .h5ad format
3. If you ran CellRanger (10x libraries), then you end up with a folder containing .mtx and .tsv files
4. If coming from your sequencing facility, it could still be in the form of .fastq or .bam. In this case, you cannot import the data in R yet, you need to finish preprocessing the files (i.e. run STARsolo or CellRanger)

Here, the data is in **text format**: tab-separated, with header and row names.
In this case, the first thing to do is to read your file in R and create a data.frame/matrix containing your object.
Since the file is gzipped, and the file is big enough, we will use the package `data.table` to do so. Especially the `fread()` function in this package:


```r
summary(cars)
```

```
##      speed           dist       
##  Min.   : 4.0   Min.   :  2.00  
##  1st Qu.:12.0   1st Qu.: 26.00  
##  Median :15.0   Median : 36.00  
##  Mean   :15.4   Mean   : 42.98  
##  3rd Qu.:19.0   3rd Qu.: 56.00  
##  Max.   :25.0   Max.   :120.00
```


## Conclusion

Of course, it is possible to run this whole analysis in R without using the Seurat framework. An online book, ["Orchestrating single-cell analysis with Bioconductor"](https://osca.bioconductor.org/), is an excellent resource for performing this.