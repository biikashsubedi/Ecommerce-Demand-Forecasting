# 🛒 E-Commerce Dynamic Pricing AI Engine

> A hybrid machine learning architecture that optimizes retail pricing by combining predictive demand forecasting with strict business margin rules.

## 📊 Executive Summary
The rapid growth of e-commerce requires intelligent, real-time pricing systems that go beyond the limitations of manual price-setting. This project serves as a Proof-of-Concept (PoC) for a Dynamic Pricing Engine designed for a mid-sized e-commerce marketplace. 

By analyzing categorical, numerical, and temporal features (including product pricing, inventory levels, competitor pricing, and weather conditions), the system identifies the exact price point that maximizes revenue without violating minimum profit margins.

## ✨ Hybrid AI Architecture
Unlike purely statistical or deep learning methods that struggle with market volatility, this system utilizes a **Hybrid AI Architecture**:
1. **Layer 1: Deterministic Rule Engine:** Enforces "Hard Rules" such as cost floors and minimum margin constraints to ensure the AI never suggests a financially damaging price.
2. **Layer 2: Demand Forecasting (LightGBM):** A highly optimized LightGBM machine learning model predicts `Units Sold` by evaluating historical signals, competitor actions, and time-series memory features (e.g., `rolling_mean_7`).
3. **Layer 3: Pricing Optimizer:** A revenue-maximizing algorithm that simulates demand across a spectrum of possible price points to select the ultimate optimal price.

## 🛠️ Tech Stack
* **Language:** Python
* **Machine Learning:** LightGBM, Scikit-Learn
* **Data Processing:** Pandas, NumPy
* **Evaluation:** Time-series-aware walk-forward cross-validation.

## 💡 Strategic Business Impact
The technical validation of the PoC confirms that high-performance forecasting can be safely integrated with automated price adjustments. System simulations indicate that deploying this architecture in high-impact categories (like Electronics and Groceries) could capture a projected **8-12% revenue lift** while strictly enforcing a minimum margin floor.

---

## 📥 Download & Run

If you prefer to explore this project locally, you can easily download the project files:

1. **[Download the Project ZIP](https://github.com/biikashsubedi/Ecommerce-Demand-Forecasting/archive/refs/heads/main.zip)** 2. Extract the folder to your local machine.
3. Open the folder in your preferred code editor or Jupyter environment.
4. Review the full architectural documentation in `Dynamic-Pricing-Blueprint.pdf`.
5. Install the required dependencies (`lightgbm`, `pandas`, `scikit-learn`) and run the `Dynamic-Pricing-Optimization.ipynb` notebook.
