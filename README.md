
This repository contains a simple practice notebook for working with Pandas in Python.

## Dataset
The dataset used is the Insurance Dataset: [Insurance Dataset Link](https://drive.google.com/file/d/1-7mcBguuzAV7JWVu2XCpgAO-fO6X2cl0/view)

## What I Did

### Loaded the data
- Loaded the CSV file into a Pandas DataFrame called `df_insurance`.  
- Previewed the first and last rows using `.head()` and `.tail()`.  
- Checked summary information with `.info()`.  

### Sliced the data
- Selected specific rows and columns using `.loc`.  
- Saved certain columns as variables (e.g., the `smoker` column).  
- Checked values for individual customers (e.g., customer at index 20).  

### Filtered the data
- Created filters for conditions like age under 30 or customers who are male.  
- Combined filters to find customers matching multiple criteria (e.g., male and under 30).  
- Filtered regions containing "south" using `.str.contains`.  

### Grouped the data
- Used `.groupby()` to calculate average charges by sex.  
- Used `.groupby()` to calculate average charges by smoker status.  
- Combined `groupby` to calculate average charges by both smoker status and sex.  

### BMI Analysis
- Plotted histogram of BMI to understand overall distribution.  
- Used boxplot to compare BMI across different regions using `seaborn`.  

**Figures:**
1. **Histogram of BMI**: Distribution of BMI across all individuals.
    <img width="571" height="455" alt="Distribution of BMI" src="https://github.com/user-attachments/assets/cd22b91c-a0d8-4d2d-a8a9-8c983308c221" />

2. **Boxplot of BMI by Region**: BMI variations by region with median and outliers.
    <img width="562" height="455" alt="BMI By Region" src="https://github.com/user-attachments/assets/43fe7eb5-19a8-4836-88d4-71179c7de8eb" />

**Key Insights:**
- **Overall BMI Distribution:** Most individuals have a BMI between approximately 20 and 35.  
- **Regional Differences:**  
  - Southwest region shows slightly higher median BMI.  
  - Northwest and Southeast regions have slightly lower median BMI.  
- **Outliers:** Some individuals have BMI greater than 50, visible in the boxplot.  
- **Implication for Insurance:** Higher BMI values may correlate with higher insurance charges, useful for risk assessment and premium calculation.

## Tools Used
- Python 3  
- Pandas library  
- Matplotlib  
- Seaborn  

## Author
Bashar Bayatna

