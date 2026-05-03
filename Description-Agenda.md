## Phase 1: Data Preparation & Repository Setup (March 30 – April 5)

* **Infrastructure:** Initialize the shared GitHub repository. All members must commit with clear version history to demonstrate collaborative participation per rubric requirements.
* **Data Ingestion:** Load and audit the Superstore transactional sales dataset.
* **Data Cleaning:** Remove incomplete records, validate time coverage, and verify data integrity.
* **Preprocessing Pipeline:** Build the shared transformation workflow including daily/monthly resampling, zero-sales handling, and log transformation.
* **Baseline Development:** Implement shared benchmark models (Naïve Forecast and Historical Mean) that all forecasting models must outperform.

---

## Phase 2: Joint Exploratory Data Analysis (April 6 – April 12)

* **Feature Engineering:** Construct calendar-based predictors, rolling trend features, and variance-stabilized log-transformed sales series.
* **EDA Artifacts:** Generate distribution plots, trend analysis, seasonality diagnostics, and autocorrelation visualizations.
* **Validation Protocol:** Formally document the chronological evaluation framework (Train: 2015–2017 / Test: 2018) and primary performance metrics (MAE, RMSE).
* **The Output:** Export finalized model-ready datasets:

  * `clean_daily_ready.csv`
  * `clean_monthly_ready.csv`

---

## Phase 3: Individual Modeling Sprints (April 13 – April 26)

*Working in individual notebooks, all members train their assigned forecasting models using the shared cleaned datasets to predict retail sales across identical forecast horizons.*

* **Member 1 (SARIMA):** Focuses on capturing structured weekly and yearly seasonal demand patterns using statistical time-series decomposition.
* **Member 2 (ETS):** Focuses on level, trend, and seasonal smoothing to model stable retail demand evolution.
* **Member 3 (XGBoost):** Focuses on nonlinear sales dynamics, calendar interactions, and short-term demand irregularities through machine learning.

---

## Phase 4: Evaluation, Discussion & Submission (April 27 – May 8)

* **Performance Review:** Evaluate all models on the exact same holdout test set using MAE and RMSE against the shared baselines.
* **Comparative Analysis:** Assess forecasting accuracy across short-term daily and medium-term monthly horizons.
* **Group Reflection:** Discuss model strengths, forecasting stability, computational efficiency, and business relevance for retail demand planning.
* **Submission Formatting:** Finalize repository deliverables including:

  * Joint EDA Notebook
  * Individual Modeling Notebooks
  * Final project synthesis and comparative evaluation report
