# 🚗 Cars Dataset Analysis  

Exploratory Data Analysis (EDA) of the **Cars Dataset** with 428 entries and 15 features.  
This project covers data cleaning, feature engineering, exploratory analysis, visualizations, and insights.  

---

## 📂 Dataset Overview  

The dataset contains both categorical and numerical features:  

- **Categorical**: Make, Model, Type, Origin, DriveTrain  
- **Numerical**: MSRP, Invoice, Engine Size, Cylinders, Horsepower, MPG (City & Highway), Weight, Wheelbase, Length  

**Shape**: 428 rows × 15 columns  
![Dataset Preview](https://github.com/Awais11227/Cars_Dataset_Analysis/blob/main/1.png?raw=true)

---

## 🧹 Data Cleaning  

Steps taken to prepare the dataset:  
- Handled missing values (Cylinders filled with median).  
- Removed duplicates.  
- Standardized categorical columns (`Type`, `Origin`, `DriveTrain`).  
- Converted categorical data types.  
- Detected and treated outliers using Z-scores and boxplots.  

---

## 🛠 Feature Engineering  

Created additional columns to enrich the dataset:  
- **Price_Difference** = MSRP – Invoice  
- **Efficiency_Ratio** = Highway MPG / City MPG  
- **HP_Category** = Low, Medium, High (based on horsepower bins)  

---

## 🔍 Exploratory Data Analysis  

Analysis included:  
- **Groupby** for comparing regions (Asia, Europe, USA)  
- **Crosstabs** for DriveTrain and Type distribution  
- **Descriptive statistics** for numeric variables  
- **Z-scores** for outlier detection  

---

## 🎨 Visualizations  

1. **Dataset Preview**  
   ![Dataset Preview](images/dataset_preview.png)  

2. **Sample Visualizations**  
   - Histogram (MSRP distribution)  
   - Boxplot (Invoice Price by Region)  

   ![Visualizations](images/visualizations.png)  

3. **Correlation Heatmap**  
   - Shows relationships between numerical variables  
   - Example: Weight ↔ Horsepower (positive), Weight ↔ MPG (negative)  

   ![Heatmap](images/heatmap.png)  

---

## 📌 Key Insights  

- **Fuel Efficiency & Weight** → Heavier cars have lower MPG.  
- **Horsepower & Cylinders** → Most cars: 4–6 cylinders, 200–250 HP.  
- **Pricing Patterns** → MSRP ranges from $10K–$193K; median ~$27K.  
- **Regional Differences** →  
  - Asia = efficient & lighter  
  - Europe = powerful & premium  
  - USA = heavier & bigger engines  
- **DriveTrain** → FWD dominates economy cars; RWD more common in luxury/performance.  

---

## 🚀 Tech Stack  

- Python 🐍  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  

---

## 📄 How to Run  

1. Clone the repo  
   ```bash
   git clone https://github.com/your-username/cars-dataset-analysis.git
   cd cars-dataset-analysis
