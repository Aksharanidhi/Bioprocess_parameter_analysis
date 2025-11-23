# 📊 Correlation Analysis of Penicillin Fermentation Parameters

## 📌 Project Overview
This project explores how different bioprocess parameters influence **penicillin production** using exploratory data analysis (EDA), correlation mapping, and visualization techniques.  
The goal is to identify which variables have the strongest relationship with **Penicillin concentration (g/L)** and understand patterns within a fermentation dataset.

---

## 🔬 Project Objectives
- Analyze fermentation parameters and their statistical relationships
- Identify key drivers influencing penicillin concentration
- Visualize relationships using correlation heatmaps, scatter plots, and scatter plot grids
- Compare online sensor data with offline lab measurements
- Interpret findings from a bioprocess engineering perspective

---

## 📁 Dataset Description
The project uses **two datasets** capturing the penicillin fermentation process:

1. **Online Dataset:**  
   - Real-time measurements collected continuously during fermentation  
   - Examples: DO concentration (mg/L), Temperature (K), Time (h), Carbon Evolution Rate (g/h), Aeration, Air Pressure, Oxygen Uptake Rate, Sugar Feed, Base/Acid flow

2. **Offline Dataset (Lab Measurements):**  
   - Lab measurements collected at specific sampling points  
   - Examples:  
     - **Offline Penicillin Concentration (g/L)**  
     - **Offline Biomass Concentration (g/L)**  
     - **Offline Viscosity (cP)**  

> Offline measurements serve as the **ground-truth values** for validating online sensor data.

---

## 🛠️ Methods Used
- Data cleaning and preprocessing  
- Correlation matrix + heatmap (**Seaborn**)  
- Individual scatter plots (**Matplotlib**)  
- Combined scatter plot grid showing all parameters vs Penicillin (**Matplotlib**)  

> Seaborn was used for the correlation heatmap due to its easy-to-read, visually appealing style. Matplotlib was used for custom scatter plots and grid visualizations.

---

## 📈 Visualizations Included
### ✔ Correlation Heatmap  
Shows positive and negative relationships between all variables.

### ✔ Individual Scatter Plots  
- Penicillin vs DO  
- Penicillin vs Temperature  

### ✔ Scatter Plot Grid  
A single figure containing small scatter plots for **Penicillin vs each process parameter**, including both online and offline measurements.  
This provides a **comprehensive view of relationships** across the dataset.

---

## 🔍 Key Findings
### Strong Positive Correlations:
- Time  
- Carbon Evolution Rate (CER)  
- Biomass concentration  
- DO concentration  
- Aeration & Air Pressure  
- Oxygen Uptake Rate  

These variables **increase as penicillin increases**, indicating strong process drivers.

### Negative Correlations:
- Temperature (weak negative)  
- Substrate concentration (moderate negative)  

Indicating conditions where penicillin biosynthesis is slightly reduced.

### No Correlation:
- pH  
- Acid/Base flow  
- Agitator rpm (constant → NaN correlation)

### Interpretation:
Penicillin production is strongly linked to **oxygen transfer and fermentation duration**, which aligns with known aerobic secondary metabolite pathways.

---
