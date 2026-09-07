# Memoire-M2-ISF-Dauphine
Forecasting and Stress Testing Bank Interest Rate Risk (IRRBB) using a Hybrid Stochastic and Machine Learning Approach


**Objective**: forecast and stress test the EUR interest rate swap spread 
(Swap 5Y − Euribor 3M), a key proxy for bank margin under the IRRBB 
regulatory framework, using a hybrid approach combining stochastic rate 
models, machine learning, an LLM regime-classification agent, and a 
diffusion-based generative model.

## Repository structure

| Notebook | Thesis section(s) | Content |
|---|---|---|
| `chapitre4.1_données+FE.ipynb` | 4.1–4.2 | Data collection from the ECB API (Euribor, EUR swap rates), Nelson-Siegel factor construction (Level, Slope, Curvature), feature engineering, descriptive analysis and correlation matrix |
| `Chapitre4.3-XGboost+4.7+4.8-stresstesting.ipynb` | 4.3, 4.7, 4.8 | Ridge/Lasso baseline, XGBoost predictive model, SHAP interpretability, EBA regulatory stress scenarios (Spread-at-Risk, NIM/EVE sensitivity), and backtesting on the 2022–2023 rate crisis |
| `Chapitre4.4-agent-IA.ipynb` | 4.4 | LLM agent (Tavily + GPT-4o-mini) for market regime classification (STRESS/NORMAL), bootstrap validation of predictive gain, SHAP analysis of the stress score |
| `Chapitre4.5_HW.ipynb` | 4.5 | Vasicek/Hull-White calibration (MLE), forward curve and convexity shift α(t), Monte Carlo simulation, Vasicek vs. Hull-White comparison |
| `Chapitre4.6_DDPMDDIM.ipynb` | 4.6 | Diffusion-based generative model (DDPM/DDIM) trained on historical rate trajectories, distribution comparison with Hull-White, Kolmogorov-Smirnov test |


