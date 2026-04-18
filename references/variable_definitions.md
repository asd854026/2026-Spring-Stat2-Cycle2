# Variable Definitions

## Selected behavior variable

- **Variable name:** `SadOrHopeless`
- **What the variable measures:** whether the student felt so sad or hopeless almost every day for 2 weeks or more in a row during the past 12 months that they stopped doing some usual activities.
- **Valid codes used:**
  - `1` = Yes
  - `2` = No
- **Recoding used in this project:**
  - `1` -> `sad_binary = 1`
  - `2` -> `sad_binary = 0`
- **How missing or invalid values are handled:** removed from the formal proportion analysis.
- **Final valid sample size for behavior analysis:** 13845

## Selected continuous variable

- **Variable name:** `HowMuchDoYouWeighWithoutShoesInKG`
- **What the variable measures:** body weight without shoes in kilograms.
- **Valid values used:** positive numeric values only.
- **How missing or invalid values are handled:** non-numeric, missing, or non-positive values are removed from the formal mean analysis.
- **Final valid sample size for mean analysis:** 13062

## Additional EDA variables

### CurrentCigaretteUse
- **What the variable measures:** number of days the student smoked cigarettes during the past 30 days.
- **Valid codes used:**
  - `1` = 0 days
  - `2` = 1 or 2 days
  - `3` = 3 to 5 days
  - `4` = 6 to 9 days
  - `5` = 10 to 19 days
  - `6` = 20 to 29 days
  - `7` = all 30 days
- **Recoding used in the exploratory EDA:**
  - `1` -> `smoker_binary = 0` (non-smoker)
  - `2` to `7` -> `smoker_binary = 1` (current smoker)
  - grouped version for exploratory smoking frequency:
    - `2`, `3` -> `Light (1~5 days)`
    - `4`, `5` -> `Moderate (6~19 days)`
    - `6`, `7` -> `Frequent (20~30 days)`

### HowOldAreYou
- **What the variable measures:** age category of the student.
- **Valid codes used:**
  - `1` = 12 years old or younger
  - `2` = 13 years old
  - `3` = 14 years old
  - `4` = 15 years old
  - `5` = 16 years old
  - `6` = 17 years old
  - `7` = 18 years old or older
- **Grouping used in the exploratory EDA:**
  - `1`, `2`, `3` -> `<=14`
  - `4` -> `15`
  - `5` -> `16`
  - `6` -> `17`
  - `7` -> `18+`
- **Why the grouped version is used:** the counts for codes `1` and `2` are very small, so the grouped version provides more stable and interpretable subgroup comparisons.

## Final exploratory-analysis sample size

- **Rows kept for the exploratory smoking-age-sad EDA:** 13120
- **Rule used:** keep only rows with valid values for `sad_binary`, `smoker_binary`, and `age_group`.
