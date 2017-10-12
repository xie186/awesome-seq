# Table of Contents
1. [Quality control](#quality_control)
2. [Tools for alignment](#alignment)
3. [Tools for DMR](#DMR)
4. [Tools for visulization](#view)
5. [Classic papers](#publication)


# BS-seq_pipeline

## Workflow <a name="workflow"></a>

## Quality control <a name="quality_control"></a>

#### [FastQC](https://www.bioinformatics.babraham.ac.uk/projects/fastqc/)

A quality control tool for high throughput sequence data.

#### [prinseq](http://prinseq.sourceforge.net/)

Easy and rapid quality control and data preprocessing.

#### [Cutadapt](http://cutadapt.readthedocs.io/en/stable/guide.html)

cutadapt removes adapter sequences from sequencing reads



#### 

[BSeQC](https://github.com/hutuqiu/bseqc)

## Tools for assigning methylcytosine

[Bycom]

## Identification of UMRs and LMRs

[MethylSeekR](http://www.bioconductor.org/packages/release/bioc/html/MethylSeekR.html)


## Tools for alignment <a name="alignment"></a>

#### [Bismark](https://www.bioinformatics.babraham.ac.uk/projects/bismark/)

A tool to map bisulfite converted sequence reads and determine cytosine methylation states

#### [MethylDackel](https://github.com/dpryan79/MethylDackel)

A (mostly) universal methylation extractor for BS-seq experiments.

#### [bwa-meth]()

#### [methylpy](https://github.com/yupenghe/methylpy/)

## DMR detection tools <a name="DMR"></a>

#### [swDMR](https://github.com/xflicsu/swDMR)

#### [dmrseq](https://github.com/kdkorthauer/dmrseq) by Keegan Korthauer

#### [methylKit]

A Sliding Window Approach to Identify Differentially Methylated Regions Based on Whole Genome Bisulfite Sequencing

#### [HOME (histogram of methylation)](https://github.com/ListerLab/HOME)

HOME (histogram of methylation) is a python package for differential methylation region (DMR) identification. The method uses histogram of methylation features and the linear Support Vector Machine (SVM) to identify DMRs from whole genome bisulfite sequencing (WGBS) data. HOME can identify both pairwise and time series DMRs with or without replicates. #Installation HOME is written for python 2.7 and tested on Linux system. It is recommended to set up virtual environment for python 2.7 first before installing HOME package.

#### [Differentially Methylated Regions (DMRs) detection](http://www.columbia.edu/~sw2206/softwares.htm)

Most existing methods developed to identify differentially methylated loci (DML) use mean signals only, and only a few methods were developed to identify DML using both mean and variance signals, while all existing methods to detect differentially methylated regions (DMRs) focus on mean signals only. This R code is for the new DMR detection algorithm we proposed that uses mean and variance combined signals

#### [MethylSeekR](https://bioconductor.org/packages/release/bioc/html/MethylSeekR.html)

This is a package for the discovery of regulatory regions from Bis-seq data

#### [methylKit](https://bioconductor.org/packages/release/bioc/html/methylKit.html)

#### [metilene](http://www.bioinf.uni-leipzig.de/Software/metilene/): Fast and sensitive detection of differential DNA methylation


#### [moabs](https://github.com/sunnyisgalaxy/moabs)

Beta-Binomial hierachical model. 

#### [methylpy](https://github.com/yupenghe/methylpy/)

Good for identifying DMRs for multiple groups of samples. 

#### [ABBA](https://github.com/SystemsGeneticsSG/ABBA)

[Paper link](http://www.biorxiv.org/content/biorxiv/early/2017/02/20/041715.full.pdf)


#### [DSS](https://bioconductor.org/packages/release/bioc/html/DSS.html): Dispersion shrinakge for sequencing data.

#### [BAT](http://www.bioinf.uni-leipzig.de/Software/BAT/): Bisulfite Analysis Toolkit

Here, a modular bisulfite analysis toolkit (BAT) is introduced. It tackles the major tasks for analyzing bisulfite sequencing data: mapping, extraction of the methylation information (referred to as methylation calling), and differential methylation analysis as well as downstream analyses like integration of the methylation data with annotation and gene expression data. Each part of this analysis workflow is modular and can easily be customized or extended by other bisulfite- or NGS-related tools, but can also be used as is with the additional benefit of many automatically generated graphics by the modules of BAT.

#### [GEMBS Pipeline](http://statgen.cnag.cat/gemBS/#)

https://www.biorxiv.org/content/early/2017/10/11/201988

GEMBS is a bioinformatic pipeline designed for hightroughput analysis of DNA methylation from whole genome bisulfites sequencing data (WGBS). It implements GEM3, a high performance read aligner and BScall, a variant caller specifically for bisulfite sequencing data.



## Visualization tools <a name="view"></a>

### [ViewBS](https://github.com/xie186/ViewBS)

ViewBS - Tools for exploring and visualizing bisulfite sequencing (BS-seq) data. 

### [BSviewer](http://sunlab.cpy.cuhk.edu.hk/BSviewer/)

BSviewer: a genotype-preserving, nucleotide-level visualizer for bisulfite sequencing data

### [IGV](software.broadinstitute.org/software/igv/)

The Integrative Genomics Viewer (IGV) is a high-performance visualization tool for interactive exploration of large, integrated genomic datasets.


## Classic papers <a name="publication"></a>

### Good paper for data analysis

[Strategies for analyzing bisulfite sequencing data](http://www.biorxiv.org/content/early/2017/02/17/109512)

### Good paper for research 

### [Spatiotemporal DNA Methylome Dynamics of the Developing Mammalian Fetus](http://www.biorxiv.org/content/biorxiv/early/2017/07/21/166744.1.full.pdf)

### [MINI REVIEW: Statistical methods for detecting differentially](http://bioinfo2.ugr.es/DMRs/Robinson_2014_Statistical%20methods%20for%20detecting%20DMCs.pdf)


#### [mint](https://github.com/sartorlab/mint)

A pipeline for the integration of DNA methylation and hydroxymethylation data




