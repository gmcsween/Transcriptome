# Transcriptome Summary
A transcriptome analysis will determine what the target genes of the transcription factors by comparing the gene expression in the knock-outs to gene expression in the whole genome sequence of Pantoea YR343. 
We will use FASTQC to perform a quality check. If there are no issues, we will use Trimmomatic to trim the reads. We will use FASTQC again to make sure the quality checks out. Next, we will use HISAT2 to map the sequences to the reference genome. We will first index the genome and then do the actual alignment. We will use Samtools to visualize the alignment. We will then use the R package, DeSeq2, to normalize to account for heterogenous transcript distributions. This will give the differential gene expression based on negative binomial distribution. The EDGE test will highlight statistically significant changes. We will download the gene ontology terms from UnitProt and do a gene set enrichment analysis (GSEA). We will also use Blast2GO to annotate the transcript. We will use Integrative Genomics Viewer (IGV) to visualize and HTSeq to generate counts. 

Outline:
1)Dowload RNA Seqs from SRA and whole genome sequence
2)FASTQC for quality check
3)Trimmomatic to trim
4)FASTQC for quality check
5)HISAT2 to map sequences to reference genome
6)Samtools to visualize alignment
7)R package, DeSeq2, to normalize
8)EDGE test to highlight statistically significant changes
9)Download gene ontology terms from UnitProt
10)Gene set enrichment analysis
11)BLAST2GO to annotate transcript
12)HTSeq to generate counts
13)IGV to visualize
