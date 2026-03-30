# Recoding Rules

## Behavior variable
- Raw variable: `EverCigaretteUse`
- Assignment benchmark: `p0 = 0.50`
- Recoding used in this project:
  - raw code 1 -> success (1)
  - raw code 2 -> failure (0)
  - anything else / missing -> NA

## Continuous variable
- Raw variable: `HowMuchDoYouWeighWithoutShoesInKG`
- Assignment benchmark: `mu0 = 68.0`
- Cleaning used in this project:
  - keep positive numeric values
  - drop missing values
