# Titanic Dataset - Exploratory Data Analysis (EDA)

This project is part of the AI & ML Internship task to perform Exploratory Data Analysis (EDA) using the Titanic dataset.

---

## 📌 Objective

The main goal is to explore the Titanic dataset using Python libraries and identify patterns, trends, and insights through visualization and statistics.

---

## 📂 Dataset

- Source: [Kaggle - Titanic Dataset](https://www.kaggle.com/datasets/yasserh/titanic-dataset)
- Format: CSV

---

## 🛠 Tools Used

- Python
- Pandas
- Seaborn
- Matplotlib

---

## 📊 Steps Performed

### 1. Data Loading
- Loaded dataset using `pandas.read_csv()`
- Displayed the first few rows using `df.head()`

### 2. Summary Statistics
- Used `.describe()` and `.info()` to get basic statistics (mean, std, count, etc.)
- Checked for missing values with `df.isnull().sum()`

### 3. Data Visualization
- **Histograms**: Distribution of Age, Fare, etc.
- **Boxplots**: To detect outliers in numeric columns
- **Pairplot**: To explore relationships between features
- **Heatmap**: Correlation between numeric features

```python
numeric_df = df.select_dtypes(include='number')
sns.heatmap(numeric_df.corr(), annot=True, cmap='coolwarm')
