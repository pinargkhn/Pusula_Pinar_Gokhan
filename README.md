# Pusula_Pinar_Gokhan  
**Email:** pinar.gkhn1@gmail.com  

**Data Science Intern Case Study – Exploratory Data Analysis and Preprocessing on a Physical Medicine & Rehabilitation Dataset**

---

## Overview  

This repository contains my solution for the **Data Science Intern Case Study**.  
The project is based on a **physical medicine & rehabilitation dataset** with **2235 observations** and **13 features**.  

The main objective is to perform **Exploratory Data Analysis (EDA)** and **Data Preprocessing** to make the dataset ready for predictive modeling.  
No model training is required — the focus is on **cleaning, structuring, and transforming** the data into a model-ready format.  

---

## Dataset  

**Target variable:** `TedaviSuresi` (treatment duration in sessions)  

**Features:**  
- **HastaNo** — Anonymized patient ID  
- **Yas** — Age  
- **Cinsiyet** — Gender  
- **KanGrubu** — Blood type  
- **Uyruk** — Nationality  
- **KronikHastalik** — Chronic conditions (multi-valued)  
- **Bolum** — Department/Clinic  
- **Alerji** — Allergies (multi-valued)  
- **Tanilar** — Diagnoses  
- **TedaviAdi** — Treatment name  
- **TedaviSuresi** — Treatment duration (target)  
- **UygulamaYerleri** — Application sites (multi-valued)  
- **UygulamaSuresi** — Application duration  

---

## Tasks Completed  

### 1. Exploratory Data Analysis (EDA)  
- Inspected dataset structure, variable types, and anomalies  
- Checked missing values and duplicates  
- Created visualizations:  
  - Histograms for numeric distributions  
  - Correlation heatmap of numeric variables  
  - Scatter plot: Age vs Treatment Duration  
  - Boxplots by department  

### 2. Data Preprocessing  
- Extracted numeric values from `TedaviSuresi` and `UygulamaSuresi`  
- Normalized text fields (gender, blood group, department names, etc.)  
- Split multi-valued columns into lists and created **count + multi-hot encoded features**  
- Handled missing values using **SimpleImputer** (median for numeric, most frequent for categorical)  
- Treated outliers with **IQR capping**  
- Checked and removed potential duplicate rows  
- Prepared final **model-ready datasets** (`model_ready.csv` and `model_matrix.csv`)  

---

## Project Structure

```text
├── 01_EDA.ipynb                 # Exploratory Data Analysis
├── 02_Preprocessing.ipynb       # Data cleaning & preprocessing
├── EDA_Preprocessing_Report.pdf # Summary report
├── data/
│   ├── Talent_Academy_Case_DT_2025.csv  # Raw dataset
│   ├── model_ready.csv                  # Clean dataset
│   └── model_matrix.csv                 # Final model matrix
└── README.md

---
## How to Run

Clone the repository and open the notebooks in **Jupyter**:

```bash
git clone https://github.com/pinargkhn/Pusula_Pinar_Gokhan.git
cd Pusula_Pinar_Gokhan
jupyter notebook



## Dependencies

All dependencies are listed in the notebooks’ first cells (**pandas, numpy, matplotlib, seaborn, scikit-learn, packaging**).  
You can install them with:


pip install pandas numpy matplotlib seaborn scikit-learn packaging



