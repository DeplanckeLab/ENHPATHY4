# ENHPATHY Event IV - Hands-on session on analyzing single-cell data
EPFL course by Vincent Gardeux

***

06.04.2022 - Prague

<br/>

In recent years, single-cell transcriptomics has become a widely used technology to study heterogeneous and dynamic biological systems. A large number of new tools and approaches have been developed for analyzing this new type of data.

The goal of this hands-on session is to provide theoretical and practical knowledge in the basic analysis of single-cell RNA-seq datasets.

This course covers the standard analysis of a single-cell RNA-seq dataset using the Seurat pipeline.
It follows to some extent the ["standard tutorial from Seurat"](https://satijalab.org/seurat/articles/pbmc3k_tutorial.html), which we encourage the readers to consult when they want to dive more into single-cell data analyis.

In this course, we will use an example data set consisting of 7,000 cells from the ["Fly Cell Atlas"](https://flycellatlas.org/) repository. These cells all come from the **Body** part, which was dissociated as a whole and sequenced using 10x Genomics technology over 10 batches, mixing males and females.

This set of 7,000 cells was carefully selected/filtered from the original **Body dataset** that consists of 96,926 cells. They belong to *a certain number* of differently annotated cell types.

<div style="width:100%; height:150px; text-align: center">

  <a href="/single-cell_sib_scilifelab_2021/project_spatial/README.html">
  <div class="zoom" style="width:150px;height:100px;padding:5px 5px;font-size:12pt;font-family:Helvetica;float:left;text-align:center;">
  <img border="0" height="100px" src="logos/spatial_transcriptomics.png"><br/>
  Spatial<br/>transcriptomics
  </div>
  </a>

  <a href="/single-cell_sib_scilifelab_2021/project_velocity/README.html">
  <div class="zoom" style="width:150px;height:100px;padding:5px 5px;font-size:12pt;font-family:Helvetica;float:left;text-align:center;">
  <img border="0" height="100px"  src="logos/rna_velocity.png"><br/>
  RNA<br/>velocity
  </div>
  </a>

  <a href="/single-cell_sib_scilifelab_2021/project_omics/README.html">
  <div class="zoom" style="width:150px;height:100px;padding:5px 5px;font-size:12pt;font-family:Helvetica;float:left;text-align:center;">
  <img border="0" height="100px"  src="logos/omics_integration.png"><br/>
  Omics<br/>integration
  </div>
  </a>

  <a href="/single-cell_sib_scilifelab_2021/project_dnn/README.html">
  <div class="zoom" style="width:150px;height:100px;padding:5px 5px;font-size:12pt;font-family:Helvetica;float:left;text-align:center;">
  <img border="0" height="100px" src="logos/deep_learning.png"><br/>
  Deep<br/>learning
  </div>
  </a>

</div>

<br/>

**Audience**
This course is addressed to any participant, with or without knowledge of bioinformatics. The R coding is very light, and will be explained in details so that anybody should be able to adress the different questions.

<br/>

# <img border="0" src="https://www.svgrepo.com/show/20800/event-date-and-time-symbol.svg" width="40" height="40" style="vertical-align:middle;"> Date

***

06.04.2022 - Prague

<br/>

# <img border="0" src="https://www.svgrepo.com/show/4199/placeholder-on-a-map.svg" width="40" height="40" style="vertical-align:middle;"> Location

***

This course will take place on-site, at the ENHPATHY event IV meeting, in Prague.


<br/>

# <img border="0" src="https://www.svgrepo.com/show/158264/schedule.svg" width="40" height="40" style="vertical-align:middle;"> Programme

***

After a short introduction to single-cell genomics, and more particularly single-cell transcriptomics, we will go to and R exercise together.

For the full schedule of the ENHPATHY meeting, please go to: **[Schedule](ENHPATHY-Event-IV-Program.pdf)**

<br/>

# <img border="0" src="https://www.svgrepo.com/show/410/list.svg" width="40" height="40" style="vertical-align:middle;"> Learning objectives

***

At the end of this session, the participants should be able to:
- have a global knowledge of what is single-cell genomics, and in particular single-cell transcriptomics,
- have a good understanding of the generic analysis pipeline for scRNA-seq,
- repeat the same type of analysis achieved during the mini-project,
- present the mini-project and more globally disseminate their experience to the members of their group.


**Pre-requisites - background knowledge**
- Intermediate/advanced usage of R is a plus

**Pre-requisites - material & software**
- The participants must use a laptop with install permissions (admin). R and Rstudio should be installed on their machine. A list of packages to be installed will be communicated during the course, it includes the following:
```r
install.packages("Seurat")
install.packages("data.table")
```

<br/>

# <img border="0" src="https://www.svgrepo.com/show/38706/group-of-people.svg" width="40" height="40" style="vertical-align:middle;"> Staff

***

## Lecturer:

- __*Vincent Gardeux*__, Senior Scientist, EPFL, Lausanne, 🇨🇭 Switzerland

<br/>
<br/>

**Additional information**

For more information, please contact [vincent.gardeux@epfl.ch](mailto://vincent.gardeux@epfl.ch).
