# Reproducibility and access notes

## Preservation

All 16 Google Colab notebooks were downloaded as raw `.ipynb` files and copied without modification. The Drive folder was not edited. SHA-256 digests and file sizes are recorded in `provenance.csv`; run `sha256sum -c docs/SHA256SUMS` from the repository root to check the local copies. Two source IDs point to byte-identical copies of the evolutionary-finance notebook.

## Environment

The notebook sources do not provide a complete lockfile, Python version, or consistent package versions. Requirements files list observed Python imports and installation commands, without asserting tested compatibility. `Codigo JULIO AI.ipynb` needs Pyomo, an external `pyomo-test.py` upload, and the GLPK system solver (`glpk-utils` in its Colab commands). `Working-code.ipynb` uses Pyomo and HiGHS through `highspy`. Chance-constrained notebooks use SciPy and, in some cases, CVXPY with installed solvers (including CLARABEL in the extended lot-sizing notebook).

## Data and external services

- `Generacion ARMA.ipynb` expects manually uploaded ZIP files containing wind-generation Excel workbooks, uses the Colab `/content` directory, and writes scenario CSV files. Those input archives were not in the supplied folder. Its final two code cells concern StatsBomb football data rather than wind modeling.
- `Codigo JULIO AI.ipynb` expects a manually uploaded `pyomo-test.py` file, which was not in the supplied folder. It modifies that uploaded file at runtime.
- `ProyectoAplica.ipynb` reads a customer-churn CSV from an external GitHub raw URL; availability and licensing were not verified.
- `Analisis_Defensivo_Flick_CVaR_LaLiga.ipynb` requests Understat and FBref pages. Network access and source terms may affect reruns.
- `Numerical Experiment 6.1 Production Planning.ipynb` writes `risk_envelope.csv`; that derived CSV is not a separately supplied source file.

## Review status

A static scan of notebook code and saved JSON found no recognizable GitHub/OpenAI/Google API keys, private-key blocks, email addresses, or `/home` and mounted-Drive paths. This is not a guarantee that arbitrary embedded outputs or third-party data are suitable for public release. No notebooks were executed because experiments could be computationally expensive and some inputs are unavailable. Saved results are preserved historical outputs, not independently reproduced findings.

## Before a public portfolio release

Review scientific claims and authorship with the relevant collaborators; secure rights to publish any data, screenshots, outputs, or external content; remove unrelated coursework if desired; obtain redistributable input data or document access; create a tested environment lockfile and lightweight reproducibility checks; and replace or annotate Colab-only upload steps in a separate reviewed revision. Preserve this raw migration commit as the provenance record.
