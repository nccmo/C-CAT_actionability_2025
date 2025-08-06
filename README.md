# C-CAT_actionability_2025
"Real-world clinical utility of comprehensive genomic profiling in advanced solid tumors" by Y.Saito, et al.

## Directory Structure
This repository provides the main R scripts used in the study.

- **1_preparation/**
    - `01_report_data_organization.Rmd` - R markdown script to process and organize report data downloaded from C-CAT. 
    - `02_case_data_organization.Rmd` - R markdown script to process and organize case data downloaded from C-CAT. 
    - `03_patient_data.Rmd` - R markdown script to combine patient data into one file. 
    - `04_cancer_type.Rmd` - R markdown script to annotate tumor types.
    - `05_actionability_data.Rmd` - R markdown script to annotate clinical actionability.
    - `06_postEP_treatment_strategy_data.Rmd` - R markdown script to annotate post-CGP treatment strategies.
    - `07_prognosis.Rmd` - R markdown script to annotate prognosis.
    - `08_MSI_and_TMB.Rmd` - R markdown script to annotate MSI status and TMB levels.
    - `09_number_of_alterations.Rmd` -  R markdown script to annotate the number of genetic alterations by case.
    - `10_treatment.Rmd` - R markdown script to organize treatment data.
    - `11_ICI_annotation.Rmd` - R markdown script to annotate the use of ICIs for each case.
    - `12_TRK_annotation.Rmd` - R markdown script to annotate the use of TRK inhibitors for each case.
    - `13_double_cancer.Rmd` - R markdown script to annotate the presence of double cancers for each case.

- **2_analysis/**
  - **1_prognosis/**
    - `1_prognosis_by_evidence_level.Rmd` - R markdown script to evaluate prognosis by evidence level.
    - `2_prognosis_by_treatment_strategy.Rmd` - R markdown script to evaluate prognosis by treatment strategies.
    - `3_prognosis_by_prev_regimen_nums.Rmd` - R markdown script to evaluate prognosis by the number of previous regimens.

  - **2_treatment_overview/**
    - `1_actionable_alterations.Rmd` - R markdown script to evaluate actionable alterations.
    - `2_treatment_strategy.Rmd` - R markdown script to evaluate treatment strategies.
    - `3_treatment_strategy_by_cancer_type.Rmd` - R markdown script to evaluate treatment strategies in each tumor type.

  - **3_evidence_A/**
    - `1_count.Rmd` - R markdown script to count level A (approved) alterations.
    - `2_treatment.Rmd` - R markdown script to evaluate treatment in cases harboring level A (approved) alterations.
    - `3_treatment_by_cancer_type.Rmd` - R markdown script to evaluate treatment in cases harboring level A (approved) alterations, categorized by tumor type.
    - `4_CGP_utility.Rmd` - R markdown script to evaluate the fraction of cases estimated to benefit from CGP.
    - `5_CGP_utility_by_cancer_type.Rmd` - R markdown script to evaluate the fraction of cases estimated to benefit from CGP by tumor type.

  - **4_TMBH/**
    - `1_TMBH_TMBL_prognosis.Rmd` - R markdown script to evaluate prognosis by TMB status (TMB-H vs. TMB-L).
    - `2_TMBH_prognosis_by_TMB_levels.Rmd` - R markdown script to evaluate prognosis by TMB levels.
    - `3_TMBH_prognosis_by_MSI.Rmd` - R markdown script to evaluate prognosis by MSI.
    - `4_TMB_pembro_response1.Rmd` - R markdown script for evaluating response to pembrolizumab in TMB-H cases (part1).
    - `5_TMB_pembro_response2.Rmd` - R markdown script for evaluating response to pembrolizumab in TMB-H cases (part2).

  - **5_NTRK/**
    - `1_NTRK_fusion_treatment.Rmd` - R markdown script to evaluate treatment response in NTRK fusion-harboring cases.
    - `2_NTRK_cancer_type_distribution.Rmd` - R markdown script to evaluate the cancer type distribution of cases harboring NTRK fusions.
    - `3_NTRK_fusion_prognosis.Rmd` - R markdown script to evaluate prognosis by NTRK fusion status.
    - `4_NTRK_previous_studies.Rmd` - R markdown script to evaluate treatment response reported in published studies.

  - **6_companion/**
    - `analysis.Rmd` - R markdown script for analysis related to non-CGP CDx.

  - **7_tumor_type_specific_biomarker/**
    - `1_prognosis.Rmd` - R markdown script to evaluate prognosis by tumor type-specific biomarkers.
    - `2_response.Rmd` - R markdown script to evaluate response by tumor type-specific biomarkers.

## Data Availability
The data that support the findings of this study are available from C-CAT (URL: https://www.ncc.go.jp/en/c_cat/about) under controlled access due to ethical and privacy restrictions. Researchers can use the C-CAT data through “Research-Use Portal site”. To apply the use, researchers need to submit the C-CAT data use application form with a research protocol and a copy of the approval from their research ethics committee and the head of their institution to C-CAT (E-mail: c-cat_use@ml.res.ncc.go.jp), which is expected to respond within approximately one week. Please refer to “Steps from application to data utilization” (URL: https://www.ncc.go.jp/en/c_cat/use/flow/index.html) for details. The data access is currently restricted to hospitals for cancer genomic medicine, industries, and research institutes in Japan, but is expected to be extended to institutions outside Japan in the near future. In the meantime, researchers outside Japan can access the C-CAT data if they conduct a collaborative study with researchers based in Japan and approved by the C-CAT data utilization review board. The “Number-of-Records Search site” (URL: https://simplesearch-use.c-cat.ncc.go.jp/en/), which provides the number of the registered records of your interest in the C-CAT cohort, is publicly available.
