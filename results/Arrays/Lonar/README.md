# NumPy Arrays – Research Outputs

This directory contains the spatial and numerical array outputs generated during the computational analysis of Lonar Crater, India, and its comparison with Jezero Crater, Mars.

## Directory Structure

```text
Arrays/
└── Lonar/
    ├── README.md
    ├── Lonar_Best_Mineral_Map.npy
    ├── Lonar_Mineral_Candidate_Map_15deg.npy
    ├── Lonar_Minimum_SAM_Angle_Map.npy
    └── Lonar_Geological_Mask.npy
```

## Lonar Crater – Sentinel-2 Analysis

The `Lonar/` subdirectory contains four NumPy arrays generated during the Sentinel-2 spectral analysis and Spectral Angle Mapper (SAM) classification.

| File | Description |
|---|---|
| `Lonar_Best_Mineral_Map.npy` | Stores the best-matching reference mineral class assigned to each pixel. |
| `Lonar_Mineral_Candidate_Map_15deg.npy` | Stores candidate mineral classifications using a 15° SAM threshold. |
| `Lonar_Minimum_SAM_Angle_Map.npy` | Stores the minimum spectral angle calculated for each pixel. |
| `Lonar_Geological_Mask.npy` | Boolean mask identifying pixels selected for geological analysis. |

## Technical Specifications

- Data format: NumPy `.npy`
- Spatial dimensions: 357 × 369 pixels
- All four arrays share the same analysis grid.
- Generated using Python and NumPy.

## Scientific Significance

These arrays preserve the pixel-level outputs of the Lonar spectral classification workflow. They can be used for spatial visualization, classification assessment, statistical analysis, and further computational investigation.

The SAM outputs represent spectral similarities to selected reference-library spectra. They do not establish definitive mineral identities or actual mineral abundances.

## Reproducibility

The arrays were generated using the notebook:

`notebooks/Lonar_Sentinel2_Analysis.ipynb`

They can be loaded in Python using:

```python
import numpy as np

best_map = np.load("Lonar_Best_Mineral_Map.npy")
candidate_map = np.load("Lonar_Mineral_Candidate_Map_15deg.npy")
angle_map = np.load("Lonar_Minimum_SAM_Angle_Map.npy")
geological_mask = np.load("Lonar_Geological_Mask.npy")
```

## Future Scope

Further work may include spatial validation, improved spectral discrimination, geological interpretation, and comparison with independent mineralogical datasets.
