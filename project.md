# Project: Prediction Model for Progression-Free Survival in Breast Cancer Patients

## Background

Progression-free survival (PFS) is defined as the time from disease diagnosis to the first occurrence of disease progression or death from any cause, whichever comes first. PFS is a key clinical endpoint in breast cancer research.

Researcher A designed a study to build a prediction model for PFS in breast cancer patients. The study enrolled 2000 patients diagnosed with breast cancer between 1990 and 1995. All patients were followed until disease progression or death, with complete follow-up for every patient (i.e., PFS was observed for all participants). The log-transformed PFS (in months) is the primary outcome of interest. Researcher A collected data on patient demographics and clinical characteristics at the time of diagnosis, as well as the initial treatment received. The data are stored in `datA.RData`. Here is a description of the dataset:

| Variable Name                  | Column Name      | Description |
|--------------------------------|------------------|-------------|
| ID                             | id               | Patient ID |
| Age                            | age              | Age at diagnosis (in years) |
| Menopausal status              | menopause        | Menopausal status at diagnosis; 0 = Pre-menopausal, 1 = Post-menopausal |
| Race/ethnicity                 | race             | 1 = White, 2 = Black, 3 = Asian, 4 = Hispanic |
| BMI                            | bmi              | Body Mass Index at diagnosis (kg/m²) |
| Tumor size                     | tumor_size       | Tumor size at diagnosis (in centimeters) |
| Tumor grade                    | tumor_grade      | Tumor grade at diagnosis; 1 = Well differentiated, 2 = Moderately differentiated, 3 = Poorly differentiated |
| Number of positive lymph nodes | lymph_nodes      | Number of positive axillary lymph nodes at diagnosis |
| Estrogen receptor status       | ER               | ER status at diagnosis; 0 = Negative, 1 = Positive |
| Progesterone receptor status   | PR               | PR status at diagnosis; 0 = Negative, 1 = Positive |
| HER2 status                    | HER2             | HER2 status at diagnosis; 0 = Negative, 1 = Positive |
| Ki-67 index                    | Ki67             | Ki-67 proliferation index at diagnosis (%) |
| Clinical stage                 | stage            | Clinical stage at diagnosis; 1 = Stage I, 2 = Stage II, 3 = Stage III |
| Surgery type                   | surgery          | Initial surgery received; 0 = Breast-conserving surgery, 1 = Mastectomy |
| Chemotherapy                   | chemo            | Initial chemotherapy received; 0 = No, 1 = Yes |
| Hormonal therapy               | hormonal_therapy | Initial hormonal therapy received; 0 = No, 1 = Yes |
| Log-transformed PFS            | log_PFS          | Log-transformed progression-free survival time (months); Response variable |

## Questions

### (I) Using this dataset, please help Researcher A build a prediction model for PFS, aiming to understand how demographic, tumor, and treatment characteristics influence progression-free survival in breast cancer patients.

`datA.RData` [Download datA.RData](datA.RData)

To answer this question, your report should at least include the following:

- **Model Training:** Provide a detailed description of the model training procedure and how you obtained the model. Your description should include sufficient detail so that another statistician can reproduce the same model. Points will be deducted if the details provided are insufficient to reproduce your results.
- **Results:** Report the model. Interpret the model and assess its performance.

### (II) About a decade later, Researcher B conducted a separate study enrolling 2000 breast cancer patients diagnosed between 2000 and 2005, using the same study design and variable definitions. Like Researcher A's study, all patients were followed until disease progression or death. Researcher B's data are stored in `datB.RData`. Researcher A would like to evaluate whether the prediction model built on the original data generalizes well to Researcher B's dataset. Does the model generalize well? If yes, provide justification. If not, build a new prediction model for the 2000–2005 cohort and discuss what has changed in prediction.

`datB.RData` [Download datB.RData](datB.RData)

## Report Requirements

Please complete a report that helps Researcher A answer the above questions.

### Formatting

- **Font:** Times New Roman, 12 pt.
- **Line spacing:** 1.5.
- **Page limit:** The main text of your report should not exceed 5 pages. This limit applies to the text only; figures and tables do not count toward the page limit.
- **Figures and tables:** All figures and tables should be placed in an Appendix at the end of the report, after the main text. Each figure and table must have a clear caption. Reference all figures and tables in the main text by their labels (e.g., "see Figure 1," "as shown in Table 2").
- **No R code in the report.** Avoid inserting raw outputs from R functions; instead, demonstrate your ability to interpret and distill useful information from output tables.
- Points will be deducted if the formatting requirements above are not followed.

### Submission

Your submission should include two components:

- **Analysis Report (PDF):** Follow the formatting requirements above.
- **R code and outputs (Rmd + knitted file):** Your submission should contain all the code for conducting your analysis, as well as for the creation of any tables/figures/numbers presented in your report.
- Due to submission restrictions, one team member will submit all the files for the entire team. Please coordinate within your team to decide who will be responsible for this task.
