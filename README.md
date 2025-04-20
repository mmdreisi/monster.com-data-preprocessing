# 🧠 Job Salary Analysis using Machine Learning

This notebook performs a data analysis and preprocessing pipeline on a sample dataset of job advertisements from Monster.com. The goal is to prepare and clean the dataset to be used for further salary prediction or clustering tasks.

---

## 📁 Dataset

- **Source**: `monster_com-job_sample.csv`
- **Features**: Includes job title, organization, job type, salary, and other metadata.
- **Target**: Clean and standardize salary field for ML-ready dataset.

---

## 🔧 Workflow

1. **Exploratory Data Analysis (EDA)**  
   Basic info, descriptive stats, shape, and missing values

2. **Data Cleaning**  
   - Dropped irrelevant columns like `page_url`, `location`, `uniq_id`
   - Cleaned salary column and converted hourly/yearly to annual salary
   - Dropped unusable text-heavy fields

3. **Feature Engineering**  
   - Used `OrdinalEncoder` to encode categorical features
   - Applied regex and logic to normalize salary values
   - Imputed missing values using `KNNImputer`

4. **Data Ready for ML**  
   Cleaned and normalized dataset is ready for clustering or salary prediction tasks.

---

## 📊 Possible Next Steps

- Use `KMeans` or `DBSCAN` for job clustering based on features
- Apply regression models to predict salary
- Visualize salary distribution by job sector/type

---

## 📌 Requirements

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

---

## 💡 Author

Made with ❤️ by Mohammad
