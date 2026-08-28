# Results and Discussion

## Results

### Expression Level of TMEM45A

TMEM45A exhibited significant cancer-type-specific dysregulation across TCGA cohorts compared to corresponding normal tissues:

**Downregulated in:** CHOL, KICH, LIHC, PRAD, THCA, and UCEC
**Upregulated in:** BRCA, GBM, HNSC, KIRC, and LUSC

- Expression was significantly higher in primary cutaneous melanoma than in metastatic SKCM lesions (TIMER2.0; Figure 2A)
- UALCAN validation confirmed these patterns (Figure 2B)
- **Pathological stage analysis** revealed significant associations with TMEM45A expression in **BRCA, KICH, KIRC, and LUSC** (GEPIA2; Figure 2C)
- No stage dependence observed in CHOL, HNSC, LIHC, SKCM, THCA, and UCEC (Supplementary Figure S1)
- Stage-wise evaluation omitted for GBM and PRAD due to incomplete clinical annotation

**Figure 2:** Pan-cancer transcriptome expression profile and pathological stage connection — TIMER2.0 (A), UALCAN (B), and GEPIA2 (C) analyses.

### Validation of TMEM45A Overexpression via GEPIA2 (TCGA-GTEx Integration)

Integrated TCGA-GTEx analysis in GEPIA2 confirmed cancer-type-specific dysregulation:

**Significantly elevated:** DLBC, GBM, HNSC, KIRC, LGG, LUSC, PAAD, and SARC (Figure 3A)
**Significantly decreased:** CHOL, KICH, LAML, LIHC, READ, SKCM, TGCT, THCA, and UCEC (Figure 3B)

No significant differences in remaining malignancies (Supplementary Figures S2A, S2B).

**Figure 3:** GEPIA2 validation of TMEM45A expression differences between TCGA tumor and GTEx normal tissues — up-regulated (A) and down-regulated (B) cohorts with sample sizes.

### Proteomic Analysis of TMEM45A

CPTAC proteomic datasets (via UALCAN), available for four TCGA cohorts:

- **Significantly higher TMEM45A protein abundance** in **BRCA, HNSC, and LIHC** versus normal tissues
- LUSC showed no significant difference (Supplementary Figure 3)

Immunohistochemical (IHC) profiling (HPA062101 antibody, Human Protein Atlas):

- **SKCM:** Strong cytoplasmic and nuclear immunoreactivity vs normal skin
- **THCA:** Moderate staining in malignant follicular cells; undetectable in normal thyroid
- **LIHC:** Positive staining in malignant hepatocyte cords

Proteomic and histological data broadly concurred with transcriptomic observations.

**Figure 4:** IHC tissue microarrays across 12 cancer types — BLCA, CESC, COAD, LIHC, OV, PAAD, READ, SKCM, STAD, TGCT, THCA, UCEC.

**Table 1:** IHC protein expression profile of TMEM45A across human cancers (HPA):

| Cancer | Staining (Level) | Intensity | Quantity | Location |
|--------|------------------|-----------|----------|----------|
| BLCA | Medium | Moderate | 75-25% | Cytoplasmic/membranous |
| CESC | High | Strong | 75-25% | Cytoplasmic/membranous nuclear |
| COAD | High | Strong | 75-25% | Cytoplasmic/membranous nuclear |
| LIHC | Low | Weak | 75-25% | Cytoplasmic/membranous nuclear |
| OV | High | Strong | 75-25% | Cytoplasmic/membranous nuclear |
| PAAD | High | Strong | 75-25% | Cytoplasmic/membranous nuclear |
| READ | Low | Moderate | <25% | Nuclear |
| SKCM | High | Strong | >75% | Cytoplasmic/membranous nuclear |
| STAD | High | Strong | 75-25% | Cytoplasmic/membranous nuclear |
| TGCT | Medium | Strong | <25% | Cytoplasmic/membranous |
| THCA | Medium | Moderate | 75-25% | Cytoplasmic/membranous |
| UCEC | Not detected | Weak | <25% | Nuclear |

*BLCA: Bladder UCC; CESC: Cervical SCC & Endocervical Adenocarcinoma; COAD: Colon Adenocarcinoma; LIHC: Liver HCC; OV: Ovarian Serous Cystadenocarcinoma; PAAD: Pancreatic Adenocarcinoma; READ: Rectum Adenocarcinoma; SKCM: Skin Cutaneous Melanoma; STAD: Stomach Adenocarcinoma; TGCT: Testicular GCT; THCA: Thyroid Carcinoma; UCEC: Uterine Corpus Endometrial Carcinoma.*

