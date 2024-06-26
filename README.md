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
| The "invoice_date" column has been converted to a datetime data type. | ![Screenshot 2024-06-17 at 10 46 54 AM](https://github.com/brian-campbell/athletic_sales_analysis/assets/798207/bc9a5d36-b065-418f-8231-00d9def5ce3b) | ![Screenshot 2024-06-10 at 6 40 00 PM](https://github.com/brian-campbell/athletic_sales_analysis/assets/798207/88b8097c-ed36-4bb3-abed-a68a382c5e47) |

### Determine which Region Sold the Most Products
| Requirement | My Results | Required Results |
| ----------- | ---------- | ---------------- |
| A `groupby` or `pivot_table` function has been used to create a multi-index DataFrame with the "region", "state", and "city" columns. | ![Screenshot 2024-06-17 at 10 55 41 AM](https://github.com/brian-campbell/athletic_sales_analysis/assets/798207/fc07a685-744d-4ccf-8946-16427f56b4d2) ![Screenshot 2024-06-17 at 10 55 49 AM](https://github.com/brian-campbell/athletic_sales_analysis/assets/798207/a02aa665-d5fd-49dc-899a-43ef2094a7fa) | ![Screenshot 2024-06-17 at 10 52 08 AM](https://github.com/brian-campbell/athletic_sales_analysis/assets/798207/32fe52a4-a20c-46da-8d21-df2a661e2dea) ![Screenshot 2024-06-17 at 10 52 40 AM](https://github.com/brian-campbell/athletic_sales_analysis/assets/798207/80566a73-d5ab-4a1d-a5c8-4588ccac9545) |
| The aggregated column has been renamed to reflect the aggregation of the data in the column. | Same as/See above. | Same as/See above. |
| The results are sorted in descending order to show the top five regions, including the state and city that sold the most products. | Same as/See above. | Same as/See above. |

### Determine which Region had the Most Sales
| Requirement | My Results | Required Results |
| ----------- | ---------- | ---------------- |
| A `groupby` or `pivot_table` function has been used to create a multi-index DataFrame with the "region", "state", and "city" columns. | ![Screenshot 2024-06-17 at 11 12 44 AM](https://github.com/brian-campbell/athletic_sales_analysis/assets/798207/bb2b5345-cfa1-4f5a-8f24-0248c06cbde9) ![Screenshot 2024-06-17 at 11 12 53 AM](https://github.com/brian-campbell/athletic_sales_analysis/assets/798207/78785765-2895-4520-b616-cd2d47ac7f97) | ![Screenshot 2024-06-17 at 11 03 06 AM](https://github.com/brian-campbell/athletic_sales_analysis/assets/798207/6a7bbf3e-975e-4ead-80a6-20e8d79dde91) ![Screenshot 2024-06-17 at 11 03 13 AM](https://github.com/brian-campbell/athletic_sales_analysis/assets/798207/883958ee-4e14-4fc7-8931-4607f1353f79) |
| The aggregated column has been renamed to reflect the aggregation of the data in the column. | Same as/See above. | Same as/See above. |
| The results are sorted in descending order to show the top five regions, including the state and city that generated the most sales. | Same as/See above. | Same as/See above. |

### Determine which Retailer had the Most Sales
| Requirement | My Results | Required Results |
| ----------- | ---------- | ---------------- |
| A `groupby` or `pivot_table` function has been used to create a multi-index DataFrame with the "retailer", "region", "state", and "city" columns. | ![Screenshot 2024-06-17 at 11 14 15 AM](https://github.com/brian-campbell/athletic_sales_analysis/assets/798207/639a0b3a-bec3-4a97-a72b-1a0ebb8c4919) ![Screenshot 2024-06-17 at 11 14 24 AM](https://github.com/brian-campbell/athletic_sales_analysis/assets/798207/5b0a3a52-a984-470b-81e0-24ff8656715e) | ![Screenshot 2024-06-17 at 11 04 46 AM](https://github.com/brian-campbell/athletic_sales_analysis/assets/798207/2e22e0ed-722a-4e5b-90ed-b2eb4799d13d) ![Screenshot 2024-06-17 at 11 04 53 AM](https://github.com/brian-campbell/athletic_sales_analysis/assets/798207/18710607-eb2d-4d3c-8e0e-647776d2ad8c) |
| The aggregated column has been renamed to reflect the aggregation of the data in the column. | Same as/See above. | Same as/See above. |
| The results are sorted in descending order to show the top five retailers along with their region, state, and city that generated the most sales. | Same as/See above. | Same as/See above. |

### Determine which Retailer Sold the Most Women's Athletic Footwear
| Requirement | My Results | Required Results |
| ----------- | ---------- | ---------------- |
| A filtered DataFrame is created that shows only women's athletic footwear sales data. (8 points) | ![Screenshot 2024-06-17 at 11 10 19 AM](https://github.com/brian-campbell/athletic_sales_analysis/assets/798207/e81a0325-5131-4995-bde9-34303bcbb630) | ![Screenshot 2024-06-17 at 11 09 17 AM](https://github.com/brian-campbell/athletic_sales_analysis/assets/798207/c3d96a97-349f-4e4d-a764-4f208b4fdb31) |
| A `groupby` or `pivot_table function` has been used to create a multi-index DataFrame with the "retailer", "region", "state", and "city" columns. | ![Screenshot 2024-06-17 at 11 11 07 AM](https://github.com/brian-campbell/athletic_sales_analysis/assets/798207/a98e3eaa-247d-41f5-ac67-d5cb4afc326a) ![Screenshot 2024-06-17 at 11 11 15 AM](https://github.com/brian-campbell/athletic_sales_analysis/assets/798207/0c2e4624-7ff1-45fd-ba94-42b3f8465faf) | ![Screenshot 2024-06-17 at 11 07 09 AM](https://github.com/brian-campbell/athletic_sales_analysis/assets/798207/17b69108-8bb8-46b2-b64d-d97ffc18baa5) ![Screenshot 2024-06-17 at 11 07 18 AM](https://github.com/brian-campbell/athletic_sales_analysis/assets/798207/e97844ae-ab3c-46ff-8be4-5777c89fbf09) |
| The aggregated column has been renamed to reflect the aggregation of the data in the column. | Same as/See above. | Same as/See above. |
| The results are sorted in descending order to show the top five retailers along with their region, state, and city that had the most women's athletic footwear sales. | Same as/See above. | Same as/See above. |

### Determine the Day with the Most Women's Athletic Footwear Sales
| Requirement | My Results | Required Results |
| ----------- | ---------- | ---------------- |
| A pivot table is created that has the "invoice_date" column as the index and the "total_sales" column assigned to the `values` parameter. | ![Screenshot 2024-06-17 at 10 50 11 AM](https://github.com/brian-campbell/athletic_sales_analysis/assets/798207/1a38f5ae-8a95-4b34-baa1-5b52fe748d48) | ![Screenshot 2024-06-10 at 6 47 45 PM](https://github.com/brian-campbell/athletic_sales_analysis/assets/798207/1db4a388-ab33-4a58-af68-9f9b46d87a87) |
| The aggregated column has been renamed to reflect the aggregation of the data in the column. | Same as/See above. | Same as/See above |
| The `resample` function is used on the pivot table, the data is placed into daily bins, and the total sales for each day is calculated. | ![Screenshot 2024-06-17 at 10 49 09 AM](https://github.com/brian-campbell/athletic_sales_analysis/assets/798207/cfd72d3e-4419-4032-927c-e6f83017a9e1) | ![Screenshot 2024-06-10 at 6 46 35 PM](https://github.com/brian-campbell/athletic_sales_analysis/assets/798207/c7d6dec7-d268-491f-8245-6cb5e0515fa9) |
| The results are sorted in descending order to show the days that generated the most women's athletic footwear sales. | Same as/See above. | Same as/See above |

### Determine the Week with the Most Women's Athletic Footwear Sales
| Requirement | My Results | Required Results |
| ----------- | ---------- | ---------------- |
| The `resample` function is used on the pivot table, the data is placed into weekly bins, and the total sales for each week is calculated. | ![Screenshot 2024-06-17 at 10 47 57 AM](https://github.com/brian-campbell/athletic_sales_analysis/assets/798207/dde87871-1fbd-4092-ae00-8eeb0690e33b) | ![Screenshot 2024-06-10 at 6 45 40 PM](https://github.com/brian-campbell/athletic_sales_analysis/assets/798207/0a54484f-0c83-43b9-b043-98bc8472fd9e) |
| The results are sorted in descending order to show the weeks that generated the most women's athletic footwear sales. | Same as/See above. | Same as/See above. |
