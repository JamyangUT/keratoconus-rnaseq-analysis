# Documented Methods

The workflow below summarizes the original capstone report. It has not been rerun for this repository.

## Data and comparison

The report describes **10 keratoconus and 10 control myopia corneal epithelial samples**, with sequencing reads retrieved from NCBI SRA through Galaxy's “Faster Download and Extract Reads in FASTQ” tool.

No SRA/GEO accession or complete sample manifest is provided in the available report text. The related study by You et al. (2018) is discussed in the literature review, but its citation alone is not sufficient to establish the exact data used in this reanalysis.

The controls are myopia samples, rather than a general healthy-population cohort.

## Read assessment and alignment

FastQC assessed sequencing quality. The report mentions a Phred score of 30, but does not provide an exported filtering or trimming step. FastQC evaluates quality; it does not itself remove reads below a threshold.

Reads were aligned to hg38 using HISAT2, producing BAM files. The exact reference/annotation release, alignment parameters, read layout, and strandedness settings are unavailable.

## Quantification and differential expression

featureCounts quantified gene-level reads. The resulting counts were analyzed with EdgeR to compare the two groups. The report presents MDS, biological coefficient of variation, quasi-likelihood, and mean-difference plots.

The exact normalization method, design matrix, dispersion procedure, tested contrast, covariates, and numeric gene-selection thresholds cannot be recovered from the report alone. Its abstract describes prioritization using FDR, p-values, and logFC and selection of ten genes for detailed interpretation.

## Functional interpretation

Enrichr was used for Gene Ontology and pathway enrichment. The report includes Reactome, WikiPathways, and KEGG findings, as well as biological process, cellular component, and molecular function annotations.

The report does not fully specify the enrichment background universe, library versions, or adjusted-significance criteria.

## Reproducibility

The original Galaxy history/workflow exports, scripts, count matrix, sample metadata, and intermediate results are unavailable. No executable pipeline or tested software environment is supplied here.

A future reconstruction would need the exact source accession, sample groups, reference genome and annotation, read-processing settings, counting configuration, EdgeR design/contrast, and enrichment inputs. It should be labeled as a new reanalysis, with results kept separate from the archived report findings.
