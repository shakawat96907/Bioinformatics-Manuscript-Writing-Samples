# Materials and Methods

## Data Sources and Study Design

This study analyzed public multi-omics datasets primarily from The Cancer Genome Atlas (TCGA), with external validation where appropriate. The overall analytical workflow is summarized in Figure 1.

The analysis pipeline integrated the following public platforms and databases:

- **TIMER2.0** — Gene expression, immune infiltration, and co-expression analysis (ref 29)
- **GEPIA2** — Differential expression integrating TCGA + GTEx, stage-wise and correlation analyses (ref 30)
- **UALCAN** — Protein-level validation, promoter methylation, and clinicopathological correlation (ref 31)
- **CPTAC** — Reverse-phase protein array and mass-spectrometry-based proteomics (via UALCAN)
- **Human Protein Atlas (HPA)** — Immunohistochemistry validation (ref 32)
- **SMART** — CpG methylation profiling (ref 33)
- **cBioPortal** — Genomic alteration analysis across TCGA PanCancer Atlas (ref 35)
- **TCGAplot (v8.0.0)** — Univariate Cox regression and data visualization in R v4.5.2 (ref 36)
- **GSCA** — Pharmacogenomic integration of GDSC and CTRP datasets (ref 40)
- **TISCH2** — Single-cell RNA sequencing across 12 cancer types (ref 39)
- **STRING (v12.0)** — Protein-protein interaction network (ref 43)
- **Enrichr** — Functional enrichment of GO (BP, CC, MF) and pathway databases (KEGG, Reactome, WikiPathways) (refs 45-48)

## Cell Line Authentication and Mycoplasma Testing

As this study utilized no experimental cell lines or laboratory assays, cell line authentication and mycoplasma testing were not applicable.

## Gene Expression Analysis

TMEM45A transcriptomic expression across TCGA malignancies was evaluated using the **Gene_DE module of TIMER2.0**. Differential expression between tumor and normal tissues was independently validated using the **GEPIA2 Expression DIY module**, integrating TCGA and GTEx datasets to compensate for limited TCGA normal samples.

Correlations between TMEM45A expression and pathological stage were assessed via GEPIA2 and cross-validated using **UALCAN**. Differential TMEM45A expression between tumor and GTEx normal tissues was validated using the GEPIA2 Expression DIY module, with significance set at **p < 0.05**.

## Proteomics Analysis and Immunohistochemistry

TMEM45A protein abundance was evaluated across **CPTAC datasets via UALCAN**. Representative immunohistochemical (IHC) staining using the **HPA062101 antibody** (Human Protein Atlas) validated protein expression patterns in paired tumor and normal tissues.

## Survival Analysis

The prognostic significance of TMEM45A across 33 TCGA malignancies was evaluated via **GEPIA2**. Overall survival (OS) and disease-free survival (DFS) were assessed using **median expression** to stratify patients into high- and low-expression groups. Survival differences were evaluated by the **log-rank test**, reporting hazard ratios (HRs) and 95% confidence intervals (CIs); **p < 0.05** was considered statistically significant.

## DNA Methylation Analysis

Probe-level CpG methylation of TMEM45A across TCGA cohorts was evaluated using **SMART**. Promoter methylation across 33 TCGA malignancies was analyzed in **UALCAN**, comparing primary tumors against paired normal controls.

- Methylation was quantified as **beta-values** (0 = unmethylated, 1 = fully methylated)
- Hypermethylation: 0.50-0.70; Hypomethylation: 0.25-0.30
- Group differences evaluated by **unpaired two-sample t-test**

## Genetic Alteration Analysis of TMEM45A

TMEM45A genetic alterations were evaluated across the **TCGA PanCancer Atlas** via **cBioPortal**. Alteration frequencies, mutation types, and cross-cancer distributions were assessed using the Cancer Types Summary module, while amino acid substitution patterns across protein domains were examined via the Mutations module.

Associations between TMEM45A alterations and clinical outcomes (overall survival [OS] and progression-free survival [PFS]) were evaluated by Kaplan-Meier analyses using the Comparison/Survival module.

## Pan-cancer Prognostic Analysis

