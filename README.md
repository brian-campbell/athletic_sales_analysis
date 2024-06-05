# AI Bootcamp - Athletic Sales Analysis - Module 5 Challenge

## Table of Contents
*  [**Overview**](#overview)
*  [**Background**](#background)
*  [**Files**](#files)
*  [**Technical Requirements**](#technical-requirements)
*  [**Run the code**](#run-the-code)
*  [**Requirements and Solution**](#requirements-and-solution)

## Overview


## Background
The background on this challenge, provided by the course instructors is as follows: 
>"You'll analyze sales data to gain insights into which cities in the U.S. have sold the most athletic wear over two years. Next, you'll determine which retailers had the greatest total sales for athletic wear, and which retailers sold the most women's athletic footwear. Finally, you'll determine which day and week had the highest sales for women's athletic footwear."

## Files
This repository contains four files and a sub-folder:
* `athletic_sales_analysis.ipynb` - the file that contains the solution for the challenge.
* `athletic_sales_analysis.ipynb.ipynb` - the original starter file for the challenge. This is for reference only.
* In the Resources directory the files `athletic_sales_2020.csv` and `athletic_sales_2021.csv` contain the data file for the project provided as part of the challenge.

## Technical requirements
The code in `athletic_sales_analysis.ipynb.` This file is a Jupyter Notebook and requires an appropriate jupyter, pandas, and python tooling installed. This can include environmental containers such a anaconda, etc. It can also be executed inside of an IDE such as Visual Studio Code. The code requires python 3.10 or greater.

The file `athletic_sales_analysis.ipynb.ipynb` is the original starter file provided for the challenge. It is part of the project for reference only. The directory Resources contains the data file client_dataset.csv provided for the challenge.

## Run the code
Assuming a python interpreter is installed and is at least version 3.10 or greater and they jupyter notebook runtime, the program can be executed by calling the jupyter notebook runtime in the directory: E.g., $> jupyter notebook. Once the notebook is running you run each code fragment individually or click on the "Run All" button.

Alternatively it can be executed from within and IDE if the IDE is configured to run python code and is at least 3.10 compatible and a jupyter notebook runtime is installed.

## Requirements and Solution
### Combine and Clean the Data
| Requirement | My Results | Required Results |
| ----------- | ---------- | ---------------- |
| The two DataFrames have been combined on the rows using an inner join and the index has been reset. | | |
| The "invoice_date" column has been converted to a datetime data type. | | |

### Determine which Region Sold the Most Products
| Requirement | My Results | Required Results |
| ----------- | ---------- | ---------------- |
| A `groupby` or `pivot_table` function has been used to create a multi-index DataFrame with the "region", "state", and "city" columns. | | |
| The aggregated column has been renamed to reflect the aggregation of the data in the column. | | |
| The results are sorted in descending order to show the top five regions, including the state and city that sold the most products. | | |

### Determine which Region had the Most Sales
| Requirement | My Results | Required Results |
| ----------- | ---------- | ---------------- |
| A `groupby` or `pivot_table` function has been used to create a multi-index DataFrame with the "region", "state", and "city" columns. | | |
| The aggregated column has been renamed to reflect the aggregation of the data in the column. | | |
| The results are sorted in descending order to show the top five regions, including the state and city that generated the most sales. | | |

### Determine which Retailer had the Most Sales
| Requirement | My Results | Required Results |
| ----------- | ---------- | ---------------- |
| A `groupby` or `pivot_table` function has been used to create a multi-index DataFrame with the "retailer", "region", "state", and "city" columns. | | |
| The aggregated column has been renamed to reflect the aggregation of the data in the column. | | |
| The results are sorted in descending order to show the top five retailers along with their region, state, and city that generated the most sales. | | |

### Determine which Retailer Sold the Most Women's Athletic Footwear
| Requirement | My Results | Required Results |
| ----------- | ---------- | ---------------- |
| A filtered DataFrame is created that shows only women's athletic footwear sales data. (8 points) | | |
| A `groupby` or `pivot_table function` has been used to create a multi-index DataFrame with the "retailer", "region", "state", and "city" columns. | | |
| The aggregated column has been renamed to reflect the aggregation of the data in the column. | | |
| The results are sorted in descending order to show the top five retailers along with their region, state, and city that had the most women's athletic footwear sales. | | |

### Determine the Day with the Most Women's Athletic Footwear Sales
| Requirement | My Results | Required Results |
| ----------- | ---------- | ---------------- |
| A pivot table is created that has the "invoice_date" column as the index and the "total_sales" column assigned to the `values` parameter. | | |
| The aggregated column has been renamed to reflect the aggregation of the data in the column. | | |
| The `resample` function is used on the pivot table, the data is placed into daily bins, and the total sales for each day is calculated. | | |
| The results are sorted in descending order to show the days that generated the most women's athletic footwear sales. | | |

### Determine the Week with the Most Women's Athletic Footwear Sales
| Requirement | My Results | Required Results |
| ----------- | ---------- | ---------------- |
| The `resample` function is used on the pivot table, the data is placed into weekly bins, and the total sales for each week is calculated. | | |
| The results are sorted in descending order to show the weeks that generated the most women's athletic footwear sales. | | |
