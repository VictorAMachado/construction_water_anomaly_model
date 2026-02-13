# 💧 Construction Water Consumption Anomaly Analysis

## 📌 Overview

This project analyzes water consumption patterns across multiple construction sites to detect operational inefficiencies such as leaks, abnormal usage, and cost risks.

Using simulated but realistic data, the study models daily consumption by construction phase and applies statistical methods to identify anomalous behavior in one specific tower.

---

## 🎯 Business Problem

Construction projects consume large volumes of water, making inefficiencies difficult to detect without structured monitoring.

Key questions addressed:

- Which sites consume above expected levels?
- Are there abnormal consumption trends over time?
- Can leaks be detected early using data analysis?
- What is the potential operational impact?

---

## 🏗️ Dataset Description

Synthetic dataset representing five construction towers over a 90-day period.

### Features include:

- Tower identification
- Number of floors (structural scale)
- Construction phase (Accelerated, Intermediate, Reduction)
- Daily water consumption (m³)
- Temporal progression
- Simulated noise and leak dynamics

The dataset was generated to reflect realistic operational behavior.

---

## ⚙️ Methodology

### 1. Exploratory Data Analysis (EDA)

- Temporal consumption analysis
- Comparison between towers
- Distribution analysis (boxplots, descriptive statistics)
- Identification of anomalous patterns

---

### 2. Phase-Aware Modeling

Consumption behavior varies by construction stage.

Phases modeled:

- Accelerated phase
- Intermediate phase
- Reduction phase

Segmenting analysis by phase allowed proper baseline comparison.

---

### 3. Statistical Trend Analysis

Linear regression applied within each phase to test for positive consumption trends over time.

Hypothesis tested:

- H₀: No growth trend (β₁ = 0)
- H₁: Positive growth trend (β₁ > 0)

---

### 4. Anomaly Quantification

Consumption in Tower D was benchmarked against peer towers normalized by structural scale (number of floors).

This enabled estimation of excess consumption attributable to abnormal behavior.

---

## 📊 Key Findings

- No significant trend during the accelerated phase (normal operation)
- Statistically significant growth detected in later phases
- Behavior consistent with progressive leakage dynamics

### 🚨 Estimated Impact

- **Excess consumption:** ~393 m³  
- **Deviation from expected:** ~22.15%

This indicates measurable operational inefficiency with financial implications.

---

## 🧠 Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Statsmodels
- Jupyter Notebook

---

## 📈 Potential Extensions

- Integration with real sensor data
- Automated anomaly detection models
- Cost estimation dashboards
- Cloud deployment (Azure / AWS)
- Real-time monitoring systems

---

## 📌 Author

Victor Augusto Machado  
Control & Automation Engineer | Data & Analytics  

---

## 📜 License

This project is for educational and portfolio purposes.
