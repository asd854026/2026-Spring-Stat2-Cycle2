# Project Cycle 2

## Group Information
- Group number: 09
- Member names: 112370216 蘇榮盛, 109370231 謝宇家, 113370220 游子涵

## Dataset
- Raw data: `YRBS_2007.csv`
- Processed data used across notebooks: `yrbs_combined_processed.csv`

## Selected formal variables
- **Behavior variable (proportion analysis):** `SadOrHopeless`
  - benchmark proportion: `p0 = 0.30`
- **Continuous variable (mean analysis):** `HowMuchDoYouWeighWithoutShoesInKG`
  - benchmark mean: `mu0 = 68.0`

## Exploratory EDA variables
- `CurrentCigaretteUse`
- `HowOldAreYou`

## Project questions

### Formal questions
1. Is the proportion of students who reported feeling **SadOrHopeless** different from **0.30**?
2. Is the mean body weight of students different from **68.0 kg**?

### Additional exploratory questions
1. Is **SadOrHopeless** more common among students who reported smoking on at least 1 day in the past 30 days, and does this association vary across age groups?
2. Among current smokers, does smoking frequency appear to differ by **SadOrHopeless** status?

## Notebook structure
- `01_data.ipynb`  
  Variable definitions, data checks, recoding rules, and final valid sample sizes.

- `02_BehaviorVariable_eda.ipynb`  
  Formal EDA for `SadOrHopeless`.

- `02_ContinueVariable_eda.ipynb`  
  Formal EDA for `HowMuchDoYouWeighWithoutShoesInKG`.

- `02_Additional_eda.ipynb`  
  Exploratory EDA relating `SadOrHopeless` to smoking status, age group, and smoking frequency.

- `03_BehaviorVariable_inference.ipynb`  
  One-sample inference for the population proportion of `SadOrHopeless`.

- `03_ContinueVariable_inference.ipynb`  
  One-sample inference for the population mean of body weight.

- `04_interpretation.ipynb`  
  Summary table of main inferential results and final synthesis.

## Short final conclusion

The formal proportion analysis found that the estimated proportion of `SadOrHopeless` is essentially equal to the benchmark of `0.30`, so the null hypothesis was **not rejected** at the 5% level.  

The formal mean analysis found that the sample mean body weight is slightly above `68.0 kg`, so the null hypothesis was **rejected** at the 5% level.  

The additional exploratory EDA suggests that `SadOrHopeless` tends to be more common among current smokers than among non-smokers across age groups, and that smoking-frequency patterns among current smokers may also differ somewhat by `SadOrHopeless` status.
