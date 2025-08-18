# Probabilistic Modeling of Methane Hydrate Kinetics

This project predicts methane hydrate kinetics across varying catalysts and concentrations using thermokinetic equation–guided machine learning and probabilistic inference (**MLE, MAP, Full Bayesian**). Models achieve **90%+ accuracy** and are validated with **MSE, RMSE, and R²**. Research-oriented metrics (**t₉₀, initial slope, final conversion**) are derived for publication-quality analysis.

## 📂 Repository Structure
- `dataset/` — data for catalysts & concentrations (train/test or raw/processed)
- `MLE-MAP/` — scripts/notebooks for ML & MAP modeling
- `full-bayesian-inference/` — PyMC/ArviZ Bayesian model, ADVI warm-start + NUTS
- `requirements.txt` — dependencies

## 🔧 Setup
```bash
python -m venv .venv && source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r requirements.txt
