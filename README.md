
###  **Project: Fraud Detection using Random Forest**

---

###  **Objective**
- Detect fraudulent transactions from financial data.
- Handle extreme class imbalance (fraud cases are very few).

---

### 📊 **Model Evaluation**
- **Confusion Matrix:**
  ```
  [[1262657    8247]
   [     18    1602]]
  ```
- **Classification Report Highlights:**
  - Fraud class (1):
    - Precision: 0.16
    - Recall: 0.99
    - F1-score: 0.28
  - Accuracy: 99%
  - Focused on **recall** to minimize false negatives

---

###  **Preprocessing Steps**
1. Drop irrelevant fields if any
2. One-hot encode `type` column
3. Split data into `X_train`, `X_test`, `y_train`, `y_test`
4. Optional: handle outliers or scale features

---

###  **Visualization**
- **Correlation Heatmap**
- **KDE Plots** for all features (4 per row for readability)
---

###  **Model Tuning**
- Used `RandomSearchCV` for hyperparameter optimization
