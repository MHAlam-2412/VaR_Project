# VaR_Project

# Monte Carlo Value at Risk (VaR) & Expected Shortfall in C++

A **simulation-based financial risk model** that computes **Value at Risk (VaR)** and **Expected Shortfall (ES)** using **Monte Carlo methods** assuming normally distributed returns.

This project is useful for **risk management**, **portfolio analysis**, and **FRM / quant finance learning**.

---

## 📌 Features

- Reads **historical returns** from a dataset (single column)
- Computes:
  - Mean return
  - Standard deviation
- Generates **Monte Carlo simulations** using a normal distribution
- Calculates:
  - **Value at Risk (VaR)**
  - **Expected Shortfall (ES)**
- Fully written in **C++ (STL based)**

---

## 📂 Input Requirements

- A text file containing **one column of numerical returns**
- Example:
-0.012
-0.008
-0.004
-0.015


---

## ⚙️ How It Works

1. User provides the **absolute path** of the dataset  
2. Program reads and stores historical returns  
3. Computes **mean** and **standard deviation**  
4. Runs **Monte Carlo simulations** using:
5. Sorts simulated returns  
6. Calculates:
- VaR at chosen confidence level  
- Expected Shortfall beyond VaR  

---

## 🧮 Mathematical Background

- **VaR (α%)**  
The loss threshold such that only `(100 − α)%` outcomes are worse.

- **Expected Shortfall (ES)**  
The **average loss beyond the VaR threshold**, capturing tail risk.

---

## ▶️ How to Run

### Compile
```bash
g++ var_simulation.cpp -o var_simulation
./var_simulation

```
Value at Risk (VaR) at 95% confidence level: -0.0234
Expected Shortfall (ES) at 95% confidence level: -0.0312
Simulation completed.
----------------------------------------------------
Author

Md Hamid Alam
B.Tech IIT Patna | Data Structures & algorithm |Quantitative Finance & Risk Modeling|Machine Learning Engineering 

