# Systematic Mapping Study: Deep Learning–Based Software Defect Prediction (2016–2025)

This repository contains the transparency and reproducibility materials for the systematic mapping study on deep learning approaches for software defect prediction (SDP). The review follows the PRISMA-ScR guidelines and applies a Kitchenham-style quality assessment to ensure methodological clarity.

---

## Files Included in This Repository

The following files correspond to the search, screening, quality assessment, and data extraction stages described in the manuscript.

### Search and Retrieval Files
- ACM_2016-2025.csv  
- IEEE_final_2016-2025.csv  
- ScienceDirect_final_2016-2025.csv  
- Wiley_2016-2025.csv  
- GoogleScholar_2016-2025.csv  
- search_strings.txt (full Boolean search queries)  
- search_log.csv (counts of retrieved records per source)

### Screening Materials
- SDP_DL_Mapping_Study_Screening_Log.csv  
  Contains deduplication information, Stage 1 and Stage 2 screening decisions, conflicts, exclusion reasons, and the final list of included studies.

### Quality Assessment
- qa_assessment.csv  
  Contains Kitchenham-based quality scores for all screened studies, including exclusion by QA < 5.

### Data Extraction
- data_extraction_sheet.xlsx  
  Contains all extracted variables for included studies, including model type, input representation, dataset, granularity, evaluation scenario, metrics, hyperparameter details, imbalance handling, XAI techniques, and statistical test usage.

### PRISMA Documentation
- Prisma_flow_diagram.pdf  
- PRISMA-ScR-Fillable-Checklist-1.docx (completed checklist)

---

## Replication Notes

To replicate the review process:

1. Review search queries in `search_strings.txt`.  
2. Verify retrieved records using the database export files (`*_2016-2025.csv`).  
3. Examine deduplication and screening decisions in `SDP_DL_Mapping_Study_Screening_Log.csv`.  
4. Confirm QA decisions using `qa_assessment.csv`.  
5. Inspect the extracted data in `data_extraction_sheet.xlsx`.  
6. Refer to `Prisma_flow_diagram.pdf` and the PRISMA checklist for transparency of the screening process.

This repository provides all artifacts required for PRISMA-ScR–aligned transparency and reproducibility.

---

## Contact

Maintainer: Oshina Vasishth  
GitHub: https://github.com/oshinavasishth
