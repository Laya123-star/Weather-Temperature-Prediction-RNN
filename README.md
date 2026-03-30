# 🌦️ Weather Temperature Prediction using RNN (Deep Learning)

![Python](https://img.shields.io/badge/Python-3.9-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-DeepLearning-orange)
![RNN](https://img.shields.io/badge/Model-RNN-green)
![Platform](https://img.shields.io/badge/Platform-Google%20Colab-yellow)

A deep learning project focused on building and evaluating a **Recurrent Neural Network (RNN)** for **time-series forecasting** using weather data.

---

## 🚀 Run Notebook in Google Colab

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1i0i7nBdfW63Q2hr2J2WSoMpHJnEK_rK1)

---

## 📘 Project Overview

This project implements a **SimpleRNN model** to predict future temperature values based on historical weather data.

The project covers:

- Dataset exploration
  
- Time-series preprocessing
  
- Sequence generation
  
- RNN model design
  
- Model training and validation
    
- Model evaluation
  
- Forecast visualization  

---

## 🎯 Objective

- Understand time-series dataset structure
  
- Perform data preprocessing and normalization
  
- Create sequences for RNN input
  
- Build a SimpleRNN model using TensorFlow/Keras
  
- Evaluate model performance
  
- Forecast future temperature values  

---

## 📂 Dataset Information

Dataset: **Daily Weather Dataset (Kaggle)**  

https://www.kaggle.com/datasets/muthuj7/weather-dataset  

| Feature | Description |
|--------|------------|
| Date | Timestamp |
| Temperature | Target variable |
| Humidity | Atmospheric moisture |
| Wind Speed | Wind velocity |
| Pressure | Atmospheric pressure |

---

## 🧹 Data Preprocessing

- Data exploration
  
- Missing value handling
  
- Feature scaling using **MinMaxScaler**
   
- Sequence creation (7–14 days input)
  
- Train / Validation / Test split  

---

## 🧠 RNN Model Architecture

- Input Layer
  
- SimpleRNN Layer (32–64 units)
  
- Dropout Layer
  
- Dense Output Layer  

---

## ⚙ Model Training

- Batch training
  
- Validation monitoring
  
- Loss curve analysis  

---

## 📊 Model Evaluation

- Mean Absolute Error (MAE)
  
- Root Mean Squared Error (RMSE)
  
- R² Score  

---

## 🔍 Prediction Visualization

- Actual vs Predicted comparison
    
- Trend visualization
  
- Forecast accuracy evaluation  

---

## 🔮 Forecasting

- Predict next **7 days temperature**
  
- Uses recent historical data  

---

## ⚠️ Limitations

- SimpleRNN struggles with long-term dependencies compared to LSTM/GRU
   
- Limited dataset size may affect generalization
  
- External weather factors are not included
  
- Performance may decrease for long-term forecasting
  
- Model depends heavily on data quality  

---

## 🛠 Tech Stack

| Tool | Purpose |
|------|--------|
| Python | Programming |
| TensorFlow / Keras | Deep Learning |
| NumPy | Computation |
| Pandas | Data handling |
| Matplotlib | Visualization |
| Scikit-learn | Preprocessing |
| Kaggle API | Dataset download |
| Google Colab | Development |

---

## 📁 Repository Structure

```
weather-rnn-temperature-prediction/

│
├── DL_Assignment_2_RNN.ipynb

├── README.md

└── DL Assignment 2 - RNN.pdf
```

---

## 🚀 How to Run the Project

### 1️⃣ Install Required Libraries

```bash
pip install tensorflow pandas numpy matplotlib scikit-learn kaggle
```

---

### 2️⃣ Kaggle API Setup & Dataset Download

```bash
mkdir -p ~/.kaggle
cp kaggle.json ~/.kaggle/
chmod 600 ~/.kaggle/kaggle.json

kaggle datasets download -d muthuj7/weather-dataset
unzip weather-dataset.zip
```

---

### 3️⃣ Run the Notebook

- Open notebook in **Google Colab**
 
- Run all cells sequentially
  
- View predictions and visualizations

---

## 📌 Academic Submission

This project was created as part of a **Deep Learning assignment**, demonstrating the implementation of a time-series forecasting model using **Recurrent Neural Networks (RNN)**, including data preprocessing, sequence generation, model training, evaluation, and prediction visualization.

---

## 📌 Future Enhancements

- Implement advanced models like **LSTM and GRU**
- 
- Perform hyperparameter tuning
- 
- Use larger and more diverse datasets
- 
- Integrate real-time weather APIs
  
- Add interactive dashboards  

---

## 👤 Author

**Name:** Laya Mary Joy  

**Organization:** Entri Elevate  

**Date:** March 21, 2026  

---

## ⭐ Acknowledgment

Thanks to **Entri Elevate** for guidance and support.

---
