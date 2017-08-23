# Table of Contents
1. [Read quality control](#quality_control)
2. [Tools for alignment](#alignment)
3. [Tools for DMR](#DMR)
4. [Tools for visulization](#view)
5. [Classic papers](#publication)


# BS-seq_pipeline

## Workflow <a name="workflow"></a>

## Read quality control <a name="quality_control"></a>

#### [FastQC](https://www.bioinformatics.babraham.ac.uk/projects/fastqc/)

A quality control tool for high throughput sequence data.

#### [prinseq](http://prinseq.sourceforge.net/)

Easy and rapid quality control and data preprocessing.

#### [Cutadapt](http://cutadapt.readthedocs.io/en/stable/guide.html)

cutadapt removes adapter sequences from sequencing reads

## Tools for alignment <a name="alignment"></a>

#### [Bismark](https://www.bioinformatics.babraham.ac.uk/projects/bismark/)

A tool to map bisulfite converted sequence reads and determine cytosine methylation states

#### [methylpy](https://github.com/yupenghe/methylpy/)

## DMR detection tools <a name="DMR"></a>

#### [swDMR](https://github.com/xflicsu/swDMR)

A Sliding Window Approach to Identify Differentially Methylated Regions Based on Whole Genome Bisulfite Sequencing

#### [HOME (histogram of methylation)](https://github.com/ListerLab/HOME)

HOME (histogram of methylation) is a python package for differential methylation region (DMR) identification. The method uses histogram of methylation features and the linear Support Vector Machine (SVM) to identify DMRs from whole genome bisulfite sequencing (WGBS) data. HOME can identify both pairwise and time series DMRs with or without replicates. #Installation HOME is written for python 2.7 and tested on Linux system. It is recommended to set up virtual environment for python 2.7 first before installing HOME package.

#### [Differentially Methylated Regions (DMRs) detection](http://www.columbia.edu/~sw2206/softwares.htm)

Most existing methods developed to identify differentially methylated loci (DML) use mean signals only, and only a few methods were developed to identify DML using both mean and variance signals, while all existing methods to detect differentially methylated regions (DMRs) focus on mean signals only. This R code is for the new DMR detection algorithm we proposed that uses mean and variance combined signals.

#### [MethylSeekR](https://bioconductor.org/packages/release/bioc/html/MethylSeekR.html)

This is a package for the discovery of regulatory regions from Bis-seq data



#### [methylpy](https://github.com/yupenghe/methylpy/)

Good for identifying DMRs for multiple groups of samples. 


## Visualization tools <a name="view"></a>

### [ViewBS](https://github.com/xie186/ViewBS)

ViewBS - Tools for exploring and visualizing bisulfite sequencing (BS-seq) data. 

### [BSviewer](http://sunlab.cpy.cuhk.edu.hk/BSviewer/)

BSviewer: a genotype-preserving, nucleotide-level visualizer for bisulfite sequencing data

### [IGV](software.broadinstitute.org/software/igv/)

The Integrative Genomics Viewer (IGV) is a high-performance visualization tool for interactive exploration of large, integrated genomic datasets.


## Classic papers <a name="publication"></a>
### [Spatiotemporal DNA Methylome Dynamics of the Developing Mammalian Fetus](http://www.biorxiv.org/content/biorxiv/early/2017/07/21/166744.1.full.pdf)

### [MINI REVIEW: Statistical methods for detecting differentially](http://bioinfo2.ugr.es/DMRs/Robinson_2014_Statistical%20methods%20for%20detecting%20DMCs.pdf)








