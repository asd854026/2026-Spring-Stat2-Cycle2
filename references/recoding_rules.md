# Recoding Rules

## Formal behavior variable

- **Raw variable:** `SadOrHopeless`
- **Assignment benchmark:** `p0 = 0.30`
- **Recoding used in this project:**
  - raw code `1` -> `sad_binary = 1`
  - raw code `2` -> `sad_binary = 0`
  - anything else or missing -> `NA`

## Formal continuous variable

- **Raw variable:** `HowMuchDoYouWeighWithoutShoesInKG`
- **Assignment benchmark:** `mu0 = 68.0`
- **Cleaning used in this project:**
  - convert entries to numeric where possible
  - keep positive numeric values only
  - treat missing, invalid non-numeric, or non-positive values as `NA`

## Exploratory EDA variables

### Smoking status used in the additional EDA
- **Raw variable:** `CurrentCigaretteUse`
- **Recoding used in this project:**
  - raw code `1` -> `smoker_binary = 0`
  - raw codes `2` to `7` -> `smoker_binary = 1`
  - anything else or missing -> `NA`

### Smoking-frequency grouping used among current smokers
- raw codes `2`, `3` -> `Light (1~5 days)`
- raw codes `4`, `5` -> `Moderate (6~19 days)`
- raw codes `6`, `7` -> `Frequent (20~30 days)`

### Age grouping used in the additional EDA
- **Raw variable:** `HowOldAreYou`
- raw codes `1`, `2`, `3` -> `<=14`
- raw code `4` -> `15`
- raw code `5` -> `16`
- raw code `6` -> `17`
- raw code `7` -> `18+`
- missing or invalid values -> `NA`
