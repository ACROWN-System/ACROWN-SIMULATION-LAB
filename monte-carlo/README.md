# Monte Carlo Models

**Status:** reserved scaffold; no Monte Carlo implementation was present in the reviewed baseline.

Before a decision-relevant run, document the target quantity, model equations, parameter distributions and provenance, dependencies/correlations, run count, seed policy, convergence or precision rationale, uncertainty method, and sensitivity checks. Explain which factors are omitted and why.

A large number of runs reduces some sampling error; it does not correct a misspecified model or unsupported input distributions. Separate numerical stability from empirical validity. If criteria or adequate validation are missing, the output is exploratory or the decision remains BLOCKED.

Consult the current [AstroCrown ACS Monte Carlo specification](https://github.com/ACROWN-System/AstroCrown_ACS_MC_Spec). See the root [simulation evidence rules](../README.md).
