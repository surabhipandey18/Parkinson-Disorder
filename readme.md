# Parkinson's Disease Detection using Voice Features 🎙️🌿

This project aims to develop a machine learning model that detects Parkinson’s Disease (PD) based on biomedical voice measurements. Parkinson’s Disease is a progressive neurological disorder that primarily affects movement and speech. Since voice impairment is an early and prominent symptom of PD, analyzing vocal biomarkers offers a promising, non-invasive method for early detection.

## 🧠 Problem Statement

Parkinson's Disease is typically diagnosed through clinical evaluation, which is subjective and often delayed. By leveraging machine learning, we aim to build a classification model that can accurately predict whether a person has Parkinson’s based solely on voice recordings — potentially enabling early diagnosis and remote screening.

---

## 📊 Dataset

- **Source**: UCI Machine Learning Repository
- **Samples**: 195 voice recordings
- **Subjects**: 31 individuals (23 diagnosed with PD)
- **Target Variable**: `status` (1 = PD, 0 = healthy)
- **Citation**:
  > 'Exploiting Nonlinear Recurrence and Fractal Scaling Properties for Voice Disorder Detection',  
  > Little MA, McSharry PE, Roberts SJ, Costello DAE, Moroz IM.  
  > _BioMedical Engineering OnLine 2007, 6:23 (26 June 2007)_

---

## 🧪 Features Used

Top features based on Random Forest feature importance:

| Feature              | Importance |
|----------------------|------------|
| PPE                  | 0.1419     |
| MDVP:Fo(Hz)          | 0.1036     |
| spread1              | 0.1006     |
| MDVP:Flo(Hz)         | 0.0794     |
| Jitter:DDP           | 0.0621     |
| ...                  | ...        |

---

## 🛠️ Model: Random Forest Classifier

We use Random Forest due to its robustness and capability to handle non-linear relationships effectively.

### ✅ Model Performance (on cross-validation)

- **Accuracy**: 89.74%
- **Precision**: 91.18%
- **Recall**: 96.88%
- **F1 Score**: 93.94%

### 📄 Classification Report

           precision    recall  f1-score   support
 Healthy       0.80      0.57      0.67         7
     PD       0.91      0.97      0.94        32

Accuracy                           0.90        39
Macro Avg 0.86 0.77 0.80 39
Weighted Avg 0.89 0.90 0.89 39

🧠 Author
Surabhi Pandey
🌐 LinkedIn