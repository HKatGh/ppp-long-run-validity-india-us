# ppp-long-run-validity-india-us
# 📊 Evaluating Long-Run Validity of Purchasing Power Parity (PPP): India vs. United States

## 📌 Project Overview

This project empirically investigates the **long-run validity of Purchasing Power Parity (PPP)** between **India and the United States** using monthly macroeconomic data from **2015 to 2025**. The study applies **time-series econometric techniques** to test whether deviations from PPP are mean-reverting, as predicted by economic theory.

The analysis combines **AR(1) modeling**, **unit-root testing**, and **structural break analysis** to assess PPP validity across the full sample and across sub-periods.

---

## 🎯 Objectives

* Construct the **real exchange rate** using nominal USD/INR exchange rate and CPI data
* Test the **stationarity** of the real exchange rate implied by PPP
* Estimate **mean-reversion dynamics** using AR(1) models
* Compute the **half-life of PPP deviations**
* Identify **structural breaks** and re-evaluate PPP validity across regimes

---

## 📂 Data Description

* **Exchange Rate:** USD/INR (monthly)
* **Price Levels:** Consumer Price Index (CPI) for India and the U.S.
* **Source:** Federal Reserve Economic Data (FRED)
* **Frequency:** Monthly
* **Period:** 2015–2025

The real exchange rate is constructed as:

[
q_t = \ln(E_t) + \ln(P_t^{US}) - \ln(P_t^{India})
]

where:

* (E_t) = nominal exchange rate (USD/INR)
* (P_t) = CPI levels

---

## 🧠 Methodology

### 1️⃣ AR(1) Time-Series Model

The real exchange rate is modeled as:

[
q_t = \alpha + \rho q_{t-1} + \varepsilon_t
]

Mean reversion exists if (|\rho| < 1).

---

### 2️⃣ Unit-Root Testing (ADF Test)

* Augmented Dickey–Fuller tests are used to test for stationarity
* Null hypothesis: Presence of unit root (PPP does not hold)

---

### 3️⃣ Half-Life Estimation

The speed of convergence toward PPP is measured by the **half-life**:

[
\text{Half-life} = \frac{\ln(0.5)}{\ln(\rho)}
]

This estimates the time required for half of a PPP deviation to dissipate.

---

### 4️⃣ Structural Break Analysis

* Structural breaks are identified to account for macroeconomic disruptions
* PPP validity is re-tested across segmented sub-periods
* Model selection is guided using **AIC / BIC**

---

## 📈 Key Findings

* Full-sample results show **weak evidence** of strict long-run PPP
* Sub-period analysis reveals **stronger mean-reversion** in certain regimes
* Estimated half-lives indicate **slow but economically meaningful convergence**
* Overall results support **partial and regime-dependent PPP validity**

---

## 🛠️ Tools & Techniques

* AR(1) Time-Series Modeling
* Augmented Dickey–Fuller (ADF) Test
* Structural Break Analysis
* Half-Life Estimation
* AIC / BIC Model Selection
* Hypothesis Testing
* Data Source: **FRED**

---

## 🧪 Technologies Used

* Python
* NumPy
* Pandas
* Statsmodels
* Matplotlib / Seaborn
* Jupyter Notebook

---

## 📁 Repository Structure

```
├── data/
│   └── raw_fred_data.csv
├── notebooks/
│   ├── data_cleaning.ipynb
│   ├── ppp_model_estimation.ipynb
│   └── structural_break_analysis.ipynb
├── results/
│   ├── plots/
│   └── tables/
├── README.md
└── requirements.txt
```

---

## 🚀 How to Run the Project

### Clone the repository

```bash
git clone https://github.com/your-username/ppp-long-run-validity-india-us.git
cd ppp-long-run-validity-india-us
```

### Install dependencies

```bash
pip install -r requirements.txt
```

### Run analysis

Open Jupyter Notebook and execute notebooks in the `notebooks/` folder.

---

## 📌 Applications

* Applied Macroeconomics
* International Finance
* Econometrics & Time-Series Analysis
* Quantitative Research
* Policy Analysis

---

## 👤 Author

**Himanshu Kushwaha**
BS Economics, IIT Patna
Interests: Econometrics, Quantitative Finance, Time-Series Modeling

---

## 📜 License

This project is for **academic and research purposes**.



