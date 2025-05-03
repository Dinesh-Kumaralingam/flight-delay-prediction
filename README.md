# NYC Flight Delay Prediction

Predict flight arrival delays for New York City’s major airports (JFK, LGA, EWR) using 2013 flight data. This repository contains end-to-end analysis: data cleaning, EDA, feature engineering, model training (Multiple Linear Regression & Random Forest), and performance comparison.

## 🚀 Features

* **Data Preparation & Cleaning**: Handle missing values, outliers, and format consistency.
* **Exploratory Data Analysis (EDA)**: Histograms, word clouds, correlation matrices, geospatial insights.
* **Feature Engineering**: Temporal variables, distance metrics, weather integration, carrier & airport flags.
* **Modeling**:

  * Multiple Linear Regression (MLR) with interpretability.
  * Random Forest Regression (RFR) for non-linear patterns.
* **Evaluation**: RMSE, MAE, MSE, R² comparisons.
* **Reproducibility**: Fixed random seed, clear preprocessing pipeline.

## 📂 Repository Structure

```
├── data/                  # Raw and cleaned datasets
│   ├── flights.csv
│   ├── weather.csv
│   └── ...
├── notebooks/             # Jupyter notebooks for analysis and modeling
│   ├── 01_data_cleaning.ipynb
│   ├── 02_eda.ipynb
│   └── 03_modeling.ipynb
├── src/                   # R scripts and helper functions
│   └── utils.R
├── results/               # Figures, tables, and model outputs
├── README.md              # Project overview and instructions
└── requirements.txt       # R package dependencies
```

## 📦 Installation

1. Clone this repo:

   ```bash
   git clone https://github.com/your-username/nyc-flight-delay-prediction.git
   cd nyc-flight-delay-prediction
   ```
2. Install R packages:

   ```r
   install.packages(c("tidyverse","nycflights13","caret","randomForest","wordcloud","RColorBrewer","GGally","Metrics","lubridate"))
   ```
3. Open the R Markdown report (`final_report.Rmd`) or run notebooks.

## 📈 Usage

* **Run full analysis**: Knit `final_report.Rmd` to generate PDF/HTML report.
* **Reproduce models**: Execute scripts in `notebooks/03_modeling.ipynb`.
* **View results**: Check `results/` for plots and metrics.

## 🎯 Key Results

* **MLR Performance**: RMSE = 15.46 min, R² = 0.8711
* **RFR Performance**: RMSE = 17.29 min, R² = 0.822
* **Top Predictor**: Departure delay has the highest impact on arrival delay.

## 🔮 Future Work

* Integrate real-time weather and air traffic data.
* Test gradient boosting and deep-learning regressors.
* Deploy model as a REST API for live delay predictions.

## 👤 Author

**Dinesh Kumaralingam** ([dkuma026@ucr.edu](mailto:dkuma026@ucr.edu))
MS Business Analytics, UC Riverside

---

*Feel free to explore and adapt this pipeline for your own flight-delay prediction tasks.*
