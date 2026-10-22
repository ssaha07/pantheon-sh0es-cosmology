# Measuring Cosmological Parameters Using Type Ia Supernovae

Python-based analysis of the Pantheon+SH0ES Type Ia supernova dataset to investigate the expansion history of the Universe, estimate the Hubble constant, and calculate the cosmic age under an explicitly stated cosmological model.

## Objectives
- Load and inspect the Pantheon+SH0ES observational data.
- Plot the Hubble diagram (distance modulus against redshift).
- Fit the selected cosmological model and estimate the Hubble constant and matter-density parameter where applicable.
- Estimate the age of the Universe under the model assumptions.
- Examine residuals for trends or outliers.
- Compare analyses with a fixed matter-density parameter and, where implemented, low-redshift and high-redshift subsamples.

## Data
The dataset is not bundled with this repository. Obtain the appropriate release from the [PantheonPlusSH0ES DataRelease repository](https://github.com/PantheonPlusSH0ES/DataRelease), review its data-use notes, and place the required file in `data/`. Document the exact filename and columns used by the notebook. Do not commit large files or data that you are not permitted to redistribute.

The project report identifies columns including `zHD`, `MU_SH0ES`, and `MU_SH0ES_ERR_DIAG`; confirm these against the exact file downloaded before running the analysis.

## Repository layout
```text
data/       # Local input data; see data/README.md
notebooks/  # Analysis notebook(s)
figures/    # Exported plots
results/    # Summary results and tables
requirements.txt
```

## Setup
Python 3.10 or later is recommended. Create and activate a virtual environment, then install dependencies:

```bash
python -m venv .venv
# Windows PowerShell: .venv\Scripts\Activate.ps1
# macOS/Linux: source .venv/bin/activate
python -m pip install -r requirements.txt
```

Launch the notebook using Jupyter Lab or Jupyter Notebook. Update the local data path if needed.

## Reported result
The submitted project report records a Hubble constant of approximately `73.53 ± 0.17 km/s/Mpc` for the stated analysis with matter-density parameter `Ωm = 0.3`, and an estimated Universe age of approximately `12.82 Gyr`. Re-run the final notebook to verify the results, uncertainty calculation, assumptions, and units before presenting them as reproduced outputs.

## Model and interpretation
The estimated parameters depend on the cosmological model, calibration, data selection, and fitting procedure. Residual plots and comparisons between subsamples should be interpreted as diagnostic checks, not by themselves as proof of a particular cosmological explanation.

## References
- Pantheon+SH0ES Data Release: https://github.com/PantheonPlusSH0ES/DataRelease
- NumPy: https://numpy.org/doc/
- pandas: https://pandas.pydata.org/docs/
- Matplotlib: https://matplotlib.org/stable/
- SciPy: https://docs.scipy.org/doc/scipy/
- Astropy: https://docs.astropy.org/

## Author
Name: Shamayita Saha
