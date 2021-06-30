# Detection_of_cfmDNA

This repository contains data files and R code used for the analyses presented in the study:

**Detection of cell-free microbial DNA using a contaminant-controlled analysis framework**

Zozaya-Valdés E, Wong SQ, Raleigh J, Hatzimihalis A, Ftouni S, Papenfuss AT, Sandhu S, Dawson MA, Dawson SJ.

**Abstract**

Background: The human microbiome plays an important role in cancer.
Accumulating evidence indicates that commensal microbiome-derived DNA may be
represented in minute quantities in the cell-free DNA of human blood and could
possibly be harnessed as a new cancer biomarker. However, there has been limited
use of rigorous experimental controls to account for contamination, which invariably
affects low-biomass microbiome studies.

Results: We apply a combination of 16S-rRNA-gene sequencing and droplet digital
PCR to determine if the specific detection of cell-free microbial DNA (cfmDNA) is
possible in metastatic melanoma patients. Compared to matched stool and saliva
samples, the absolute concentration of cfmDNA is low but significantly above the
levels detected from negative controls. The microbial community of plasma is
strongly influenced by laboratory and reagent contaminants introduced during the
DNA extraction and sequencing processes. Through the application of an in silico
decontamination strategy including the filtering of amplicon sequence variants
(ASVs) with batch dependent abundances and those with a higher prevalence in
negative controls, we identify known gut commensal bacteria, such as
Faecalibacterium, Bacteroides and Ruminococcus, and also other uncharacterised ASVs.
We analyse additional plasma samples, highlighting the potential of this framework
to identify differences in cfmDNA between healthy and cancer patients.

Conclusions: Together, these observations indicate that plasma can harbour a low
yet detectable level of cfmDNA. The results highlight the importance of accounting
for contamination and provide an analytical decontamination framework to allow
the accurate detection of cfmDNA for future biomarker studies in cancer and other
diseases.

## R scripts

The main analyses of this study were performed across four R markdown scripts organized in the following way:

* Group 1 and 2 samples (see paper Figure 1)
  + Diversity analysis
    - Input data: Group_1_and_2.data.RData 
    - Analysis script: Group_1_and_2.diversity_analysis.Rmd
    - Output data: Group_1_and_2.OTU_tables.RData
  + Decontamination analysis
    - Input data: Group_1_and_2.OTU_tables.RData
    - Analysis script: Group_1_and_2.decontamination.Rmd

* Group 3 samples (see paper Figure 1)
  + Diversity analysis
    - Input data: Group3.data.RData 
    - Analysis script: Group3.div_analysis.v2.GB1.Rmd 
    - Output data: Group3.div_analysis.v2.GB1.OTU_tables.Rdata
  + Decontamination analysis
    - Input data: Group3.div_analysis.v2.GB1.OTU_tables.Rdata
    - Analysis script: Group3.decontamination.Rmd
