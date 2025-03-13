# 🏥 H1N1 Vaccine Hesitancy Prediction  
## 📌 Project Overview  
This project predicts **H1N1 vaccine uptake** using **machine learning models** on survey data from the **2009 National Flu Survey (NHFS)**. The goal is to **understand key factors** influencing vaccine hesitancy and improve public health strategies.

---

## 📊 Data Understanding  
- **Dataset**: 2009 National Flu Survey (NHFS)  
- **Target Variable**: `h1n1_vaccine` (1 = Vaccinated, 0 = Not Vaccinated)  
- **Key Features**:
  - **Doctor recommendations**  
  - **Perceived vaccine effectiveness**  
  - **Health insurance status**  
  - **Demographic factors** (age, location, employment)  
  - **Health behaviors** (handwashing, mask-wearing, etc.)

---

## 🔍 Machine Learning Models Tested  
The following models were evaluated:  
✅ **Decision Tree**  
✅ **Logistic Regression**  
✅ **Random Forest (Best Performing)**  
✅ **K-Nearest Neighbors (KNN)**  
✅ **Naive Bayes**  

📌 **Random Forest achieved the highest accuracy of 83.5%** with balanced precision and recall.

---

## 🛠 Model Training & Hyperparameter Tuning  
- Data preprocessing included **handling missing values, scaling numerical features, and encoding categorical variables**.  
- **GridSearchCV** was used for **hyperparameter tuning** to optimize model performance.  
- The best **Random Forest model** was trained with:  
  - `n_estimators`: 100  
  - `max_depth`: None  
  - `min_samples_split`: 2  
  - `min_samples_leaf`: 1  

---

## 📊 Model Performance & Insights  
### 🎯 **Final Random Forest Performance**
- **Accuracy**: **83.5%**  
- **Precision**: **70.0%**  
- **Recall**: **39.0%**  
- **F1-Score**: Balanced precision and recall.  

### 🔹 **Top Features Influencing Vaccine Uptake**  
1️⃣ **Doctor Recommendations** – Strongest predictor.  
2️⃣ **Perceived Risk & Effectiveness** – Higher belief in effectiveness increases uptake.  
3️⃣ **Demographics & Health Behavior** – Age, location, and precautions impact vaccination.  

---

## 📌 Conclusion  
- **Doctor recommendations and risk perception are the strongest factors** influencing vaccination.  
- The **Random Forest model provided the best predictions**, balancing accuracy and interpretability.  
- These insights can help **public health officials improve vaccine awareness campaigns** and increase uptake.


References
National Flu Survey (NHFS) 2009
Scikit-Learn Documentation: https://scikit-learn.org
