# 🏥 ICUstay — Predicting ICU Length of Stay for Digestive System Diseases

This notebook presents a **complete machine learning pipeline** to predict the **length of stay (LOS)** in the **Intensive Care Unit (ICU)** for patients diagnosed with **diseases of the digestive system**, using the **MIMIC-III** clinical database.

The objective is to estimate the expected duration of ICU stay **early in the admission process**, which can help optimize **resource allocation** and improve **patient management**.

---

## 🧾 Dataset
The project uses data from the **MIMIC-III** database (Medical Information Mart for Intensive Care), a large open-access dataset containing de-identified health information from ICU patients.

Only patients diagnosed with **digestive system diseases** (ICD-9 codes `520–579`) were selected.  
Relevant tables from MIMIC-III were joined to include demographic information, admissions data, and ICU stay details.

📚 Reference: [MIMIC-III Tables Documentation](https://mimic.mit.edu/docs/iii/tables/)

---

## ⚙️ Data Preprocessing
1. **Data Extraction:**  
   Selection and merging of relevant tables (patients, admissions, diagnoses, icustays).
2. **Filtering:**  
   Patients with ICD-9 codes in the digestive system range were retained.
3. **Cleaning:**  
   Removal of missing or inconsistent records.
4. **Feature Engineering:**  
   Computation of age at admission, ICU stay duration, and other relevant predictors.
5. **Ethical Considerations:**  
   Adjustment for anonymized ages (patients older than 89 per HIPAA policy).

---

## 🧠 Modeling Pipeline
The notebook implements:
- Exploratory Data Analysis (EDA)
- Feature scaling and encoding
- Model training using NN
- Evaluation using standard metrics (MAE, RMSE, R²)
- Comparison and discussion of model performance

---

## 📈 Results
Models were evaluated in terms of accuracy and interpretability.  
The study highlights the predictive potential of clinical features for early LOS estimation and discusses trade-offs between complexity and explainability.

---

## 🧩 Technologies
- Python 3  
- pandas, NumPy, scikit-learn, matplotlib, seaborn  
- Jupyter Notebook  
- SQL (for MIMIC-III data extraction)

---

## 📘 Project Information
This project was developed for academic purposes only.  
**Course:** Machine Learning 2024  
**Professors:** Ines Dutra, Maria Pedroto  
**Date:** June 3rd, 2025  

## 👨‍💻 Authors
- Giulio Tamburini (ID: 202411174)
- Fabian Alexander Bug (ID: 202412325)  
- Gabriele Pascali (ID: 202411175)  
