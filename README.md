# 🏎️ Formula 1 2025 World Champion Prediction

This repository contains two separate approaches to predict the potential winner of the 2025 Formula 1 World Championship.

## 📊 Project Overview

The aim is to estimate the most probable championship-winning driver using two different data sources and modeling techniques:

1. **Machine Learning Model** trained on historical race results (1950–2020)
2. **Ergast API-Based Model** using recent race data from 2021 to 2024

Both models aim to predict which driver has the highest chance of becoming the 2025 world champion.

---

## 🔍 Dataset & API

### 📂 Historical Dataset (ML Model)
- Source: [Formula 1 World Championship (1950–2020) on Kaggle](https://www.kaggle.com/datasets/rohanrao/formula-1-world-championship-1950-2020)
- Used for training a **Random Forest classifier** that estimates each driver's win probability across a simulated 2025 season.

### 🌐 Live Data (API Model)
- Source: [Ergast Developer API](https://ergast.com/mrd/)
- Used to generate predictions based on recent performance trends (2021–2024).

---

## 🧠 Machine Learning Model

The machine learning pipeline includes:
- Dataset merging and preprocessing
- Feature selection: grid position, qualifying times, standings, and more
- Handling missing values and data transformation
- Training a `RandomForestClassifier` to predict individual race winners
- Simulating a full 2025 season and calculating the average win probability per driver

> **Result**: The model outputs a predicted 2025 World Champion.

---

## 🔗 API-Based Model

This model fetches race results from the Ergast API and:
- Collects driver performance statistics from recent seasons
- Calculates win rates and average finishing positions
- Predicts the top-performing driver based on historical consistency and performance

> **Result**: A simpler and data-driven prediction.

---

## 📂 Notebooks

| Notebook | Description |
|----------|-------------|
| `f1_winner_prediction_ML.ipynb` | Machine Learning-based prediction using Kaggle dataset |
| `f1_winner_API_based_model.ipynb` | API-based prediction using Ergast Developer API |

---

## 🚀 How to Use

1. Clone this repository
2. Install required dependencies  
   ```bash
   pip install -r requirements.txt
   ```bash
3. Run each notebook in order to see predictions

---

## 📝 Acknowledgements

- Rohan Rao for the Kaggle dataset
- Ergast API for providing high-quality F1 data

---

## 📢 About

This project was built as a part of my personal exploration into sports analytics and machine learning. Feel free to fork, adapt, or contribute!

Made with ❤️ by Esma 
