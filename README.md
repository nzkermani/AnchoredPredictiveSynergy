# Anchored Predictive Synergy

Reproducible analysis code for the **Anchored Predictive Synergy (APS)** manuscript.

## What is included

`AnchoredSynergy_analysis.ipynb` contains the analysis pipeline used to estimate predictive interaction between a prespecified anchor and one molecular extension at a time. It implements the four factorial prediction states, repeated cross-validation, subject-level out-of-fold probability storage, negative cross-entropy APS estimation, bootstrap uncertainty, multiplicity-adjusted summaries, sensitivity analyses, and the final exploratory drugomics heterogeneity analyses and figures.

## What is not included

U-BIOPRED participant-level data are not distributed here. The notebook expects locally available, authorised source data. Do not upload participant identifiers, governed cohort data, or derived files that could compromise cohort data-use agreements.

## Local configuration

Set:

```bash
export APS_DATA_DIR=/path/to/ubiopred/Dataset/G2/VersionTwo/data
export APS_RESULT_DIR=/path/to/results/FINAL_S1_30x5
```

Then launch Jupyter and run the notebook.

## Reproducibility recommendation

Before manuscript submission or public release:

1. create a clean Python environment;
2. install the versions used for the final analysis;
3. run the notebook from top to bottom against the authorised data;
4. confirm that the manuscript tables, confidence intervals, q-values and figures are reproduced;
5. tag the exact submitted version of the code.

The release notebook has had stored outputs removed. This avoids publishing participant-level or machine-specific output accidentally and makes the repository diff easier to review.

## Repository structure

```text
.
├── AnchoredSynergy_analysis.ipynb
├── README.md
├── requirements.txt
├── .gitignore
└── REPRODUCIBILITY_CHECKLIST.md
```

## Archiving

For the manuscript, use GitHub for the living code repository and archive the exact submitted release in Zenodo to obtain a persistent DOI. Add the DOI to the manuscript's Code Availability statement after the release has been archived.

## Licence

Choose a software licence only after confirming that it is compatible with the IntegrAO dependency and your institutional/cohort requirements. No licence is asserted by this preparation package.