### Prognostic Value of TMEM45A in Human Cancers

- Elevated TMEM45A expression was associated with **unfavorable clinical outcomes** across multiple TCGA cohorts (Figures 5A, 5B)
- **Kaplan-Meier analyses** (significant for OS at p < 0.05):

**Overall Survival (OS)** significantly worse with high TMEM45A in:
- KIRC, KIRP, LIHC, STAD, and THCA

**Disease-Free Survival (DFS)** significantly shorter with high TMEM45A in:
- KIRC, OV, and STAD

- KIRC and STAD showed associations across both OS and DFS (Figure 5C, 5D)

**Figure 5:** Survival heatmaps and KM curves across 33 TCGA cancers.

### Methylation Analysis

#### SMART (Probe-level CpG Methylation)

- Widespread **TMEM45A promoter hypomethylation** across TCGA cohorts (Figure 6A)
- Significant hypomethylation at **N-shore probe cg07907506** in BRCA, CHOL, KIRC, LIHC, LUAD, LUSC, PRAD, and UCEC vs normal (Figure 6B; Supplementary Figure S4)
- Supported by CpG-aggregated promoter analysis (Figure 6C)

**Figure 6:** Chromosomal ideogram (A), N-shore probe cg07907506 box plots (B), and promoter methylation (C).

#### UALCAN (Promoter Methylation Validation)

Significant promoter hypomethylation (beta-values) in:
- BRCA, CESC, CHOL, KIRP, LUSC, PAAD, PCPG, PRAD, READ, THCA, and UCEC

No significant differences in: ESCA, GBM, HNSC, KIRC, LIHC, LUAD, SARC, STAD, THYM
No normal controls available for: ACC, DLBC, KICH, LAML, LGG, MESO, SKCM, TGCT, UCS, UVM

Cross-platform comparison (SMART vs UALCAN) confirmed concordant hypomethylation in **BRCA, CHOL, and UCEC**.

**Figure 7:** UALCAN promoter validation across TCGA cohorts — notable patterns in CHOL, KIRP, CESC, BRCA, LUSC, PAAD, PCPG, PRAD, THCA, UCEC, READ.

### Genetic Alteration Analysis of TMEM45A

- TMEM45A displayed **low yet cancer-type-specific genomic alteration frequencies**
- **Predominant alteration type:** copy-number amplification

**Highest alteration frequencies:**

| Cancer | Alteration Frequency |
|--------|---------------------|
| LUSC | ~8% |
| CESC | ~5.5% |
| ESCA | ~4.3% |
| HNSC | ~3.8% |
| UCEC | ~3.8% |
| OV | ~3.0% |
| SARC | ~2.4% |
| UCS | ~2.0% |

**Figure 8:** Mutational landscape and alteration frequency across TCGA cohorts.

#### Mutation Profiling

- Identified across the 275-amino-acid TMEM45A protein:
  - 44 missense, 7 truncating, 4 splice-site, 5 fusion events
  - Total: 60 variants
- **Mutation hotspot:** recurrent **V236I substitution** within the **DUF716 domain** (Figure 8B)
- Kaplan-Meier analyses across the eight top-altered cohorts: **no significant associations** between TMEM45A alterations and OS or PFS

### Univariate Cox Regression Analysis of TMEM45A

Significant associations with **poor overall survival** (HR > 1) in:

| Cancer | HR | 95% CI | P-value |
|--------|----|--------|---------|
| CHOL | 1.596 | 1.090–2.337 | 0.016 |
| KICH | 6.293 | 2.207–17.948 | 0.001 |
| KIRC | 1.146 | 1.033–1.270 | 0.010 |
| LGG | 1.432 | 1.113–1.843 | 0.005 |
| LIHC | 1.146 | 1.013–1.296 | 0.030 |
| LUAD | 1.164 | 1.030–1.317 | 0.015 |
| STAD | 1.221 | 1.007–1.482 | 0.042 |
| THCA | 5.749 | 2.555–12.936 | <0.001 |

**Figure 9:** Forest plot of HR, 95% CI, and log-rank p-values across 33 cancer types.

### Immune Infiltration Landscape of TMEM45A

TMEM189 correlated with immune cell infiltration, TMB, and MSI across TCGA cohorts (Figure 10).

**Figure 10:** Pan-cancer heatmaps and radar plots — immune infiltration (A), TMB (B), MSI (C).

