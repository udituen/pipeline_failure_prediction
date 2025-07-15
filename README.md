# Pipeline Failure Prediction Using Machine Learning

## Project Overview
This project builds a machine learning model to predict the risk of pipeline failure based on sensor and operational data. It demonstrates techniques commonly used in predictive maintenance within the oil & gas sector, where failure prevention has high safety and financial impact.

---

## Business Problem
Pipeline failures can cause environmental damage, operational downtime, and financial losses. Predicting failures allows operators to take preventive actions, reducing risk and costs.

---

## Technologies & Tools
- **Python**: pandas, scikit-learn, xgboost, imbalanced-learn
- **Visualization**: matplotlib, seaborn
- **ML Techniques**: Classification, Anomaly Detection
- **Evaluation**: Precision, Recall, F1-Score, ROC-AUC
- **Optional**: Power BI for reporting dashboards

---

## 📂 Project Structure
```
pipeline-failure-prediction/
├── data/
│   ├── raw/                # Original, unprocessed data files
│   └── processed/          # Cleaned and feature-engineered datasets
├── notebooks/
│   ├── 01-EDA.ipynb        # Exploratory Data Analysis
│   ├── 02-Modeling.ipynb   # Model Training and Evaluation
│   ├── 03-Visualization.ipynb # Visualization for reporting
├── src/
│   ├── preprocessing.py    # Data cleaning and feature engineering functions
│   ├── modeling.py         # ML training pipeline
├── reports/
│   ├── figures/            # Model performance charts, visualizations
│   ├── results-summary.md  # Summary of findings, key metrics
├── requirements.txt        # Python dependencies
├── README.md               # Project overview, instructions
└── .gitignore              # Standard .gitignore for Python
```


---

## Data Sources
- **PHMSA Pipeline Incident Data**: [PHMSA Data Portal](https://www.phmsa.dot.gov/data-and-statistics/pipeline/pipeline-incident-20-year-trends)
- **Simulated Sensor Data**: Synthetic datasets created for pressure, temperature, flow rate, and vibration.

---

## How to Run This Project
1. Clone this repository:
    ```bash
    git clone https://github.com/YOUR-USERNAME/pipeline-failure-prediction.git
    cd pipeline-failure-prediction
    ```

2. Create a virtual environment:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    ```

3. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

4. Run the Jupyter notebooks:
    ```bash
    jupyter notebook
    ```
Note: This project uses docker and airflow for end to end MLOps process
on windows, the command 
```Remove-Item alias:curl```
is needed to run the curl script that pulls docker compose when building
---

## Expected Outcomes
- Clean, analyzed dataset of pipeline sensor data
- Trained machine learning model for failure prediction
- Business-focused evaluation report (precision, recall, cost of failure avoided)
- Visual dashboard for communicating findings

---

## Key Results (Sample)
- ROC-AUC: 0.92
- Precision (Failure Class): 0.85
- Recall (Failure Class): 0.88

---

## Future Work
- Incorporate time-to-failure modeling (survival analysis)
- Deploy model as a REST API for real-time inference
- Integrate dashboard with Power BI for live reporting

---

## Author
**Uduak Ituen**  
Machine Learning Engineer  
[GitHub](https://github.com/udituen) • [LinkedIn](https://linkedin.com/in/uduak-ituen)

---
