

# Case Study 2 — Yelp Check-in and Business Analytics

*(Data Mining & Exploratory Analytics Project)*

## 📌 Overview

This project performs exploratory data analytics on the public **Yelp Academic Dataset**, focusing specifically on the relationship between **business attributes** and **user check-in behaviors**.

The analysis integrates two large JSON data sources:

* `yelp_academic_dataset_business.json`
* `yelp_academic_dataset_checkin.json`

The notebook performs data loading, cleaning, preprocessing, transformation, descriptive analytics, and visualization to uncover temporal patterns and insights about business activity and popularity.

---

## 🎯 Objectives

The goals of this case study are:

1. Combine business metadata with check-in timestamps
2. Understand business popularity over time
3. Explore temporal check-in patterns (by hour, day, weekday/weekend)
4. Identify high-traffic locations and business types
5. Produce interpretable analytics and visual insights

---

## 📂 Repository Content

| File                                  | Description                                       |
| ------------------------------------- | ------------------------------------------------- |
| `CaseStudy2.ipynb`                    | Main analysis notebook                            |
| `yelp_academic_dataset_business.json` | Business metadata (categories, location, rating…) |
| `yelp_academic_dataset_checkin.json`  | Check-in timestamps                               |
| `business_ids.txt`                    | Filtered/business selection list                  |
| `checkin_ids.txt`                     | Filtered check-in keys                            |

---

## 🔧 Techniques & Methods

### ✔ Data Preparation

* JSON parsing
* Flattening nested Yelp structures
* Handling missing values
* Filtering relevant business IDs
* Extracting datetime features

### ✔ Feature Engineering

* Hour of day
* Day‐of‐week
* Aggregate counts
* Business category rollups

### ✔ Analytics & Methods

* Temporal analysis
* Business popularity ranking
* Category-wise comparison
* Descriptive statistics

### ✔ Visualization

* Time-series plots
* Check-in histograms by hour
* Weekday/weekend distributions

---

## 🧠 Key Insights

Although details appear inside the notebook, major findings include:

* Check-ins follow predictable temporal cycles
* Weekend behavior differs significantly from weekdays
* Certain business categories consistently receive more check-ins
* Location and category strongly influence demand patterns

These insights demonstrate how real-world location analytics can indicate customer behavior, business demand, and operational timing.

---

## 🛠 Requirements

### Environment

* Python 3.7+
* Jupyter Notebook

### Libraries (commonly used in the notebook)

```txt
pandas
numpy
json
matplotlib
seaborn
datetime
```

---

## ▶ How to Run

1. Download the all dataset
2. Open the notebook:

```bash
jupyter notebook CaseStudy2.ipynb
```

3. Run all cells sequentially

Processing may take additional time depending on system memory and JSON size.

---

## 📈 Output

Running the notebook produces:

* temporal check-in visualizations
* aggregated business statistics
* category comparisons
* busiest business rankings

These results form the basis for further ML modeling or demand forecasting.

---

## 🔚 Conclusion

This case study demonstrates how raw geo-business datasets can be transformed into meaningful behavioral insights through structured exploratory analysis. The workflow presented here represents a reproducible analytical pipeline applicable to broader real-world recommendation, business intelligence, or urban analytics use-cases.
