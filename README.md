# Sell-A-Car

# Used Car Price Analysis

This repository addresses a critical business question for a dealership client: **What factors make a used car more or less expensive?**

Using Python (`pandas`, `numpy`, `scikit-learn`) and visualizations (`Matplotlib` + `Seaborn` used in-notebook), we model the relationship between vehicle features (age, mileage, brand, condition, etc.) and final sale price to provide a data-driven strategy for inventory optimization.

## 📊 Dataset

  - **Source:** Curated Used Car Dataset.
  - **Size:** 426,000 car listings (reduced from 3 million for speed).
  - **Target Variable (Y):** `price` (US Dollars).
  - **Methodology:** CRISP-DM framework, utilizing Linear, Lasso, and Ridge Regression models.

## ⚡ Quick Findings

  - **Model Performance:** $\text{R}^2 \approx 0.4096$; MAE (Avg. Error) $\approx \$6,941$.
  - **Highest Price Premium:** Manufacturers like **Ferrari, Porsche, and Tesla**.
  - **Significant Factor:** **Electric and Hybrid** fuel types command higher prices.
  - **Value Maximization:** Cars in **'Excellent' or 'Like New'** condition yield the strongest price boost.
  - **Highest Negative Impact:** Standard depreciation driven by **Car Age** and **Odometer Reading**.

**Based on the model coefficients:**

  - **Brand Prestige Matters:** Manufacturers and luxury brands strongly dictate the highest price points. Focus on acquiring these.
  - **Condition is Paramount:** The physical state of the car is a major non-depreciation driver. Investment in reconditioning to 'Excellent' status is highly profitable.
  - **Technology is Trending:** EV and Hybrid vehicles are highly valued by consumers, reflecting a willingness to pay more for newer, fuel-efficient technology.

**Actionable Ideas**

  - **Promote High-Value Inventory:** Focus acquisition funds on high-premium manufacturers and EV/Hybrid fuel types.
  - **Invest in Condition:** Fund aggressive detailing and minor repairs to ensure all viable inventory reaches the 'Excellent' condition category.
  - **Optimize Turnover:** Implement a rapid sales strategy for newer, low-mileage vehicles to minimize depreciation losses.
  - **Next Steps:** Proceed with exploration of **non-linear models** (e.g., XGBoost, LightGBM) to capture complex feature interactions and improve $R^2$ beyond the current 41%.

## 🔗 Link to Notebook: [car\_price\_analysis.ipynb](https://www.google.com/search?q=notebooks/car_price_analysis.ipynb)

## 📁 Project Structure

```
Used-Car-Price-Analysis/
├─ data/
│  ├─ vehicles.csv
├─ images/
│  ├─ price_distribution_histogram.png
│  ├─ numerical_vs_price_scatterplots.png
│  ├─ categorical_features_boxplot_combined.png
│  └─ manufacturer_boxplot_top10.png
├─ notebooks/
│  └─ car_price_analysis.ipynb
├─ requirements.txt
├─ .gitignore
└─ README.md
```

## ▶️ How to Run Locally

1.  Clone or download this repo.
2.  (Recommended) Create a virtual environment.
3.  Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```
4.  Launch Jupyter and open the notebook:
    ```bash
    jupyter notebook notebooks/car_price_analysis.ipynb
    ```
5.  Run all cells to reproduce the analysis and charts.

## 📝 License

MIT (feel free to reuse for learning).
