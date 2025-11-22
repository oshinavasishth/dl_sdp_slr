# Protocol for Systematic Mapping Study on Deep Learning–Based Software Defect Prediction
*(PRISMA-ScR–aligned)*

## 1. Background and Rationale
Deep learning (DL) has become a dominant approach in software defect prediction (SDP) owing to its capacity to learn complex code and metric representations.  
Despite rapid progress, the field is fragmented across datasets, representations, and architectures (e.g., CNNs, RNNs, GNNs, Transformers).  
A systematic mapping study is required to consolidate what has been explored, identify gaps, and provide a foundation for future research directions.

---

## 2. Objectives
This study aims to:
1. **Map and categorize** existing DL-based SDP research published between **January 2016 and October 2025**.  
2. **Identify trends** in architectures, representations, evaluation methods, and validation settings.  
3. **Summarize quantitative characteristics** (datasets, metrics, QA scores) without performing inferential meta-analysis.  
4. **Highlight gaps** for emerging topics such as explainable AI (XAI), LLMs, and cross-project generalization.

---

## 3. Review Type and Framework
- **Type:** Systematic Mapping Study (Scoping Review)  
- **Reporting Standard:** PRISMA-ScR (Tricco et al., 2018)  
- **Planning Framework:** Adapted from Kitchenham & Charters (2007)  
- **Outcome:** Descriptive synthesis and evidence map, *not* meta-analysis.

---

## 4. Research Questions (RQs)

| ID | Research Question | Motivation / Expected Output |
|----|-------------------|------------------------------|
| **RQ1** | What are the different DL techniques used in software defect prediction?  | Categorize architectures (CNN, RNN, LSTM, GAT, Transformer, Hybrid). |
| **RQ2** | What are the different source code representations for DL-based SDP models? | Identify input modalities (AST, CFG, metrics, text, hybrid). |
| **RQ3** | What are the key categories of hyperparameters commonly used in DL models? | Summarize hyperparameters (learning rate, batch size, optimizer, epochs, activation). |
| **RQ4** | What code-embedding techniques are used? | List pretrained models or custom embeddings (Word2Vec, CodeBERT, GraphCodeBERT). |
| **RQ5** | At what granularity level (e.g., file, function, line) are software defects predicted? | Map prediction granularity (file, class, method, line). |
| **RQ6** | What explainable AI (XAI) techniques are most applicable to DL-based SDP models | Identify interpretability methods (e.g., SHAP, LIME, attention visualization). |
| **RQ7** | How well do DL models work for defect prediction in within-version, cross-version, and cross-project cases | Summarize reported metrics (AUC, F1, MCC etc.) per validation scenario. |
| **RQ8** | What are the popular datasets used? | List and count datasets (NASA, PROMISE, GitHub, proprietary). |
| **RQ9** | What performance metrics are commonly used to evaluate results? | Frequency of metrics (Precision, Recall, F1, AUC, MCC, Accuracy). |
| **RQ10** | To what extent do SDP studies use statistical tests to validate their results | Identify validation tests (Wilcoxon, Scott–Knott ESD, Cliff's δ, t-test). |

---

## 5. Search Strategy

### 5.1 Information Sources
The following digital libraries are searched:
- ACM Digital Library  
- IEEE Xplore  
- ScienceDirect  
- SpringerLink  
- Wiley Online Library  
- Google Scholar (manual screening)

### 5.2 Time Window
- **January 2016 – October 2025**  
- Final search execution date: **25 October 2025**

### 5.3 Search Queries
Full Boolean search strings for all databases are provided in: search_strings.txt

Additional Search Methods - Incremental Primary studies from recent relevant surveys


## 6. Eligibility Criteria

### Inclusion Criteria
- Studies applying *deep learning* to software defect prediction  
- Peer-reviewed journal or conference papers  
- Published between 2016–2025  
- Written in English  
- Empirical evaluation with defect labels  

### Exclusion Criteria
- Non–deep learning approaches (E1)  
- Secondary studies (SLRs/SMS/surveys) (E2)  
- Irrelevant domain (E3)  
- Full text unavailable (E5)  
- Poor quality (QA score < 5) (E6)  
- Non-English (E7)  
- Preprint-only, non–peer-reviewed (E9)

## 7. Study Selection Process

### Stage 1: Title/Abstract Screening
- Two reviewers screened independently.  
- Disagreements documented in 'SDP_DL_Mapping_Study_Screening_Log.csv'.  
- Cohen’s κ = 0.90 (almost perfect agreement).

### Stage 2: Full-Text Screening
- Objective criteria applied (E5, E6).  
- No conflicts.  
- PRISMA flow diagram included in manuscript.

### Final Inclusion
- **167 primary studies** included.


---

## 8. Data-Extraction Variables (Charting Form)

Data items extracted (charting variables):

- Bibliographic details  
- Model family / architecture  
- Input representation (metrics, AST, CFG, PDG, tokens)  
- Code embedding approach (if applicable)  
- Granularity (file/function/line)  
- Dataset(s) used  
- Evaluation scenario (WV/CV/CPDP)  
- Metrics reported (Precision, Recall, F1, AUC, MCC…)  
- Hyperparameters and optimization approach  
- XAI techniques  
- Statistical tests used 

This table constitutes the data_extraction_sheet.xlsx for all included studies.

## 9. Quality Assessment

### QA Instrument
A 9-item Kitchenham-based checklist assessing:
- clarity of objectives  
- dataset description  
- model description  
- baseline comparison  
- hyperparameter reporting  
- experimental setup  
- statistical validity  
- result interpretation  
- reproducibility

### Scoring
- 0 / 0.5 / 1 per item  
- Maximum score: 9  
- Cutoff: studies scoring **< 5** excluded

QA results provided in: qa_assessment.csv

## 10. Synthesis Method

- **No meta-analysis** performed.  
- **Descriptive synthesis** only.  
- Medians and interquartile ranges (IQRs) used for performance metrics.  
- Trends plotted annually.  
- Evidence grouped thematically per RQ.  
- Statistical tests used in primary studies counted and summarized.  

This approach aligns with PRISMA-ScR item on descriptive synthesis.

## 11. Outputs and Reproducibility Artifacts

- PRISMA-ScR checklist  
- PRISMA flow diagram  
- Screening log  
- Extraction sheet  
- QA scores  
- Full list of 167 included primary studies  
- Replication instructions in `README.md`

---
