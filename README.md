# 🏡 House Price Prediction using Machine Learning  

## 📌 Overview  
This project aims to **predict housing prices** using machine learning techniques by considering property details, education quality, neighborhood safety, and green living features.  

The goal is to build a reliable model that can assist **buyers, sellers, and real estate agents** in making informed decisions.  

---

## 🎯 Objectives  
- Predict house prices using structured data.  
- Incorporate **education (school ratings)**, **neighborhood safety (crime statistics)**, and **green living (walkability, parks, pollution)** into the model.  
- Use **XGBoost** for accurate regression predictions.  
- Provide **visual insights** into how features affect housing prices.  
- Deliver a **reproducible ML workflow** with preprocessing, training, evaluation, and saving the model.  

---

## 📊 Dataset  
The dataset includes property and neighborhood details such as:  
- **Property Features** → Bedrooms, Bathrooms, Square footage, Year built, Lot size.  
- **Financials** → Listing price, Sold price, Taxes.  
- **Education** → Elementary, Middle, and High school ratings.  
- **Neighborhood Safety** → Crime grades (overall, violent, property, other crimes).  
- **Green Living** → Walk score, Air quality, distance to amenities (parks, trails, grocery).  

---

## 🛠️ Libraries Used  
- **pandas** → Data loading & manipulation  
- **numpy** → Numerical computations  
- **matplotlib / seaborn** → Data visualization  
- **scikit-learn** → Preprocessing, pipelines, metrics  
- **xgboost** → Machine learning model  
- **joblib** → Save and load trained models  

---

## ⚙️ Workflow  
1. **Data Preprocessing** → Clean column names, handle missing values.  
2. **Feature Engineering** → Create new features:  
   - `House_Age`  
   - `Avg_School_Rating`  
   - `AvgCrimeScore`  
   - `GreenLivingIndex`  
3. **Feature Selection** → Choose structural, financial, and engineered features.  
4. **Train-Test Split** → 80/20 split for unbiased evaluation.  
5. **Pipeline & Scaling** → Use StandardScaler & imputation inside pipeline.  
6. **Model Training** → Train with **XGBoost Regressor**.  
7. **Evaluation** → MAE, RMSE, R².  
8. **Visualizations** → Feature importance, scatter plots, heatmaps.  
9. **Model Saving** → Export trained model as `.joblib`.  

---

## 📈 Results  
- **XGBoost** achieved strong performance in predicting housing prices.  
- **Most influential features**: Listing Price, Original Price, Square Footage, Taxes, School Ratings, and Neighborhood Safety.  
- Added **visualizations** to show correlations and feature distributions.  

---

## 📂 Project Structure  
├── AIML Project.ipynb # Jupyter notebook with full code
├── Case Study.docx # Detailed documentation
├── Case Study.pdf # PDF version of the report
├── housing_price_model_strong_predictors.joblib # Saved ML model
├── README.md # Project overview (this file)
