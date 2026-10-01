# Introduction to single-cell RNA-seq data analysis

### 9<sup>th</sup>, 12<sup>th</sup>, 16<sup>th</sup> October 2026 || 09:30 - 17:30
#### Online via Zoom

![](SingleCell_Seurat_Base/Images/uniOfCamCrukLogos.png)

## Instructors

- Adam Reid (Gurdon Institute)
- Chandra Chilamakuri (CRUK-CI)
- Yunxiao Wang
- Guest Speaker: Kasia Kania (Cosyne Therapeutics)

## Outline

This workshop is aimed at biologists interested in learning how to perform
standard single-cell RNA-seq analyses.

This will focus on the droplet-based assay by 10X genomics and include running
the accompanying `cellranger` pipeline to align reads to a genome reference and
count the number of read per gene, reading the count data into R, quality control,
normalisation, data set integration, clustering and identification of cluster
marker genes, as well as differential expression and abundance analyses.
You will also learn how to generate common plots for analysis and visualisation
of gene expression data, such as TSNE, UMAP and violin plots.

> ## Prerequisites
>
> __**Some basic experience of using a UNIX/LINUX command line is assumed**__
>
> __**Some R knowledge is assumed and essential. Without it, you
> will struggle on this course.**__
> If you are not familiar with the R statistical programming language we
> strongly encourage you to work through an introductory R course before
> attempting these materials.
> We recommend our [Introduction to R course](https://bioinformatics-core-shared-training.github.io/r-intro/).

## Data

* The course data is based on '[CaronBourque2020](https://www.nature.com/articles/s41598-020-64929-x)'
  relating to pediatric leukemia, with four sample types, including:
  * pediatric Bone Marrow Mononuclear Cells (PBMMCs)
  * three tumour types: ETV6-RUNX1, HHD, PRE-T  
* The data used in the course can be [downloaded from Dropbox](https://www.dropbox.com/scl/fo/9x1rg6qxqw5crq2vtb1ho/AMawguf1kqRYQQs-qZPhFZA?rlkey=6y4w1skyjzpq36zfyocis24t6&st=vh4vbsvc&dl=0). Please note that:
  * these data have been processed for teaching purposes and are therefore not suitable for research use;
  * all the data is provided on our training machines, you don't need to download it to attend the course.

## Schedule

**PDF of materials:** if you want a PDF version of the materials go to the "Print" option on your browser and select "Print to PDF" (all major browsers have this functionality).

<div style="background-color: #eef3f8; padding: 14px; border: 1px solid #b6c2cf; border-left: 5px solid #4a6fa5; border-radius: 6px;">
    <h2 style="color: #2f4a6d; font-size: 1.1em; margin-top: 0; margin-bottom: 0.5em;">
        Latest Course Materials
    </h2>
    <p style="color: #333; margin: 0 0 0.8em 0;">
        The materials for this course are regularly updated. Please ensure you have the latest version by visiting our course history page:
    <a href="https://bioinformatics-core-shared-training.github.io/UnivCambridge_ScRnaSeqIntro_Base/" style="color: #2f4a6d" target="_blank">
        <b>Single-cell RNA-seq analysis - course listing</b>
    </a>
    </p>
</div>

### Day 1


* 09:30 - 09:45 **Welcome**
* 09:45 - 10:30 **Introduction to Single Cell Technologies** - Katarzyna Kania
    + [Slides](SingleCell_Seurat_Base/Slides/01_Introduction.html) ([pdf](SingleCell_Seurat_Base/Slides/01_Introduction.pdf))
* 10:30 - 10:44 **Preamble**: data set and workflow - Daianna  
    + [Slides](SingleCell_Seurat_Base/Slides/02_PreambleSlides.html) ([pdf](SingleCell_Seurat_Base/Slides/02_PreambleSlides.pdf))
* 10:45 - 11:00 - **Break**
* 11:00 - 12:30 Library structure, **cellranger** for alignment and cell calling - Daianna   
    + [Slides](SingleCell_Seurat_Base/Slides/03_CellRangerSlides.html) ([pdf](SingleCell_Seurat_Base/Slides/03_CellRangerSlides.pdf))
    + [Demonstration](SingleCell_Seurat_Base/Markdowns/03_CellRanger.html)
* 12:30 - 13:30 **Lunch break**
* 13:30 - 17:00 **QC and exploratory analysis** - Adam  
    + [Slides](SingleCell_Seurat_Base/Slides/04_QualityControlSlides.html) ([pdf](SingleCell_Seurat_Base/Slides/04_QualityControlSlides.pdf))
    + [Demonstration](SingleCell_Seurat_Base/Markdowns/04_Preprocessing_And_QC.html)
        

### Day 2


* 09:30 - 09:40 **Recap** - Ash  
    + [Slides](SingleCell_Seurat_Base/Slides/00_Day1_Recap.html) ([pdf](SingleCell_Seurat_Base/Slides/00_Day1_Recap.pdf))
* 09:40 - 12:30 **Normalisation and feature selection** - Ash  
    + [Slides](SingleCell_Seurat_Base/Slides/05_NormalisationSlides.html) ([pdf](SingleCell_Seurat_Base/Slides/05_NormalisationSlides.pdf))
    + [Demonstration](SingleCell_Seurat_Base/Markdowns/05_NormalisationAndFeatureSelection.html)    
* 12:30 - 13:30 **lunch break**
* 13:30 - 15:25 **Dimensionality reduction** - Adam  
    + [Slides](SingleCell_Seurat_Base/Slides/06_DimensionalityReduction_slides.html) ([pdf](SingleCell_Seurat_Base/Slides/06_DimensionalityReduction_slides.pdf))
    + [Demonstration](SingleCell_Seurat_Base/Markdowns/06_DimensionalityReduction.html)
* 15:25 - 15:35 10 min **break**
* 15:35 - 17:30 **Batch correction and data set integration** - Daianna   
    + [Slides](SingleCell_Seurat_Base/Slides/07_DatasetIntegrationSlides.html) ([pdf](SingleCell_Seurat_Base/Slides/07_DatasetIntegrationSlides.pdf))
    + [Demonstration](SingleCell_Seurat_Base/Markdowns/07_Dataset_Integration.html)
   

### Day 3

* 09:30 - 09:40 Recap - Adam
* 09:40 - 11:05 **Cell clustering** - Adam
    + [Slides](SingleCell_Seurat_Base/Slides/08_Clustering_Slides.html) ([pdf](SingleCell_Seurat_Base/Slides/08_Clustering_Slides.pdf))
    + [Demonstration](SingleCell_Seurat_Base/Markdowns/08_Clustering.html)
* 11:05 - 11:15 10 min **break**
* 11:15 - 12:30 **Identification of cluster marker genes** - Adam
    + [Slides](SingleCell_Seurat_Base/Slides/09_ClusterMarkerGenes.html) ([pdf](SingleCell_Seurat_Base/Slides/09_ClusterMarkerGenes.pdf))
    + [Demonstration](SingleCell_Seurat_Base/Markdowns/09_Cluster_Marker_Genes.html)
* 12:30 - 13:30 **lunch break**
* 13:30 - 16.00 **Differential Expression Analysis** - Daianna
	+ [Slides](SingleCell_Seurat_Base/Slides/10_Differential_Expression_Slides.html) ([pdf](SingleCell_Seurat_Base/Slides/10_Differential_Expression_Slides.pdf))
	+ [Demonstration](SingleCell_Seurat_Base/Markdowns/10_Differential_Expression.html)
* 16.00 - 17.30 **Differential Abundance Analysis** - Ash
	+ [Slides](SingleCell_Seurat_Base/Slides/11_Differential_Abundance_Slides.html) ([pdf](SingleCell_Seurat_Base/Slides/11_Differential_Abundance_Slides.pdf))
	+ [Conversion to SingleCellExperiment](SingleCell_Seurat_Base/Markdowns/10a_ConversionToSCE.html)
	+ [Milo Demonstration](SingleCell_Seurat_Base/Markdowns/11_Differential_Abundance.html)


## Software Installation

You can make use of the computer environment provided for the course, which is ready for use and have the necessary data & software installed.
However, if you want to run the analysis on your own computer, you can follow these instructions.

* Download and install R: https://cloud.r-project.org/
  * (Windows users only): Download and install RTools: https://cran.r-project.org/bin/windows/Rtools/
* Download and install RStudio: https://www.rstudio.com/products/rstudio/download/#download
* Open RStudio and run the following commands from the console:

    ```r
    install.packages("BiocManager")
    BiocManager::install(c("sctransform",
                           "Seurat",
                           "tidyverse",
                           "ggbeeswarm",
                           "glmGamPoi",
                           "patchwork",
                           "SparseArray",
                           "scales",
                           "bluster",
                           "cluster",
                           "DESeq2",
                           "SingleCellExperiment",
                           "scater",
                           "BiocParallel",
                           "miloR",
                           "scran",
                           "Matrix"))

    # for much faster FindAllMarkers()
    remotes::install_github("immunogenomics/presto")
    ```

For Cellranger, you will need to use a Linux machine.
See the [installation instructions from 10x Genomics](https://www.10xgenomics.com/support/software/cell-ranger/latest/tutorials/cr-tutorial-in).


## Acknowledgments:

This version of the course is a rewrite by Abigail Edwards and Hugo Tavares using the [Seurat](https://satijalab.org/seurat/) package of the original course developed as detailed below

Much of the material has been derived from the demonstrations found in the
[OSCA book](https://bioconductor.org/books/release/OSCA/)
and the [Hemberg Group course materials](https://www.singlecellcourse.org/). 
Additional material concerning `miloR` has been based on the [demonstration from the Marioni Lab](https://marionilab.github.io/miloR/articles/milo_demo.html).

The materials have been contributed to by many individuals over the last several years, including:

- Abigail Edwards
- Adam Reid
- Ashley D Sawle
- Chandra Chilamakuri
- Hugo Tavares
- Jon Price
- Kamal Kishore
- Katarzyna Kania
- Roderik Kortlever
- Stephane Ballereau
- Tom Smith
- Zeynep Kalendar Atak

Apologies if we have missed anyone!
