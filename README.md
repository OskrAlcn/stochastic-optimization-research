# Stochastic Optimization Research

Private research-notebook archive covering stochastic optimization, chance-constrained programming, risk measures, and applications. The repository owner is a Civil Mathematical Engineering student at Universidad Técnica Federico Santa María and reports working as a research assistant to Professor Julio Deride since August 2025. The notebooks were developed by the owner and subsequently reviewed and discussed with the professor. The files do not, by themselves, establish authorship of external publications or independent validation of the recorded results.

## Research lines

| Line | Focus |
| --- | --- |
| [Stochastic optimization](research/stochastic-optimization/README.md) | Adaptive and non-adaptive mathematical programming. |
| [Rockafellians and chance-constrained programming](research/rockafellians-and-chance-constrained-programming/README.md) | Probability constraints, scenario approximations, and CVaR-based formulations. |
| [Production planning and lot-sizing](research/production-planning-and-lot-sizing/README.md) | Stochastic production decisions and service reliability. |
| [Hydroelectric reservoir optimization](research/hydroelectric-reservoir-optimization/README.md) | Scheduling cascaded reservoirs under uncertain inflows. |
| [Demand-side management](research/demand-side-management/README.md) | Time-of-use pricing subject to transformer reliability. |
| [Wind energy and time-series modeling](research/wind-energy-and-time-series-modeling/README.md) | ARMA modeling and wind-generation scenarios. |
| [Evolutionary finance](research/evolutionary-finance/README.md) | Investor survival with endogenous asset payoffs. |
| [Risk measures](research/risk-measures/README.md) | Budget-risk envelopes, CVaR, and related measures. |

The [archive](archive/README.md) retains preliminary, secondary, duplicate, and unrelated notebooks without changing their code or saved outputs. See the [full inventory](docs/SOURCE_INVENTORY.md), [provenance and checksums](docs/provenance.csv), and [reproducibility notes](docs/REPRODUCIBILITY.md).

## Working with the notebooks

The notebooks were authored in Google Colab. Create an isolated Python environment and install the requirements for the relevant research line from `requirements/`. Package versions were not recorded consistently in the sources, so these files identify dependencies rather than guaranteeing an exact recreation of the original Colab environment. Some notebooks require a solver, manually uploaded data, or network access; consult each line's README and the reproducibility notes before running. Existing saved outputs are historical artifacts and have not been regenerated during this migration.

## Scope of this migration

All 16 source notebooks were copied as original `.ipynb` files. The source Drive folder was read only. No mathematical code or saved output was edited, and no computational experiments were run. The repository is intended to remain private until data rights, scientific claims, licensing, and reproducibility have been reviewed.
