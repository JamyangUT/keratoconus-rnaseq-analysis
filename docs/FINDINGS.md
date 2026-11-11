# Findings and Limitations

These findings summarize the capstone report and its original figures. They are not newly computed results.

## Prioritized genes

The original annotation table lists:

| Gene ID | Symbol | Annotation in the report |
| ---: | --- | --- |
| 8939 | FUBP3 | Far upstream element binding protein 3 |
| 9877 | ZC3H11A | Zinc finger CCCH-type containing 11A |
| 1783 | DYNC1LI2 | Dynein cytoplasmic 1 light intermediate chain 2 |
| 8731 | RNMT | RNA guanine-7 methyltransferase |
| 84640 | USP38 | Ubiquitin-specific peptidase 38 |
| 6240 | RRM1 | Ribonucleotide reductase catalytic subunit M1 |
| 79977 | GRHL2 | Grainyhead-like transcription factor 2 |
| 5770 | PTPN1 | Protein tyrosine phosphatase non-receptor type 1 |
| 9354 | UBE4A | Ubiquitination factor E4A |
| 55717 | WDR11 | WD repeat domain 11 |

The abstract particularly highlights FUBP3, ZC3H11A, DYNC1LI2, and RNMT. This prioritization supplies hypotheses for follow-up rather than evidence of diagnostic performance or therapeutic efficacy.

## Functional themes

The interpretation discusses RNA capping and binding, protein homeostasis, intracellular transport, receptor signaling, cell adhesion, corneal maintenance, and oxidative stress. Pathway associations do not establish that a specific pathway caused keratoconus in the analyzed samples.

## Sample structure and differential expression

The MDS figure and report describe sex-related structure among controls. The available methods do not establish how this covariate was handled in the disease comparison.

The report describes predominantly downregulated expression, including 25,967 downregulated genes, 2,428 classified as flat, and none upregulated in one EdgeR summary. The original design, contrast direction, count normalization, and input matrix are unavailable, so these counts should not be interpreted as a verified global disease mechanism. The pronounced directionality warrants checking those analysis choices in any reconstruction.

## Interpretation limits

- The sample set is small and compares keratoconus with myopia controls.
- Sex-related sample structure may complicate the disease contrast.
- Exact thresholds, covariates, normalization, and source accession are incompletely documented.
- There is no independent-cohort or experimental validation of the shortlisted candidates in the supplied capstone.
- Gene expression in corneal epithelium does not by itself establish a mechanism in other corneal tissues.
- Original executable workflows and intermediate files are unavailable.

## Follow-up priorities

Recover the original sample manifest and count data, audit the design/contrast and normalization, account for covariates where supported, and evaluate candidates in independent cohorts and biological experiments.
