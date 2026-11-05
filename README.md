# Task 1: Data Cleaning and Preprocessing

## Dataset
Netflix Movies and TV Shows (Kaggle)

## Tools Used
Python, Pandas, Jupyter Notebook (VS Code)

## Steps Performed
1. Loaded the dataset and inspected it using `head()`, `shape`, `info()` and `isnull().sum()`.
2. Renamed column headers to lowercase with no spaces.
3. Checked for duplicates: none found.
4. Handled missing values:
   - director (2634), cast (825), country (831), rating (4), duration (3) filled with "Unknown"
   - 10 rows with missing date_added were dropped
5. Standardized text values (removed extra spaces, consistent casing).
6. Converted `date_added` to datetime and saved in dd-mm-yyyy format.

## Summary of Changes
| | Before | After |
|---|---|---|
| Rows | 8807 | 8797 |
| Columns | 12 | 12 |
| Missing values | 4,307 | 0 |

## Files
- `cleaning.ipynb`: code
- `netflix_titles.csv`: raw dataset
- `cleaned_netflix.csv`: cleaned dataset