#### EPIC Deconvolution (TIMER2.0)

- **Positive correlation:** cancer-associated fibroblasts (CAFs)
- **Negative correlation:** CD8+ T-cell infiltration (Figure 10A)
- NK-cell associations were heterogeneous

Significant T-cell associations in ACC, BLCA, BRCA, COAD, ESCA, HNSC, LIHC, LUAD, LUSC, MESO, PAAD, PCPG, PRAD, SARC, SKCM (primary/metastatic), TGCT, THYM.

#### TMB Associations (Pearson correlation)

- **Positive:** LAML, KICH, COAD, LGG
- **Negative:** HNSC

#### MSI Associations (Pearson correlation)

- **Positive:** MESO, COAD, LUAD, TGCT, LUSC
- **Negative:** CHOL, PRAD, HNSC, UCEC, UCS

### Immune Regulatory Landscape of TMEM45A

TMEM45A expression significantly associated with tumor immune microenvironment features across TCGA (Figure 11).

**Figure 11:** Immscore, infiltration, checkpoint, and immunoinhibitory heatmaps.

#### ESTIMATE Profiling

Predominantly positive correlations between TMEM45A and StromalScore, ImmuneScore, and ESTIMATEScore across: BLCA, BRCA, CESC, COAD, KIRC, KIRP, LIHC, LUAD, LUSC, PAAD, PCPG, PRAD, READ, STAD.

#### CIBERSORT Analysis (22 immune cell types)

- **Positive correlations:** macrophage subsets, neutrophils, resting memory T cells
- **Negative correlations:** T cells, regulatory T cells, T follicular helper cells, activated NK cells, plasma cells, memory B cells

> Indicating **myeloid enrichment** alongside **reduced lymphocyte infiltration**.

#### Immune Checkpoints & Immunoinhibitors

Widespread positive correlations with immune checkpoints (notably in BLCA, COAD, KICH, KIRP, LIHC, PAAD, PRAD, READ, THYM; ACC, BRCA, CESC, CHOL, ESCA, LAML, LUAD, STAD, UVM). TGCT exhibited inverse correlations.

Key immunoinhibitor correlations (most prominent in COAD, KICH, PRAD, READ): positive association; TGCT showed inverse trends.

### Immunostimulatory and Chemokine Signatures

TMEM45A associated with immunostimulatory molecules, chemokine signaling networks (Figure 12).

**Figure 12:** Immunostimulatory profiles (A), chemokine ligands (B), chemokine receptors (C), differential expression (D).

#### Co-expression Findings

- **Positive correlations** with immunostimulatory genes in GBM, HNSC, OV, SARC, UCEC
- **Inverse correlations** in KICH, KIRP, PRAD, TGCT
- **Chemokine ligands** positively correlated in LAML, LGG, UVM; negatively in PRAD, TGCT
- **Chemokine receptors** positively correlated in BRCA, HNSC, LUAD, STAD (notably CXCL12-CXCR4 axis)
- Differential expression reconfirmed TMEM45A **upregulation** across multiple tumor cohorts; **downregulation** in KICH and PRAD

### Single-Cell Transcriptomic Analysis of TMEM45A

Single-cell RNA sequencing (TISCH2) across 12 tumor microenvironments (BLCA, BRCA, HNSC, KIRC, LIHC, NSCLC, OV, PAAD, SARC, SKCM, STAD, UCEC):

- TMEM45A predominantly expressed in **malignant epithelial populations** in BRCA, NSCLC, STAD
- Further enriched in **stromal lineages** (fibroblasts, endothelial cells)
- Enriched in **myeloid compartments** (macrophages, monocytes)
- **Minimal detection** in T and B lymphoid populations

Single-cell patterns corroborated bulk transcriptomic deconvolution.

### Pharmacogenomic Associations of TMEM45A

Significant correlations with therapeutic sensitivity across GDSC and CTRP (Figure 13).

**Figure 13:** Drug sensitivity bubble plots (A, B), PPI network (C), Venn diagram (D), co-expression heatmap (E).

#### GDSC Findings

- **Positive correlations** (reduced sensitivity) with: BHG712, BMS345541, I-BET-762, LAQ824, Methotrexate, Navitoclax, NPK76-II-72-1, PHA-793887, TPCA-1, and **Vorinostat**
- **Inverse correlations** (increased sensitivity): **Docetaxel**, Bleomycin, ZSTK474

#### CTRP Findings

