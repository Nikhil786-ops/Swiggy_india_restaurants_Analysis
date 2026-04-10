# Swiggy India Restaurant Analysis

This is one of my data analysis projects where I explored Swiggy's restaurant data from across India.
The dataset had 1.48 lakh+ restaurants and was pretty messy — so most of the work went into cleaning it first before doing any analysis.

---

## What This Project Is About

I wanted to answer some real questions like:
- Which cities have the most restaurants on Swiggy?
- What cuisines are most popular across India?
- Does expensive food actually get better ratings?
- Which restaurant chains have the most outlets?

---

## Tools Used

- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook (Kaggle)

---

## Files in This Repo

| File | Description |
|------|-------------|
| Swiggy_Data_Analysis.ipynb | Main notebook with cleaning + EDA |
| swiggy_cleaned.csv | Cleaned dataset after processing |
| README.md | This file |

---

## Data Cleaning Steps

The raw data had quite a few issues:

- cost column had rupee symbol — removed and converted to numeric
- rating column had '--' for unrated restaurants — replaced with median
- rating_count had values like 'Too Few Ratings', '1K+ ratings' — dropped the column
- lic_no column had 229+ missing values and was not useful — dropped
- City and restaurant names had inconsistent casing like 'DELHI', 'delhi' — fixed with str.title()
- Found one restaurant with cost = 3,00,350 (clearly a data entry error) — removed as outlier
- Missing cuisine values filled with 'Unknown'

---

## Key Findings

1. Bikaner has the most restaurants on Swiggy — honestly did not expect this
2. North Indian + Chinese is the most popular cuisine combo in India
3. Dominos Pizza leads with 442+ outlets across India
4. Smaller cities like Chopda and South Goa have better average ratings than metros
5. Khan Market Delhi and Fort Colaba Mumbai are the most expensive areas
6. There is very low correlation between cost and rating — price does not guarantee quality

---

## Visualizations

- Top 10 cities by number of restaurants
- Top 10 most popular cuisines
- Top restaurant chains by outlets
- Rating distribution
- City-wise average rating
- City-wise average cost
- Cost vs Rating scatter plot

---

## What I Learned

This was my first time working with such a large real-world dataset.
I learned that data cleaning takes way more time than the actual analysis — and small things like a rupee symbol or inconsistent casing can break everything if not handled properly.

---

## Connect With Me

- LinkedIn: linkedin.com/in/nikhil-raghuwanshi-26sr
- GitHub: github.com/nikhil-raghuwanshi
