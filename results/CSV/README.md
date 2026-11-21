# CSV Results – Lonar–Jezero Comparative Study

This directory contains the CSV datasets generated during the computational spectral and mineral-candidate analysis of Lonar Crater, India, and Jezero Crater, Mars.

## 1. Integrated Project Results

| File | Description |
|---|---|
| `Integrated_Project_Summary.csv` | Consolidated summary of the integrated investigation |
| `Lonar_Jezero_Comparative_Spectra.csv` | Comparative normalized spectral data for Lonar and three Jezero ROIs |

## 2. Lonar Crater – Sentinel-2 Analysis

Location: `Lonar/`

| File | Description |
|---|---|
| `Lonar_Median_Spectrum.csv` | Median reflectance spectrum across nine Sentinel-2 bands |
| `SAM_Threshold_Comparison.csv` | Comparison of SAM classification at different angular thresholds |
| `SAM_Quality_Statistics.csv` | Spectral angle distribution and classification quality statistics |
| `Mineral_Candidate_Distribution.csv` | Distribution of candidate mineral spectral matches |

## 3. Jezero Crater – CRISM Analysis

Location: `Jezero/`

| File | Description |
|---|---|
| `Jezero_Equal_Band_Validation.csv` | Equal-band validation of selected spectral reference matches |
| `Jezero_Mineral_Class_Statistics.csv` | Candidate mineral classification statistics |
| `Jezero_ROI_SAM_Results.csv` | SAM results for three selected regions of interest |
| `Jezero_SAM_Similarity_Matrix.csv` | Spectral similarity matrix across ROIs and reference spectra |

## 4. Data Processing

The CSV outputs were generated through two independent analytical workflows:

- **Lonar:** Sentinel-2 Level-2A surface reflectance preprocessing, geological candidate masking, spectral library matching, and Spectral Angle Mapper (SAM) analysis.
- **Jezero:** Mars Reconnaissance Orbiter (MRO) Compact Reconnaissance Imaging Spectrometer for Mars (CRISM) MTRDR processing, ROI-based spectral extraction, reference-library comparison, and constrained candidate classification.

## 5. Scientific Interpretation

The mineral classes represent candidate spectral matches, not confirmed mineral identifications or measured mineral abundances.

The Lonar–Jezero comparison uses normalized spectral shapes. It is exploratory and does not represent calibrated cross-sensor equivalence.

These results do not establish the presence of biosignatures or evidence of extraterrestrial life.

## 6. Reproducibility

The complete analytical workflows are available in:

- `notebooks/Lonar_Sentinel2_Analysis.ipynb`
- `notebooks/Jezero_CRISM_Analysis.ipynb`

See the individual subdirectory README files for further details.