- Predominantly positive correlations with drug response
- Highly significant associations for: belinostat, ciclopirox, CR-1-31B, gemcitabine, panobinostat, sotrastaurin, and **vorinostat**

Cross-dataset concordance for **Vorinostat** consistently linked elevated TMEM45A to **reduced HDAC inhibitor sensitivity**.

### TMEM45A-Centered Protein-Protein Interaction Network

STRING analysis predicted a PPI network enriched for transmembrane and functionally associated proteins.

**Predicted interacting partners:**
- TMEM189 (highest combined interaction score)
- TMEM25, TMEM14A, TMEM9, TMEM30B, TMEM158, TMEM221, TMEM205
- APOA2, CETP, FTO, NDC1, IPPK, APMAP

### Integrated Network Analysis: TMEM189 as Functional Partner

- **TMEM189** identified as the sole convergent candidate across 151 evaluated targets
- Intersected 51 STRING interaction partners and 100 GEPIA2 co-expressed genes (Supplementary Table S4)
- Prioritized as the primary functional partner of TMEM45A

**Figure 13D:** Venn diagram of STRING 51 proteins vs GEPIA2 100 genes — only TMEM189 shared.

### Pan-Cancer Validation of TMEM45A-TMEM189 Co-expression

Pearson correlation confirmed a **predominantly positive co-expression pattern** between TMEM45A and TMEM189 across the majority of TCGA tumor cohorts (Figure 13E).

**Significant positive correlations** in:
- BRCA, CESC, CHOL, DLBC, ESCA, KICH, KIRC, KIRP, LGG, LIHC, LUAD, OV, PAAD, PCPG, THCA

**Inverse correlation** in: TGCT

### Functional Annotation of the TMEM45A-TMEM189-Associated Network

Enrichment analysis of the 150-gene network via Enrichr identified:

**Gene Ontology (GO):**
- **BP (Figure 14A):** skin barrier establishment, epidermis development, skin epidermis development, intermediate filament organization
- **CC (Figure 14B):** cornified envelope, desmosome, intermediate filament cytoskeleton, cell-cell junction
- **MF (Figure 14C):** wide-pore channel activity, calcium ion binding, gap junction channel activity, RAGE receptor binding

**Pathways:**
- **KEGG (Figure 14D):** IL-17 signaling, p53 signaling, arachidonic acid metabolism, cornified envelope formation
- **Reactome (Figure 14E):** cornified envelope formation, keratinization, metal sequestration by antimicrobial proteins, antimicrobial peptide pathways
- **WikiPathways (Figure 14F):** pancreatic cancer subtypes, hair follicle development, calcium regulation in cardiac cells, lipid particle composition

**Figure 14:** Pathway enrichment across GO, KEGG, Reactome, and WikiPathways.

---

## Discussion

### Pan-Cancer Oncogenic and Prognostic Landscape of TMEM45A

This study integrated transcriptomic, proteomic, epigenetic, immunological, pharmacogenomic, and single-cell analyses across 33 human malignancies to systematically characterize the oncogenic landscape of TMEM45A and its functional partner TMEM189.

**Key Findings:**

1. **TMEM45A overexpression** across aggressive malignancies (BRCA, DLBC, GBM, HNSC, KIRC, LGG, LUSC, PAAD, SARC) — validated at transcript (TIMER2.0/GEPIA2) and protein (CPTAC/HPA) levels
2. **Advanced pathological stage association** in BRCA, KICH, KIRC, LUSC
3. **Poor prognostic value** — high expression predicts shorter OS/DFS in KIRC, STAD, LIHC, THCA, OV, and pan-cancer-wide Cox significance across 8 cohorts
4. **Immune-excluded TME** — negative correlation with CD8+ T cells / NK cells, positive with CAFs and M2 macrophages
5. **Pharmacogenomic signature** — vorinostat resistance, docetaxel sensitivity
6. **TMEM189 partnership** — sole convergent partner across STRING PPI and GEPIA2 co-expression

### Epigenetic Regulation: Promoter DNA Hypomethylation

SMART probe-level analysis identified significant **hypomethylation at N-shore locus cg07907506** in BRCA, CHOL, KIRC, LIHC, LUAD, LUSC, PRAD, and UCEC, corroborated by UALCAN promoter analysis across 11 TCGA cancer types.

This indicates **promoter DNA hypomethylation as a key epigenetic driver** of TMEM45A transcriptional activation — consistent with the concept that N-shore epigenetic unmasking facilitates transcription factor access during carcinogenesis.

