# CO₂ Emissions Prediction
 
**OpenClassrooms — Data Scientist Path | Project 4** (December 2022 – February 2023)
 
> Note: project deliverables (notebooks, presentation) are in French.
 
## Sector
Energy
 
## Tech Stack
- Jupyter Notebook
- Python: scikit-learn, HyperOpt, SHAP
## Keywords
supervised regression, ensemble models, hyperparameter tuning, feature importance
 
## Context
The City of Seattle has set a carbon neutrality target for 2050. As part of this strategy, the city needs to monitor two key metrics for non-residential buildings: total energy consumption and CO₂ emissions. Accurate predictions would allow the city to adapt its policy without relying solely on costly on-site measurements.
 
## Mission
Build two prediction models: one for total energy consumption, one for CO₂ emissions of non-residential buildings.
 
## Selected Algorithm
**XGBoost**
 
## Deliverables
- `notebook_exploratoire.ipynb` — data cleaning and exploratory analysis
- `notebook_prediction_conso.ipynb` — model experiments for energy consumption prediction
- `notebook_prediction_co2.ipynb` — model experiments for CO₂ emissions prediction
- `toolbox.py` — helper functions used across notebooks
- `presentation.pdf` — presentation slides (in French)
## Methodology
 
1. **Data cleaning**
   - Select relevant variables
   - Handle duplicates, outliers, and missing values
2. **Feature engineering & preprocessing**
   - Variable transformations: RobustScaler, OrdinalEncoder, TargetEncoder, log and square transformations
3. **Modelling**
   - Pipeline + cross-validation framework
   - Baseline (naive) model as reference
   - Benchmarked multiple model families:
     - Linear: Linear Regression, Lasso, Ridge, Elastic Net, SVM
     - Kernel: Kernel Ridge, Kernel SVM
     - Ensemble: Gradient Boosting, XGBoost, CatBoost, Bagging, Random Forest, AdaBoost
   - Feature importance analysis with SHAP
   - Iterative refinement of input variables based on SHAP insights
4. **Hyperparameter optimisation**
   - Shortlist best models by training time, MAE, R², RMSE
   - Optimise hyperparameters of top candidates with HyperOpt
   - Select final model
## Skills
- Selecting the appropriate supervised learning algorithm for a business problem
- Engineering and transforming features for supervised models
- Evaluating model performance with relevant metrics
- Tuning hyperparameters to improve model performance
## Data Source
[City of Seattle — 2016 Building Energy Benchmarking](https://data.seattle.gov/dataset/2016-Building-Energy-Benchmarking/2bpz-gwpy)
