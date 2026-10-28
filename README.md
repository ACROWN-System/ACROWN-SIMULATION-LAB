# ACROWN-SIMULATION-LAB

**Reviewed main tree SHA:** `35f150a971f7500812f1657e53a2a27a0f23700d`  
**Current status:** scaffold; no executable simulation or result evidence was present in that baseline.

## Purpose

A controlled home for scenario models and simulations supporting ACROWN-System research. The repository currently reserves these areas:

- `agent-models/` — agent and interaction models
- `governance-models/` — governance and decision-rule models
- `monte-carlo/` — stochastic and parameter-uncertainty simulations
- `paymaster-models/` — transaction-sponsorship and cost models
- `scenarios/` — defined scenario inputs
- `results/` — reproducible outputs and evaluations

These directories are organizational placeholders, not evidence that the corresponding models are implemented.

## Scientific boundary

A simulation establishes what follows **inside a specified model under specified assumptions**. It does not, by itself, establish that the assumptions describe reality; prove general understanding or transfer; demonstrate swarm safety; predict an actual financial outcome; or provide a security, regulatory, or independent certification.

Passing tests can show that code behaves as intended. It does not establish that the model is adequate for the real-world question. Keep implementation correctness, empirical validity, and decision suitability as separate claims.

## Minimum record for every substantive run

Record, at minimum:

1. Question, intended decision, scope and exclusions.
2. Model structure, assumptions, units, equations/rules and known omissions.
3. Provenance/version of parameters and data, including transformations.
4. Code commit, configuration, runtime/dependencies, exact command and seed policy.
5. Predeclared acceptance criteria and the reason they fit the intended decision.
6. Implementation tests, calibration evidence where applicable, and independent/out-of-sample validation where available.
7. Uncertainty method, sensitivity analysis, scenario coverage and material failure cases.
8. Raw outputs, analysis steps, limitations, anomalies and reproducibility instructions.

Where a requirement is unavailable, say so rather than silently substituting an assumption. Report run counts, seeds, distributions and uncertainty in a form appropriate to the model; do not present a point estimate as certainty.

## Decision boundary

Use the repository's established result labels: **PASS / FAIL / N/A / BLOCKED**. State the tested scope beside any result. A PASS applies only to its predeclared criteria and tested scope; it is not a global guarantee. If decision-critical assumptions, acceptance criteria, or adequate validation are missing, keep the decision **BLOCKED** or explicitly exploratory.

For Monte Carlo work, consult the current [AstroCrown ACS Monte Carlo specification repository](https://github.com/ACROWN-System/AstroCrown_ACS_MC_Spec). If decision-grade requirements are ambiguous, incomplete or unverified, do not label outputs decision-grade.

## Change discipline

Keep models, inputs, evaluation code and results traceable to versions. Do not overwrite historical evidence. Preserve failed and inconclusive runs when they materially explain a decision. Never infer safety or validity merely from model complexity, number of agents, run volume, or plausible-looking output.

This README defines evidence expectations; it does not implement a simulator or certify that any model is valid.