### Genomic Alterations and Clinical Outcomes

cBioPortal analysis revealed **copy-number amplification as the predominant genomic alteration** (~8% in LUSC, ~5.5% in CESC), with a recurrent **V236I missense mutation within the DUF716 domain**.

- Kaplan-Meier analyses showed **no significant associations** between TMEM45A genomic alterations and OS/PFS
- Suggests prognostic significance is driven by **epigenetically regulated transcriptional activation** rather than recurrent somatic genomic disruption
- Consistent with emerging concepts that transcriptional upregulation, rather than recurrent genomic disruption alone, contributes substantially to tumor progression

### Immune Microenvironment and Immunotherapy Contexture

Computational immunogenomic analyses linked TMEM45A to an **immunosuppressive TME**:

- Positive correlations with StromalScore, ImmuneScore, ESTIMATEScore
- CIBERSORT/EPIC: increased CAFs, M0/M1/M2 macrophages, neutrophils; depleted CD8+ T cells, NK cells, regulatory T cells, B cells, plasma cells
- Single-cell validation (TISCH2): TMEM45A enriched in malignant epithelial cells, fibroblasts, and myeloid lineages; minimal in lymphoid populations

> This defines an **immune-excluded phenotype** — extracellular matrix-rich, stromal-remodeled, with restricted lymphocyte infiltration.

- **Immune checkpoint correlations** (PDCD1, CTLA4, HAVCR2, and others)
- **TMB/MSI associations** in LAML, COAD, MESO (immunotherapy responsiveness candidates)

### Pharmacogenomics: HDAC Inhibitor Resistance & Taxane Sensitivity

Elevated TMEM45A expression was consistently associated with:

- **Reduced sensitivity to Vorinostat** (HDAC inhibitor) — across GDSC and CTRP datasets
- **Increased sensitivity to Docetaxel** (microtubule-stabilizing agent)

This aligns with evidence that transmembrane proteins influence microtubule dynamics and taxane sensitivity, suggesting **TMEM45A as a candidate pharmacogenomic marker** for therapeutic stratification.

### Strengths

1. **Integrative multi-omics design** spanning transcriptomic, proteomic, epigenetic, single-cell, immunological, and pharmacogenomic dimensions
2. **Single-cell + bulk integration** (TISCH2) — cell-type-specific TMEM45A expression across tumor, stromal, and myeloid compartments
3. **Orthogonal validation** — transcript (TIMER2.0/GEPIA2) + protein (CPTAC/IHC) + epigenetic (SMART/UALCAN)
4. **TMEM189 convergence** — sole overlapping gene across STRING (51 proteins) and GEPIA2 (100 genes) analyses
5. **Cross-dataset pharmacogenomics** — consistent GDSC/CTRP concordance for Vorinostat and Docetaxel

### Limitations

1. **Selection/batch bias** — exclusive reliance on public TCGA/GTEx datasets with heterogeneous acquisition and processing pipelines
2. **Scarcity of matched normal controls** in several cancer types limited comprehensive validation
3. **Unvalidated mechanistic basis** — TMEM45A-TMEM189 co-expression and associated pathways (p53, IL-17) remain experimentally unverified
4. **Computational-only study** — in vitro / in vivo experiments required to confirm roles in EMT, macrophage polarization, immune exclusion, and HDAC inhibitor resistance

---

## Conclusion

Integrative pan-cancer multi-omics analysis identified **TMEM45A** as significantly overexpressed across multiple high-incidence solid tumors, where elevated expression:

- Correlates with **advanced pathological stage** and **poorer OS/DFS**
- Is driven by **promoter DNA hypomethylation** (cg07907506)
- Associates with an **immune-excluded, myeloid-enriched TME**
- Predicts **docetaxel sensitivity** and **vorinostat resistance**

The **TMEM45A-TMEM189 axis**, validated by convergent STRING PPI and GEPIA2 co-expression analyses across TCGA cohorts, represents a **functional molecular target requiring in vitro and in vivo validation** to clarify its role in immune exclusion, therapeutic response, and tumor progression.
</arg_value>
<task_progress>
- [x] Extract title, author, and abstract
- [x] Create Abstracts/TMEM45A_Abstract.md
- [x] Create Methodology_Sections/TMEM45A_Methods.md
- [x] Create Results_and_Discussions/TMEM45A_Results_and_Discussion.md
- [ ] Clean up Samples/ and commit/push
</task_progress>
</write_to_file>