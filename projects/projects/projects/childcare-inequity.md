---
layout: page
title: "Childcare Cost Inequity in the United States"
permalink: /projects/childcare-inequity/
---

# Childcare Cost Inequity in the United States

![Childcare Map](../assets/img/childcare-map.png)

[![Excel](https://img.shields.io/badge/Tool-Excel-green.svg)]()
[![Python](https://img.shields.io/badge/Python-EDA-blue.svg)]()
[![Policy](https://img.shields.io/badge/Focus-Policy%20Analysis-purple.svg)]()

This project examines **county-level childcare costs** across the U.S. using the National Database of Childcare Prices and CPI data to understand affordability and equity. 

## 🧩 Problem

Childcare costs often exceed affordability benchmarks, especially for infant care and for low- to moderate-income families. Policymakers need clear data to guide subsidies and reforms.

## 🧰 Tech Stack

- Excel (cleaning, pivot tables, charts)
- Python (data prep & demo pipeline)
- CPI adjustment
- Tableau / visualization tools (optional)

## 🔎 Methods

- Cleaned and structured county-level childcare data (2008–2018)  
- CPI-adjusted costs to real terms  
- Compared:
  - **FCC vs. CCC**
  - **Urban vs. rural**
  - **Age groups (infant, toddler, preschool)**  
- Calculated **income burden (% of median household income)**  

## 📊 Key Findings

- Infant care is consistently the most expensive across regions. :contentReference[oaicite:7]{index=7}  
- Urban counties often have childcare costs ~50% higher than rural areas.   
- CCC is typically 20–30% more expensive than FCC.   
- In some counties, families spend **>30%** of income on infant care.   

## 🧪 Full Demo Pipeline

I also built a **self-contained Python script** that:

- Validates schema  
- Performs CPI adjustment  
- Computes income burden  
- Builds summary tables  
- Exports clean CSVs, Excel outputs, and PNG charts :contentReference[oaicite:11]{index=11}  

## 📂 Repositories

- Analysis & demo script: *(add your childcare repo link here)*

## 📄 Supporting Docs

- Milestone 1 proposal  
- Milestone 2 white paper  
- Milestone 3 findings & Q&A  
- `childcare_analysis_full_demo.py` (full pipeline)
