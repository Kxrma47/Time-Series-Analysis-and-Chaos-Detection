

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


![image](https://github.com/user-attachments/assets/6a41e753-532f-4323-a653-f1d98ab05d32)

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

![image](https://github.com/user-attachments/assets/4a2e2a08-0a07-408a-b59f-8b118aff3872)

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

![image](https://github.com/user-attachments/assets/d1b11f21-fcd9-4652-a411-d37db1d51744)

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
![image](https://github.com/user-attachments/assets/591b20ad-f56e-43e3-a3a4-fc6e6f1dd0a7)
![image](https://github.com/user-attachments/assets/de737f03-8fc1-4278-a8ab-c19b191b2bea)
![image](https://github.com/user-attachments/assets/ddac804c-795b-4529-b82b-fd07cee5ff08)
![image](https://github.com/user-attachments/assets/a60ffe95-3416-40fd-94f4-07216a94ec8d)
![image](https://github.com/user-attachments/assets/cf3ea435-ec05-4974-9bc1-abfccb9d9c1d)




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
