# Architecture

Exploratory data analysis of solar irradiance datasets from Benin, Sierra Leone, and Togo, organized as notebooks with reusable helpers and CI.

## Layout

| Path | Role |
| ---- | ---- |
| `notebooks/benin_eda.ipynb`, `sierraleone_eda.ipynb`, `togo_eda.ipynb` | Per-country profiling, cleaning (outliers, missing values), and EDA |
| `notebooks/compare_countries.ipynb` | Cross-country comparison of GHI/DNI/DHI and related variables |
| `scripts/` | Shared loading/cleaning helpers importable from notebooks |
| `tests/` | pytest suite for the helpers |
| `.github/workflows/ci.yml` | Installs requirements and runs tests |

## Data

Raw CSVs are not committed. Place them under `data/` (gitignored) using the file names referenced at the top of each notebook.
