# Wind energy and time-series modeling

## Notebook

- [Generacion ARMA.ipynb](Generacion%20ARMA.ipynb) — The notebook reads manually uploaded ZIP archives of hourly wind-generation spreadsheets, fits an ARMA(2,2) model via statsmodels, diagnoses residuals, and simulates future scenarios. The last two code cells switch to unrelated football passing data and are retained as part of the original notebook.

## Method and scope

This description summarizes the notebook's stated model and code structure. Saved figures and numerical output are historical results from the original Colab file; they were preserved but not independently rerun or scientifically verified in this migration.

## Related material

The [source inventory](../../docs/SOURCE_INVENTORY.md) lists the complete archive.

## Environment

Install `requirements/wind-energy-and-time-series-modeling.txt` from the repository root. Consult [reproducibility notes](../../docs/REPRODUCIBILITY.md) for source data, solvers, and runtime limitations. Package versions are not pinned because a verified original environment lockfile is unavailable.
