# 🚢 Titanic Survival Prediction

A binary classification project to predict whether a passenger survived the Titanic disaster using machine learning models.

## 📁 Dataset

The dataset includes details like:
- Passenger class (Pclass)
- Sex
- Age
- SibSp (siblings/spouses aboard)
- Parch (parents/children aboard)
- Ticket fare
- Cabin info
- Embarked (port of embarkation)

## 🧹 Data Preprocessing

- **Missing values**: Handled appropriately (e.g., filling or dropping depending on context).
- **Categorical Encoding**: Dictionary-based encoding used for categorical features, as there were very few unique labels.
- **Normalization**: `StandardScaler` was applied to numerical data, especially for models like Logistic Regression and SVC.

## 🧠 Model Selection

Three models were considered for binary classification:

- **Logistic Regression**
- **Random Forest Classifier**
- **Support Vector Classifier (SVC)**

```python
# Models used
models = {
    'logistic_regression': LogisticRegression(...),
    'random_forest': RandomForestClassifier(...),
    'svc': SVC(...)
}
```

Each model was trained on the scaled training data and evaluated using accuracy and confusion matrix.

## ✅ Results

| Model               | Accuracy |
|---------------------|----------|
| Logistic Regression | 1.0000   |
| Random Forest       | 1.0000   |
| SVC                 | 0.94     |

> 💡 *Final model chosen:* **Random Forest Classifier** due to consistent high performance.

## 📊 Evaluation Metrics

- Accuracy
- Confusion Matrix

## 📌 Conclusion

This project successfully demonstrates a complete ML pipeline:
- Data cleaning
- Encoding and scaling
- Model training and evaluation
- Final model selection based on performance

---
