

# 📊 Time Series Analysis and Chaos Detection

This repository contains multiple tasks related to time series analysis, chaos detection, predictive clustering, noise filtering, and forecasting. Each task involves different algorithms and techniques to analyze, visualize, and interpret various types of time series data.

---

## Table of Contents

1. [Lorenz and Logistic Map Chaos Analysis](#lorenz-and-logistic-map-chaos-analysis)
2. [Entropy-Complexity Plane](#entropy-complexity-plane)
3. [Predictive Clustering with Healing](#predictive-clustering-with-healing)
4. [Fourier Filtering and ARIMA Forecasting](#fourier-filtering-and-arima-forecasting)
5. [How to Run the Code](#how-to-run-the-code)
6. [Dependencies](#dependencies)
7. [Results Summary](#results-summary)

---

## 1. Lorenz and Logistic Map Chaos Analysis

This task estimates the **Largest Lyapunov Exponent (LLE)** for the Lorenz system and the logistic map using **Rosenstein's method**. Positive LLE values indicate chaotic behavior.

### 📈 Key Outputs

- **Lorenz System LLE**: 0.02321
- **Logistic Map LLE**: 0.69288

### 🔹 Lorenz System Plot
![Lorenz Plot](image.png)

### 🔹 Logistic Map Plot
![Logistic Map Plot](image.png)

---

## 2. Entropy-Complexity Plane

This task calculates the **entropy-complexity pairs** for various time series, including chaotic systems and noise.

### Time Series Analyzed

1. **Lorenz System**
2. **Henon Map**
3. **Skew Tent Map**
4. **Logistic Map**
5. **Schuster Map**
6. **White Noise**
7. **Regular Time Series**

### 🔹 Entropy-Complexity Plane Plot
![Entropy Complexity Plot](image.png)

### Key Results

| **Time Series** | **Entropy (H)** | **Complexity (C)** | **Type**          |
|-----------------|-----------------|--------------------|-------------------|
| Lorenz          | 0.4515          | 0.2731             | Chaotic           |
| Logistic        | 0.8619          | 0.1456             | Chaotic           |
| White Noise     | 0.9999          | 0.0001             | Random            |
| Regular         | 0.3916          | 0.2715             | Periodic          |

---

## 3. Predictive Clustering with Healing

This task applies **K-Means** and **Agglomerative Clustering** to predict chaotic time series and uses a **healing algorithm** to correct outliers.

### 🔹 Results Plot
![Predictive Clustering Plot](image.png)

### Key Metrics

| **Metric**            | **K-Means** | **Agglomerative** |
|------------------------|-------------|------------------|
| **MSE Before Healing**| 1.1734      | 1.3372           |
| **MSE After Healing** | 0.8801      | 0.9631           |
| **Unpredictable Points** | 404      | 418              |

---

## 4. Fourier Filtering and ARIMA Forecasting

This task involves:

1. **Fourier Analysis** to denoise a signal.
2. **ARIMA** model for time series forecasting.

### 🔹 Fourier Filtering Plot
![Fourier Filtering Plot](image.png)

### 🔹 ARIMA Forecast Plot
![ARIMA Forecast Plot](image.png)

### ARIMA Model Summary

- **ADF Test**: The time series was non-stationary and required differencing.
- **Model**: ARIMA(2, 1, 2)

| **Metric** | **Value**     |
|------------|---------------|
| AIC        | 539.361       |
| BIC        | 555.827       |

---

## 5. Dependencies

- **Python 3.8+**
- **NumPy**
- **Matplotlib**
- **SciPy**
- **scikit-learn**
- **statsmodels**
- **ordpy**
- **tqdm**

Install all dependencies with:

```bash
pip install numpy matplotlib scipy scikit-learn statsmodels ordpy tqdm
```

---

## 6. Results Summary

This project demonstrates:

- **Chaos Analysis** using the Lorenz and Logistic maps.
- **Entropy-Complexity Characterization** for different time series.
- **Predictive Clustering** with a healing mechanism for better forecasting.
- **Noise Filtering** using Fourier analysis.
- **Time Series Forecasting** with the ARIMA model.
