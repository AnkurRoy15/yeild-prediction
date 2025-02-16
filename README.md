# XGBoost-Based Crop Yield Prediction

## 📌 Project Overview
This project implements a **Crop Yield Prediction Model** using **XGBoost**. The model leverages key agricultural features such as **crop type, season, rainfall, fertilizer usage, and pesticide application** to predict the expected crop yield.

## 🚀 Features
- **Uses XGBoost Regressor** for accurate predictions
- **Handles missing values** effectively
- **Feature engineering**: Interaction terms and log transformations
- **Hyperparameter tuning** with GridSearchCV
- **Custom input prediction function** for real-time yield estimation
- **Feature importance analysis**

## 🛠️ Installation & Setup
1. **Clone the repository**
   ```bash
   git clone https://github.com/your-repo/xgboost-yield-prediction.git
   cd xgboost-yield-prediction
   ```
2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```
3. **Run the script**
   ```bash
   python yield_prediction.py
   ```

## 📂 Dataset Format
The model expects a dataset with the following columns:
- **Crop** (Categorical)
- **Crop_Year** (Integer)
- **Season** (Categorical)
- **State** (Categorical)
- **Area** (Float)
- **Annual_Rainfall** (Float)
- **Fertilizer** (Float)
- **Pesticide** (Float)
- **Yield** (Target Variable)

## 📊 Model Training & Evaluation
The model is trained using **GridSearchCV** to find the optimal hyperparameters. It evaluates performance using:
- **Mean Absolute Error (MAE)**
- **R² Score**
- **Feature Importance Analysis**

## 🔍 Predicting Yield for Custom Inputs
You can use the function `predict_yield()` to estimate crop yield for a custom set of inputs:
```python
predicted_yield = predict_yield("Wheat", 2023, "Rabi", "Punjab", 5000, 1200, 300, 50)
print(f"Predicted Yield: {predicted_yield:.2f}")
```

## 📌 Future Enhancements
- Implement a **REST API using FastAPI** for real-time predictions
- Develop a **React Native app** to integrate the model
- Incorporate **more advanced feature engineering** and external weather data

## 🤝 Contributing
Feel free to fork the repo and submit **pull requests** for improvements! 😊

## 📜 License
This project is open-source under the **MIT License**.