The prognostic value of TMEM45A across TCGA cohorts was evaluated using **univariate Cox proportional hazards regression via the TCGAplot package (v8.0.0)** in R (v4.5.2), reporting hazard ratios (HRs) and 95% confidence intervals (CIs) for overall survival as forest plots.

- **HR > 1** indicated elevated mortality risk
- **HR < 1** indicated reduced risk
- Two-sided **p < 0.05** considered statistically significant

## Immune Infiltration, Tumor Mutation Burden, and Microsatellite Instability Analysis

Immune cell infiltration (CD8+ T cells, NK cells, and CAFs) was evaluated across TCGA cohorts using **TIMER2.0 with the EPIC algorithm**. Confounding non-tumor cellular components were controlled via **purity-adjusted partial Spearman correlation**.

Correlations between TMEM45A expression and:

- **Tumor mutation burden (TMB)** — evaluated by Pearson correlation
- **Microsatellite instability (MSI)** — evaluated by Pearson correlation

Data processing and visualization were performed using **ggplot2, dplyr, and TCGAplot** in R (v4.5.2). Significance was set at **p < 0.05** (corrected for multiple testing where applicable).

## Immune Regulatory Signature Analysis

Associations between TMEM45A expression and immune regulatory signatures — including immune scores, immune checkpoints, immunoinhibitors, immunostimulators, chemokines, and chemokine receptors — were evaluated across TCGA cohorts.

- Differential expression between high- and low-TMEM45A groups: **Wilcoxon rank-sum test** (TCGAplot v8.0.0, R v4.5.2)
- Gene correlations: **Spearman's rank correlation**

## Single-Cell Transcriptomic Analysis

Single-cell TMEM45A expression was evaluated using the **Gene module of TISCH2** across 12 cancer types:

- LUAD (NSCLC datasets)
- BRCA
- STAD
- LIHC
- HNSC
- UCEC
- BLCA
- KIRC
- SKCM
- PAAD
- SARC
- OV

Representative datasets with validated cell-type annotations were analyzed to characterize the cellular distribution of TMEM45A across annotated tumor, immune, and stromal cell populations.

## Drug Sensitivity Analysis

The association between TMEM45A expression and anticancer drug sensitivity was evaluated using the **Gene Set Cancer Analysis (GSCA) platform**, integrating TCGA transcriptomic profiles with pharmacogenomic datasets from:

- **Genomics of Drug Sensitivity in Cancer (GDSC)**
- **Cancer Therapeutics Response Portal (CTRP)**

**Spearman correlation analysis** assessed relationships between TMEM45A expression and half-maximal inhibitory concentration (IC50) values.

- **Positive correlation** (p > 0) indicated **reduced drug sensitivity**
- **Negative correlation** (p < 0) indicated **greater predicted sensitivity**

## Protein-Protein Interaction and Functional Enrichment Analysis

A TMEM45A-centered protein-protein interaction (PPI) network was constructed in **STRING (v12.0)** using all evidence sources and a minimum interaction score of 0.150.

- The **top 50 interacting proteins** (ranked by STRING confidence score) were retained
- Intersected with the **top 100 positively co-expressed genes** from GEPIA2 using **InteractiVenn**
- Co-expression validated using TIMER2.0 (Gene_Corr) and GEPIA2 (Correlation Analysis)

Functional enrichment analyses — including Gene Ontology (BP, CC, MF) and pathway databases (KEGG, Reactome, WikiPathways) — were performed using **Enrichr**.

## Statistical Analysis

- Differential expression between tumor and normal tissues: **Wilcoxon rank-sum test** (TIMER2.0) or **Student's t-test / one-way ANOVA** (UALCAN)
- Correlation analyses: **Spearman's rank correlation coefficient**
- Two-sided **p < 0.05** considered statistically significant (with platform-specific multiple testing correction where applicable)
</arg_value>
<task_progress>
- [x] Extract title, author, and abstract
- [x] Create Abstracts/TMEM45A_Abstract.md
- [x] Create Methodology_Sections/TMEM45A_Methods.md
- [ ] Create Results_and_Discussions/TMEM45A_Results_and_Discussion.md
- [ ] Clean up Samples/ and commit/push
</task_progress>
</write_to_file>