# CODSOFT_TASK1
# CodSoft Internship - Task 1: Data Cleaning & Preprocessing

## About this task
This is Task 1 of my Data Analytics internship with CodSoft. The goal was 
to take a messy, real-world dataset and clean it up so it's ready for analysis.

## Dataset
I used the Zomato Bangalore Restaurants dataset from Kaggle 
(link: https://www.kaggle.com/datasets/himanshupoddar/zomato-bangalore-restaurants).

I picked this one on purpose instead of a pre-cleaned dataset because it actually 
has real problems in it - missing values, duplicate rows, ratings stored as text 
like "4.1/5" or "NEW", and prices with commas in them like "1,200". Felt like a 
more realistic dataset to practice on.

## What I did
- Loaded the dataset and checked its shape and structure (51,717 rows, 17 columns 
  to start with)
- Checked which columns had missing values - some had almost 50% missing (like 
  dish_liked)
- Found duplicate rows in the data
- Noticed the rate column was text ("4.1/5") instead of a number, and had junk 
  values like "NEW" and "-"
- Dropped columns I didn't need for analysis (url, phone, address, etc.)
- Removed duplicates
- Converted rate and cost columns into proper numbers
- Filled missing values (used median for numeric columns, "Unknown" for a couple 
  of categorical ones)
- Renamed some columns to make them easier to work with

## Before vs After
Started with 51,717 rows and a bunch of missing values + duplicates.
Ended with 51,588 clean rows, 0 missing values, 0 duplicates, and correct data 
types throughout.

## Tools
Python, Pandas, NumPy, Google Colab

## Files in this repo
- CodSoft_Task1_Cleaning.ipynb - all the code
- zomato_cleaned.csv - the final cleaned dataset

#codsoft #dataanalytics
