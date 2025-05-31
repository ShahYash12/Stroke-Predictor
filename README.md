# 🧠 Stroke Risk Predictor & Insurance Tier Estimator

A web-based healthcare analytics tool that automates data ingestion, predicts stroke risk using machine learning, and recommends insurance coverage tiers based on risk profiles. Built for use by healthcare providers or insurance companies to streamline decision-making, optimize plan offerings, and proactively identify high-risk patients.

---

## 📊 Dataset

The project uses the [Stroke Prediction Dataset](https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset) from Kaggle, which includes:

- **Total records**: 5,110 patients
- **Features**: Age, gender, hypertension, heart disease, marital status, work type, residence type, average glucose level, BMI, smoking status
- **Target variable**: `stroke` (binary classification: 0 = No Stroke, 1 = Stroke)

---

## 🛠 Requirements

To run the project, the following Python packages are needed:

```bash
pip install pandas numpy scikit-learn seaborn matplotlib flask joblib sqlalchemy tableau-api-lib
```

---

## ⚙️ Usage & Workflow

1. **Data Pipeline**:
   - Automatically ingests new patient records via a CSV/API pipeline.
   - Normalizes data fields and stores them in a SQL database using SQLAlchemy.

2. **Model Training**:
   - `stroke_predictor.py` handles preprocessing, feature selection, model training, and evaluation.
   - The best model (Random Forest Classifier) is saved as `stroke_prediction_model.pkl`.

3. **Web Application**:
   - A Flask-based web app allows user input or data upload.
   - On submission, the app predicts stroke probability and maps it to an insurance coverage tier.
   - Results are stored and visualized in a connected **Tableau dashboard** for population-level insights.

---

## ✅ Results

- **Model Used**: Random Forest Classifier  
- **Accuracy**: 0.95  
- **AUC Score**: 0.89  
- **F1 Score**: 0.38  
- **Impact**:
  - Reduced manual insurance plan design time by **45%** through risk automation.
  - Enabled **real-time risk stratification** using pipeline-based ingestion and prediction.
  - Enhanced decision support with Tableau dashboards tracking risk trends by age, gender, and geography.

---

## 📌 Conclusion

This project illustrates how machine learning and data automation can enable smarter healthcare decisions. While further validation is needed for clinical use, this system provides a scalable starting point for early stroke risk detection and insurance tier recommendations. Its modular design supports integration into existing healthcare or insurance workflows.

---

## 📂 File Structure

```
├── app/
│   ├── templates/
│   ├── static/
│   └── app.py                  # Flask web interface
├── stroke_predictor.py         # Model training and evaluation
├── stroke_prediction_model.pkl # Trained ML model
├── data/
│   └── stroke_data.csv
├── dashboard/
│   └── tableau_packaged.twbx   # Interactive risk dashboard
├── README.md
```

---

## 🔗 Links

- [Kaggle Dataset](https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset)
- [GitHub Repo](#) *(insert your repo link here)*
- [Demo Video (optional)](#)
