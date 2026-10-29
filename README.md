# bayesian-scorecard-sandbox
Experiment sandbox for credit risk scorecard research.

Workflow:
1. Data cleaning & filtering
2. Train/test split
3. WOE binning, IV calculation, traditional scorecard construction
4. Stratified analysis, probability transformation
5. Counterfactual experiments
6. Optional: Bayesian probability calibration / other probabilistic calibration methods

Environment: Python
Packages: numpy, scipy, pandas, matplotlib, seaborn, scikit-learn, statsmodels, pymc, dowhy, numba

⚠️ Important note on probability calibration:
When implementing probability calibration (Bayesian calibration, Platt scaling, isotonic regression etc.),
must include calibration evaluation: reliability diagram, Brier score, calibration curve, Hosmer-Lemeshow test.
Do NOT skip calibration diagnosis.
