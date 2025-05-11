
# 🧬 Predicting Vital Status in Sickle Cell Disease Using Machine Learning

## Overview

Sickle Cell Disease (SCD) is a complex genetic disorder associated with chronic complications and shortened life expectancy. This project leverages synthetic patient data to train and evaluate machine learning models that predict vital status in SCD patients. The primary goal is to facilitate **clinical risk stratification**, assess the **impact of gene therapy**, and improve **personalized treatment planning**.

---

## 📁 Project Structure

```
scd_vital_status_dashboard.html   ← Interactive HTML visualization
README.md                         ← Project overview and methodology
```

---

## 🧪 Dataset & Simulation

- **Data Type**: High-fidelity synthetic data (1,000 patients)
- **Class Imbalance**: 95% Alive, 5% Deceased
- **Features**: Demographics, clinical lab values, hospitalizations, organ damage, temporal metrics
- **Preprocessing**:
  - Iterative imputation
  - SMOTE oversampling
  - Feature engineering

---

## 🤖 Machine Learning Models

### 1. **LightGBM**  
- AUC ROC: > 0.99  
- AUPRC: > 0.96  
- Recall: 0.90  
- Interpretation: Feature importance + partial dependence plots

### 2. **Random Forest**  
- AUC ROC: > 0.99  
- Precision: 1.0  
- Specificity: 1.0  
- Slightly less recall, ideal for minimizing false positives

### 3. **Artificial Neural Network (ANN)**  
- Lower performance on test set  
- Not competitive with tree-based models in this scenario

---

## 📊 Key Insights

- Top Predictive Features:
  - Oxygen Saturation
  - LDH (Lactate Dehydrogenase)
  - Hemoglobin
  - Hospitalizations
  - Organ Damage

- These features align with clinical understanding of SCD progression and severity.

---

## 💡 Gene Therapy Simulation

A hypothetical 1.5x increase in Fetal Hemoglobin (HbF) was simulated using the LightGBM model, resulting in:

- **36% mean reduction** in predicted mortality risk

This supports the biological and clinical rationale behind **HbF-targeting gene therapy strategies**.

---

## 🔬 Future Directions

- Apply models to **real-world clinical data**
- Extend to **multi-outcome prediction** (e.g., hospitalization risk)
- Integrate **gene therapy patient cohorts**
- Use models for **personalized treatment optimization**

---

## 📫 Contact

**Victor Ikechukwu**  
📧 Email: [vikechukwu43@gmail.com](mailto:vikechukwu43@gmail.com)  
🔗 LinkedIn: [linkedin.com/in/victor-ikechukwu-1169942a7](https://www.linkedin.com/in/victor-ikechukwu-1169942a7?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app)  
📍 Location: Port Harcourt, Nigeria
