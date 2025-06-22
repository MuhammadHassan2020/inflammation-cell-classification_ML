
# 🧠 Inflammation Classification with Machine Learning on Histology Data

## 📌 Project Overview  
This project focuses on **classifying inflammation severity** based on histology-derived features using machine learning. The goal is to evaluate performance across full and reduced feature sets to determine the feasibility of using fewer measurements without compromising accuracy.  

Using advanced ML techniques, including feature selection, classification, and evaluation metrics, this study explores the diagnostic capabilities of AI in medical data analysis.

## 🧠 Business Problem  
Manual inflammation classification from histology data is time-consuming and prone to human bias. Automating this process with machine learning offers:  
- Faster diagnosis and clinical decision-making  
- Reduction of human error in inflammation classification  
- Potential to improve healthcare efficiency using fewer diagnostic features  

## 💥 Impact  
- 🚑 Supports clinicians in diagnosing inflammation with minimal inputs  
- ⚕️ Enables AI-assisted histopathology for real-world application  
- 📉 Demonstrates reduced-feature models retain high performance—critical for cost-effective diagnostics  
- 💻 Builds foundation for more scalable inflammation classification systems

## ✅ Solution  
The solution pipeline included:  

- **Data Cleaning & Preparation**  
  - Dropped rows with high missing values  
  - Median imputation (robust to outliers)  
  - Class balancing using **SMOTE**

- **Feature Selection**  
  - Identified top 10 features via importance metrics

- **Modeling**  
  - Models: **Random Forest (RF)** and **Logistic Regression (LR)**  
  - Tasks:  
    - Multi-class classification of inflammation severity  
    - Binary classification (No Inflammation vs Inflammation)

- **Evaluation Metrics**  
  - Accuracy, Sensitivity, Specificity, ROC AUC  
  - Stratified GroupKFold Cross Validation  
  - Full vs Reduced feature comparisons

---

## 🧰 Tools & Technologies Used  
- **Languages**: Python  
- **Libraries**: pandas, numpy, scikit-learn, imbalanced-learn, matplotlib, seaborn  
- **Techniques**: SMOTE, GroupKFold, Random Forest, Logistic Regression  
- **Platform**: Jupyter Notebook  

## 📊 Dataset Information  
- Source: Clinical Histology Dataset  
- Features: 150+ histology variables  
- Labels:  
  - Severity Score (0–5) – Multi-class  
  - Binary Label (Inflammation / No Inflammation)  

## 📈 Results Summary  

### 🔹 Multi-class Classification (Severity Score)  
| Model             | Accuracy (Reduced) | Accuracy (Full) |
|------------------|--------------------|-----------------|
| Random Forest     | 79.66%             | 87.88%          |
| Logistic Regression | 60.86%           | 65.15%          |

### 🔹 Binary Classification (Inflammation Detection)  
| Model             | Accuracy (Reduced) | Accuracy (Full) | ROC AUC (Full) |
|------------------|--------------------|-----------------|----------------|
| Random Forest     | 92.30%             | 96.15%          | 0.95           |
| Logistic Regression | 84.61%           | 92.30%          | 0.94           |

🔍 **Key Insight**: Reduced-feature models performed well, showing that fewer variables can still yield strong performance—critical for low-cost medical diagnostics.

## 🔍 Why This Project?  
This project aligns with the increasing demand for **AI in medical diagnostics**. I aimed to:  
- Apply ML in a healthcare setting  
- Explore interpretability of reduced feature models  
- Develop robust classification pipelines in a real-world scenario  


## 🚀 Future Work  
- 🧠 Integrate interpretability methods (e.g., SHAP, LIME)  
- 🔍 Deploy web app for real-time inflammation prediction  
- 📊 Test generalizability on external histology datasets  
- 🩺 Collaborate with clinical experts for validation  


## 📂 Repository Usage  
To run this project:

```bash
git clone https://github.com/your-username/inflammation-classification-ml.git
cd inflammation-classification-ml
