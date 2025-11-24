---
layout: page
title: "Predicting Air Quality Levels Using Environmental & Weather Data"
permalink: /projects/aqi-prediction/
---

# Predicting Air Quality Levels Using Environmental & Weather Data

![AQI Feature Importance](../assets/img/aqi-feature-importance.png)

[![Python](https://img.shields.io/badge/Python-Data%20Science-blue.svg)]()
[![Random Forest](https://img.shields.io/badge/Model-Random%20Forest-brightgreen.svg)]()
[![EPA AQS](https://img.shields.io/badge/Data-EPA%20AQS-lightgrey.svg)]()

This project predicts daily **Air Quality Index (AQI)** using pollutant concentrations and weather data from EPA AQS and NOAA NCEI APIs. 

## 🎯 Goals

1. Predict AQI from environmental and meteorological inputs  
2. Identify the most influential variables driving poor air quality  
3. Explore seasonal and regional patterns  

## 🧰 Tech Stack

- Python (Pandas, NumPy)
- Random Forest Regressor
- Matplotlib / Seaborn
- APIs: EPA AQS, NOAA NCEI

## 📊 Methods

- API-based data collection  
- Merge pollutant + weather data on date & location  
- Imputation of missing values  
- Encoding regional/city variables  
- Random Forest modeling and feature importance  

## 🔥 Key Results

- Random Forest achieved **R² ≈ 0.82** on test data.   
- Top predictors: **PM2.5**, **temperature**, **wind speed**. :contentReference[oaicite:14]{index=14}  
- Strong seasonal variation and clear regional differences in AQI.   

## 📂 Repository

- *(Add your AQI project repo link here)*

## 📄 Supporting Docs

- Final AQI white paper  
- Final presentation slides
