# Transcriptome Summary
A transcriptome analysis will determine what the target genes of the transcription factors by comparing the gene expression in the knock-outs to gene expression in the whole genome sequence of Pantoea YR343. 
We will use FASTQC to perform a quality check. If there are no issues, we will use Trimmomatic to trim the reads. We will use FASTQC again to make sure the quality checks out. Next, we will use HISAT2 to map the sequences to the reference genome. We will first index the genome and then do the actual alignment. We will use Samtools to convert the alignment to bam files. We will use HTSeq to generate counts. We will then use the R package, DeSeq2, to normalize to account for heterogenous transcript distributions. This will give the differential gene expression based on negative binomial distribution. We will download the gene ontology terms from UnitProt and determine a phenotype prediction.  

Outline:
1)Dowload RNA Seqs from SRA and whole genome sequence
2)FASTQC for quality check
3)Trimmomatic to trim
4)FASTQC for quality check
5)HISAT2 to map sequences to reference genome
6)Samtools to visualize alignment
7)HTSeq to generate counts
8)R package, DeSeq2, to normalize and differential expression analysis
9)Download and analyze gene ontology terms from UnitProt
