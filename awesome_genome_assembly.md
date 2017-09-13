#  

## Suggested data for genome assembly

1. 

2. PacBio Long reads 

3. BioNano 


## Scaffolding methods

Scaffolding using RNA-seq data
Scaffolding using HiC-seq data
Scaffolding using homologous genes


## 

It depends a lot on what you are planning to do with your PacBio data. For assembly and error correction, there are different strategies:

Ideal coverage required for PacBio error correction using HGAP + PacBio assembly (HGAP, FALCON, etc..) would requires >50X coverage.
What tools you use or know for PacBio Long Read error correction? + some form of hybrid or low coverage PacBio assembly (FALCON). This works with 10-20X coverage + >50X Illumina. However correction can be computationally intensive for a 1.5GB genome and I haven't seen a adequate hybrid assembler for this size of genome.
Scaffolding + Gapclosing (pbJelly2, sspace-longread, finisherSC) can be done with raw or error corrected PacBio reads and 10X coverage should be sufficient
Also, I've seen a lot of issues with large/repetitive plant genomes and library prep/size selection for PacBio. Make sure to test your protocols. Good subread length is very important if you do low coverage PacBio. With short subreads you may get a theoretical coverage of 10X, but since all subreads from one read stack onto each other, you'll have much less real overlapping fragments than you need for assembly/scaffolding
