# 🧬 Next-Generation Sequencing (NGS)

*20251217*

Next-Generation Sequencing (NGS) refers to a collection of high-throughput DNA and RNA sequencing technologies that enable the parallel sequencing of millions to billions of nucleic acid fragments in a single experiment. Compared with traditional Sanger sequencing, NGS dramatically reduces sequencing cost and time while vastly increasing data output, making genome-scale analyses feasible in both research and clinical settings.

NGS has become a foundational technology in modern **genomics, transcriptomics, epigenomics, microbiome research, and precision medicine**, supporting applications ranging from basic biological discovery to translational and clinical diagnostics.

---

## 1. NGS vs. Conventional Sanger Sequencing

| Feature              | Sanger Sequencing              | Next-Generation Sequencing (NGS)                   |
| -------------------- | ------------------------------ | -------------------------------------------------- |
| Throughput           | Single or few DNA fragments    | Millions to billions of reads per run              |
| Cost per base        | High                           | Low                                                |
| Turnaround time      | Slow                           | Rapid                                              |
| Scalability          | Limited                        | Highly scalable                                    |
| Typical applications | Gene validation, small regions | Whole genomes, transcriptomes, large-scale studies |

---

## 2. Core Components of NGS

NGS is not a single technique but a **complete ecosystem** composed of multiple tightly coupled components:

1. **Wet-lab library preparation**
   Conversion of biological samples into sequencing-ready libraries

2. **Sequencing platforms**
   Instruments and chemistries that generate raw sequencing reads

3. **Computational data processing**
   Bioinformatics pipelines that transform raw reads into biologically meaningful results

4. **Statistical and biological interpretation**
   Downstream analyses, visualization, and hypothesis generation

---

## 3. General NGS Workflow

### 3.1 Sample Preparation

* Extraction of high-quality DNA or RNA
* Optional enrichment or depletion steps (e.g., exome capture, rRNA depletion)
* Library construction:

  * Fragmentation (enzymatic or mechanical)
  * Adapter ligation
  * PCR amplification and indexing

### 3.2 Sequencing

Sequencing is performed on dedicated platforms using platform-specific chemistries:

* **Short-read sequencing**: typically 50–300 bp reads
* **Long-read sequencing**: reads ranging from several kilobases to >100 kb

Common sequencing platforms include:

* Illumina
* Oxford Nanopore Technologies
* Pacific Biosciences (PacBio)

### 3.3 Bioinformatics Data Processing

Key computational steps typically include:

* **Quality control (QC)**: read quality assessment and filtering (e.g., FastQC, fastp)
* **Read alignment or mapping**: alignment to a reference genome or transcriptome (e.g., BWA, STAR, HISAT2)
* **Quantification**:

  * Gene or transcript expression (e.g., featureCounts, Salmon, Kallisto)
  * Variant detection (e.g., GATK, FreeBayes)
* **Downstream analyses**:

  * Differential expression
  * Pathway and functional enrichment
  * Variant annotation and interpretation

---

## 4. Major NGS Applications

| Application                       | Description                                                |
| --------------------------------- | ---------------------------------------------------------- |
| Whole Genome Sequencing (WGS)     | Sequencing of the complete genomic DNA                     |
| Whole Exome Sequencing (WES)      | Targeted sequencing of protein-coding regions              |
| RNA sequencing (RNA-seq)          | Quantification of gene expression and transcript structure |
| Small RNA-seq                     | Profiling of miRNA, siRNA, and other small RNAs            |
| Single-cell RNA-seq               | Transcriptomic analysis at single-cell resolution          |
| ChIP-seq                          | Identification of protein–DNA interaction sites            |
| ATAC-seq                          | Analysis of chromatin accessibility                        |
| 16S rRNA / Metagenomic sequencing | Characterization of microbial communities                  |

---

## 5. Comparison of Major NGS Platforms

| Platform        | Read Type   | Strengths                                         | Limitations                                   |
| --------------- | ----------- | ------------------------------------------------- | --------------------------------------------- |
| Illumina        | Short reads | High accuracy, high throughput                    | Limited ability to resolve repetitive regions |
| Oxford Nanopore | Long reads  | Real-time sequencing, portable devices            | Higher raw error rate                         |
| PacBio (HiFi)   | Long reads  | High accuracy long reads, full-length transcripts | Higher cost                                   |

---

## 6. Common NGS Data Formats

| Format    | Description                              |
| --------- | ---------------------------------------- |
| FASTQ     | Raw sequencing reads with quality scores |
| SAM / BAM | Aligned reads (text / binary)            |
| VCF       | Genetic variants (SNPs, INDELs, SVs)     |
| GTF / GFF | Gene and feature annotations             |
| BED       | Genomic intervals and regions            |

---

## 7. Challenges and Considerations in NGS

* Sequencing depth and coverage design
* Batch effects and technical variability
* Data storage and computational requirements
* Reproducibility and pipeline standardization
* Interpretation of high-dimensional data

---

NGS has become a cornerstone of modern life sciences and precision medicine. A solid understanding of its experimental design, sequencing technologies, and bioinformatics workflows is essential for researchers working in genomics, transcriptomics, and data-driven biomedical research.
