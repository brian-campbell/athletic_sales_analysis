# AI Bootcamp - Athletic Sales Analysis - Module 5 Challenge

## Table of Contents
*  [**Overview**](#overview)
*  [**Background**](#background)
*  [**Files**](#files)
*  [**Technical Requirements**](#technical-requirements)
*  [**Run the code**](#run-the-code)
*  [**Requirements and Solution**](#requirements-and-solution)

## Overview
This repository contains the source code for the OSU AI Bootcamp athletic sales analysis for Module 5. This challenge uses a dataset for athletic sales over two years. The goal is to use continue to use the pandas framework to explore and analyze data.

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
| The two DataFrames have been combined on the rows using an inner join and the index has been reset. | ![Screenshot 2024-06-17 at 10 45 21 AM](https://github.com/brian-campbell/athletic_sales_analysis/assets/798207/55cc4194-762c-4cbd-b84a-4f95b130eb9f) | ![Screenshot 2024-06-10 at 6 38 41 PM](https://github.com/brian-campbell/athletic_sales_analysis/assets/798207/f128b5c2-8651-4915-a9b5-e45bbb5313f0) |
| The "invoice_date" column has been converted to a datetime data type. | | ![Screenshot 2024-06-10 at 6 40 00 PM](https://github.com/brian-campbell/athletic_sales_analysis/assets/798207/88b8097c-ed36-4bb3-abed-a68a382c5e47) |

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
| A pivot table is created that has the "invoice_date" column as the index and the "total_sales" column assigned to the `values` parameter. | | ![Screenshot 2024-06-10 at 6 47 45 PM](https://github.com/brian-campbell/athletic_sales_analysis/assets/798207/1db4a388-ab33-4a58-af68-9f9b46d87a87) |
| The aggregated column has been renamed to reflect the aggregation of the data in the column. | | Same as/See above |
| The `resample` function is used on the pivot table, the data is placed into daily bins, and the total sales for each day is calculated. | | ![Screenshot 2024-06-10 at 6 46 35 PM](https://github.com/brian-campbell/athletic_sales_analysis/assets/798207/c7d6dec7-d268-491f-8245-6cb5e0515fa9) |
| The results are sorted in descending order to show the days that generated the most women's athletic footwear sales. | | Same as/See above |

### Determine the Week with the Most Women's Athletic Footwear Sales
| Requirement | My Results | Required Results |
| ----------- | ---------- | ---------------- |
| The `resample` function is used on the pivot table, the data is placed into weekly bins, and the total sales for each week is calculated. | | ![Screenshot 2024-06-10 at 6 45 40 PM](https://github.com/brian-campbell/athletic_sales_analysis/assets/798207/0a54484f-0c83-43b9-b043-98bc8472fd9e) |
| The results are sorted in descending order to show the weeks that generated the most women's athletic footwear sales. | | Same as/See above. |
