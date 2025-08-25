# Insurance Dataset Analysis

This repository contains a practice notebook for exploring the Insurance dataset using Python. The analysis includes data cleaning, exploration, univariate and multivariate visualizations, and correlation insights.


## Dataset
The dataset used is the Insurance Dataset: [Insurance Dataset Link](https://drive.google.com/file/d/1-7mcBguuzAV7JWVu2XCpgAO-fO6X2cl0/view)
**Basic Information:**

- Rows: 1,338  
- Columns: 7  
- Features: `age`, `sex`, `bmi`, `children`, `smoker`, `region`, `charges`

**Sample Data:**

| age | sex    | bmi   | children | smoker | region     | charges   |
|-----|--------|-------|----------|--------|-----------|-----------|
| 19  | female | 27.90 | 0        | 1      | southwest | 16885.0   |
| 18  | male   | 33.77 | 1        | 0      | southeast | 1726.0    |
| 28  | male   | 33.00 | 3        | 0      | southeast | 4449.0    |
| 33  | male   | 22.70 | 0        | 0      | northwest | 21984.0   |
| 32  | male   | 28.88 | 0        | 0      | northwest | 3867.0    |

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

### Visualization 
- did both Univariate and Multivariate plots.  

**Figures:**
1. **Histogram of BMI**: Distribution of BMI across all individuals.
   <img width="571" height="455" alt="Distribution of BMI" src="https://github.com/user-attachments/assets/cd22b91c-a0d8-4d2d-a8a9-8c983308c221" />
- Most individuals have a BMI between approximately 20 and 35.
- Some individuals have BMI greater than 50, visible in the boxplot.
2. **Boxplot of BMI by Region**: BMI variations by region with median and outliers.
    <img width="562" height="455" alt="BMI By Region" src="https://github.com/user-attachments/assets/43fe7eb5-19a8-4836-88d4-71179c7de8eb" />
- Southwest region shows slightly higher median BMI.  
- Northwest and Southeast regions have slightly lower median BMI. 

    
3. **Correlations**
<img width="1102" height="836" alt="Heatmap_Insurance" src="https://github.com/user-attachments/assets/2e59b00b-399d-4e4f-9582-b75e317e3b91" />

- Strong positive correlation between `smoker` and `charges` (0.79).  
- Moderate correlation between `age` and `charges` (0.30).  
- `BMI` also positively correlates with `charges` (0.20).

4. **Barplot charges for both Genders and their smoking status**
<img width="589" height="455" alt="Charges for Males:Females and smoker:non-smoker" src="https://github.com/user-attachments/assets/58bf8d33-9d73-49fa-bf8d-eadaf810b8c8" />


- Smokers pay significantly higher charges than non-smokers.  
- Boxplot highlights outliers, showing extreme charges among smokers.
- 
5. **Linear Model Plot-ChargesVS. BMI- Colored by Smoking status**
<img width="549" height="512" alt="Charged VS  BMI colored by Smoker" src="https://github.com/user-attachments/assets/3ea75be9-1076-4286-8401-55212ddbb2e8" />
- As expected from the previous analysis, there is a strong positive correlation between BMI and charges for smokers, which is evident from the upper regression line. For non-smokers, the correlation is weaker, visible along the lower regression line.
  


## Tools Used
- Python 3  
- Pandas library  
- Matplotlib  
- Seaborn  

##  Information 
 For any Questions or Recommendations:
  - Bashar Bayatna (Mechatronics Engineer|Junior Data Scientist)
  - Basharbayatna11@gmail.com

