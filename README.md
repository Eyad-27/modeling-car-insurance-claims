# 🚗 Modeling Car Insurance Claim Outcomes  

<center><img src="car.jpg" width=500></center>  

Car insurance providers aim to estimate the likelihood of customers making claims during their policy period. Building predictive models allows them to optimize pricing and manage risks more effectively.  

In this project, I analyzed customer insurance data and built models using **one feature at a time** to determine which feature best predicts whether a customer will make a claim. The outcome was evaluated using **accuracy metrics**, with the goal of identifying a simple yet effective model for production.  

---

## 📌 Guiding Question  
- Which single feature in the dataset provides the **highest accuracy** in predicting whether a customer will make an insurance claim?  

---

## 📂 The Data  

### **car_insurance.csv**  
| Column      | Description                                                                 |  
|-------------|-----------------------------------------------------------------------------|  
| `id`        | Unique identifier for each customer                                         |  
| `outcome`   | Target variable indicating whether the customer filed a claim (1 = Yes, 0 = No) |  
| *other features* | Customer demographics, vehicle information, and insurance details (varied columns) |  

---

## 🛠️ How I Approached the Project  

1. **Reading and Exploring Data**  
   - Loaded the dataset into pandas.  
   - Inspected data types, distributions, and checked for missing values.  

2. **Data Cleaning**  
   - Filled missing values using appropriate statistics (mean, median, or mode depending on feature type).  

3. **Preparing for Modeling**  
   - Isolated each feature (excluding `id`) as a potential predictor of `outcome`.  
   - Created lists to store models and accuracy results.  

4. **Building Models**  
   - Iterated through features to train individual models.  
   - Stored predictions and evaluation metrics for each.  

5. **Measuring Performance**  
   - Used **confusion matrices** and accuracy scores to evaluate each model.  
   - Compared results across all features.  

6. **Identifying the Best Feature**  
   - Located the feature with the **highest accuracy score**.  
   - Stored the result in a DataFrame `best_feature_df` with:  
     - `best_feature`  
     - `best_accuracy`  

---

## ✅ Key Deliverables  
- Cleaned and prepared customer insurance dataset for modeling.  
- Built **single-feature models** for claim prediction.  
- Evaluated models using **accuracy scores** and confusion matrices.  
- Identified the most predictive feature for insurance claims.  
- Produced a summary DataFrame (`best_feature_df`) with results.  

---

## 🧰 Skills Used  
- Python (`pandas`, `scikit-learn`)  
- Data cleaning & preprocessing  
- Handling missing values  
- Model training & evaluation  
- Confusion matrix & accuracy metrics  
