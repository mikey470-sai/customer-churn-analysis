# 📊 Telecom Customer Churn Analysis

A data analysis project that explores customer churn patterns in a telecom dataset using Python. The notebook performs end-to-end EDA (Exploratory Data Analysis), feature engineering, visualization, and business insight generation.

---

## 📁 Dataset

- **File:** `telecom_churn_csv.csv`
- **Target Variable:** `Churn` — whether a customer has left the service
- **Key Features Used:** `tenure`, `Contract`, `MonthlyCharges`

---

## 🛠️ Technologies Used

| Library | Purpose |
|---|---|
| `pandas` | Data loading and manipulation |
| `numpy` | Numerical operations |
| `matplotlib` | Plotting and visualization |
| `seaborn` | Statistical visualizations |

---

## 🔍 Project Workflow

### 1. Data Loading & Inspection
- Load dataset from CSV
- Inspect shape, data types, and null values using `df.info()`, `df.describe()`, and `df.isnull().sum()`

### 2. Feature Engineering
- **TenureGroup**: Customers are bucketed into tenure bands — `0-3`, `4-12`, `13-24`, `25-48`, `49-60`, `61-72` months
- **ContractType**: Contract labels are simplified to `Monthly`, `Annual`, and `Biennial`

### 3. Exploratory Data Analysis (EDA)

The following visualizations are generated:

- **Churn Count** — Overall distribution of churned vs. retained customers
- **Churn by Tenure Group** — How churn varies across different tenure bands
- **Churn by Contract Type** — Churn rates for Monthly, Annual, and Biennial contracts
- **Monthly Charges vs Churn** — Boxplot comparing charges for churned vs. retained customers
- **Distribution of Monthly Charges** — Histogram of charge spread across all customers
- **Correlation Heatmap** — Pearson correlations among all numeric features

### 4. Churn Analysis
- Calculate overall churn percentage
- Break down churn rate by `ContractType` and `TenureGroup` combination

### 5. Key Insights
- 🚨 A significant portion of churned users are on **Monthly contracts with less than 3 months of tenure**
- 💡 Recommendation: Improve **early engagement strategies** to retain new customers

---

## 🚀 Getting Started

### Prerequisites

```bash
pip install pandas numpy matplotlib seaborn
```

### Run the Notebook

```bash
jupyter notebook Untitled1__2_.ipynb
```

Make sure `telecom_churn_csv.csv` is placed in the same directory as the notebook before running.

---

## 📌 Folder Structure

```
.
├── Untitled1__2_.ipynb       # Main analysis notebook
├── telecom_churn_csv.csv     # Dataset (required)
└── README.md                 # Project documentation
```

---

## 📈 Sample Insights

| Segment | Churn Insight |
|---|---|
| Monthly Contract + 0–3 months tenure | Highest churn risk group |
| Biennial Contract | Lowest churn rate |
| High Monthly Charges | Correlated with higher churn likelihood |

---

## 🤝 Contributing

Feel free to fork this repository, improve the analysis, or add machine learning models on top of the EDA.

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
