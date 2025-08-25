# Insurance Data Practice

This repository contains a simple practice notebook for working with **Pandas** in Python.

## Dataset

The dataset used is the Insurance Dataset: https://drive.google.com/file/d/1-7mcBguuzAV7JWVu2XCpgAO-fO6X2cl0/view

## What I Did

1. **Loaded the data**  
   - Loaded the CSV file into a Pandas DataFrame called `df_insurance`.  
   - Previewed the first and last rows using `.head()` and `.tail()`.  
   - Checked summary information with `.info()`.

2. **Sliced the data**  
   - Selected specific rows and columns using `.loc`.  
   - Saved certain columns as variables (e.g., the `smoker` column).  
   - Checked values for individual customers (e.g., customer at index 20).

3. **Filtered the data**  
   - Created filters for conditions like age under 30 or customers who are male.  
   - Combined filters to find customers matching multiple criteria (e.g., male and under 30).  
   - Filtered regions containing "south" using `.str.contains`.

## Tools Used

- Python 3  
- Pandas library  

## Author

- Bashar Bayatna
