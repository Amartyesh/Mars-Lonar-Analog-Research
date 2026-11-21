# Scientific Figures – Lonar–Jezero Comparative Study

This directory contains visual outputs generated during the multispectral and mineral-candidate analysis of Lonar Crater, India, and Jezero Crater, Mars.

## Directory Structure

```text
Figures/
├── README.md
├── Lonar/
│   └── README.md
└── Jezero/
    └── README.md
```

## 1. Lonar Crater – Sentinel-2 Figures

The `Lonar/` directory is intended to contain visual outputs from Sentinel-2 Level-2A analysis, including:

- Sentinel-2 multispectral and false-colour visualisations.
- Geological candidate mask.
- SAM mineral-candidate classification maps.
- Spectral reflectance plots.
- SAM threshold and classification quality plots.

## 2. Jezero Crater – CRISM Figures

The `Jezero/` directory contains visual outputs from Mars Reconnaissance Orbiter (MRO) CRISM analysis, including:

- CRISM false-colour visualisations.
- ROI spectral comparison plots.
- SAM spectral similarity visualisations.
- Candidate mineral classification maps.
- Lonar–Jezero comparative spectral plots.

## Scientific Interpretation

These figures represent exploratory remote-sensing and spectral-analysis outputs. Candidate mineral classifications indicate spectral similarity to reference spectra and should not be interpreted as definitive mineral identification, mineral abundance, or evidence of biological activity.

## Reproducibility

The figures were generated using the analytical workflows documented in:

- `notebooks/Lonar_Sentinel2_Analysis.ipynb`
- `notebooks/Jezero_CRISM_Analysis.ipynb`

Refer to the individual subdirectory README files for figure-specific descriptions.
