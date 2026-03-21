# 🌦️ Weather Temperature Prediction using RNN (Deep Learning)

![Python](https://img.shields.io/badge/Python-3.9-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-DeepLearning-orange)
![RNN](https://img.shields.io/badge/Model-RNN-green)
![Platform](https://img.shields.io/badge/Platform-Google%20Colab-yellow)

A deep learning project focused on building and evaluating a **Recurrent Neural Network (RNN)** for **time-series forecasting** using weather data.

---

## 🚀 Run Notebook in Google Colab

Click the button below to open the notebook directly in Google Colab.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1i0i7nBdfW63Q2hr2J2WSoMpHJnEK_rK1)

---

# 📘 Project Overview

This project implements a **SimpleRNN model** to predict future temperature values based on historical weather data.

The project covers the complete deep learning pipeline including:

- Dataset exploration  
- Time-series preprocessing  
- Sequence generation  
- RNN model design  
- Model training and validation  
- Model evaluation using regression metrics  
- Forecast visualization  

The goal is to build a **robust RNN model capable of capturing temporal patterns in weather data**.

---

# 🎯 Objective

The main objectives of this project are:

🔹 Understand time-series dataset structure  
🔹 Perform data preprocessing and normalization  
🔹 Create sequences for RNN input  
🔹 Build a SimpleRNN model using TensorFlow/Keras  
🔹 Evaluate model performance using regression metrics  
🔹 Forecast future temperature values  

---

# 📂 Dataset Information

The dataset used is the **Daily Weather Dataset** available on Kaggle.

Dataset Link:  
https://www.kaggle.com/datasets/muthuj7/weather-dataset

### Dataset Details

| Feature | Description |
|------|-------------|
| Date | Timestamp |
| Temperature | Target variable |
| Humidity | Atmospheric moisture |
| Wind Speed | Wind velocity |
| Pressure | Atmospheric pressure (optional) |

---

# 🧹 Data Preprocessing

Before training the RNN model, several preprocessing steps were applied:

### ✔ Data Exploration
- Displayed initial rows  
- Plotted temperature trends over time  

### ✔ Missing Value Handling
- Checked and handled missing values  

### ✔ Feature Scaling
- Used **MinMaxScaler** to normalize values between 0 and 1  

### ✔ Sequence Creation
- Used past **7–14 days** as input sequences  
- Target: **Next day temperature**  

### ✔ Train / Validation / Test Split

The dataset was split into:

- Training Set  
- Validation Set  
- Test Set  

---

# 🧠 RNN Model Architecture

A **SimpleRNN model** was built using **TensorFlow / Keras**.

### Architecture Components

✔ Input Layer (sequence data)  
✔ SimpleRNN Layer (32–64 units)  
✔ Dropout Layer for regularization  
✔ Dense Layer (1 neuron for output)  

---

# ⚙ Model Training

The RNN model was trained using the **training dataset** and validated using the **validation dataset**.

### Training Techniques Used

- Batch Training  
- Validation Monitoring  
- Loss Curve Analysis  

Training progress was monitored using:

- Training Loss vs Validation Loss  

---

# 📊 Model Evaluation

After training, the model was evaluated using the **test dataset**.

### Evaluation Metrics

- Mean Absolute Error (MAE)  
- Root Mean Squared Error (RMSE)  
- R² Score  

---

# 🔍 Prediction Visualization

To better understand the model’s performance:

- Compared **actual vs predicted temperatures**  
- Visualized prediction trends  
- Evaluated forecasting accuracy  

---

# 🔮 Forecasting

- Predicted **next 7 days temperature**  
- Used recent historical data as input  
- Visualized future predictions  

---

# 🛠 Tech Stack

| Tool | Purpose |
|----|----|
| Python | Programming language |
| TensorFlow / Keras | Deep learning framework |
| NumPy | Numerical computation |
| Pandas | Data handling |
| Matplotlib | Visualization |
| Scikit-learn | Preprocessing & metrics |
| Kaggle API | Dataset download |
| Google Colab | Development environment |

---

# 📁 Repository Structure
 weather-rnn-temperature-prediction/
│
├── DL_Assignment_2_RNN.ipynb
├── README.md
└── DL Assignment 2 - RNN.pdf


---

# 🚀 How to Run the Project

### 1️⃣ Open the Notebook

Click the **Google Colab button above**.

---

### 2️⃣ Install Required Libraries

```python
pip install tensorflow pandas numpy matplotlib scikit-learn kaggle

# Kaggle API Setup + Download Dataset

!mkdir -p ~/.kaggle && \
cp kaggle.json ~/.kaggle/ && \
chmod 600 ~/.kaggle/kaggle.json && \
kaggle datasets download -d muthuj7/weather-dataset && \
unzip weather-dataset.zip
