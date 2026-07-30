# Food Waste Prediction – Data Cleaning with Excel

## Project Overview

This project is based on the **Messy Food Waste Prediction Dataset** from Kaggle.

The project began as a data cleaning exercise in Microsoft Excel. Instead of following a complete Excel course, I am learning by solving real-world problems as they arise. Whenever I encounter a new challenge, I research the appropriate solution using Google and YouTube.

The objective is to improve my Excel and data analysis skills while preparing the dataset for future analysis and predictive modeling.

---

## Dataset

**Competition:** Messy Food Waste Prediction Dataset

**Source:** https://www.kaggle.com/competitions/messy-food-waste-prediction-dataset/overview/description

> This repository documents my personal learning process and solution. It is not an official Kaggle submission.

---

## Dataset Features

| Column           | Description                                                     |
| ---------------- | --------------------------------------------------------------- |
| date             | Date of food waste measurement                                  |
| meals_served     | Number of meals served (stored as text with formatting issues)  |
| kitchen_staff    | Number of kitchen staff (stored as text with formatting issues) |
| temperature_C    | Temperature in Celsius                                          |
| humidity_percent | Humidity percentage                                             |
| day_of_week      | Numeric representation of weekdays (0 = Monday, 6 = Sunday)     |
| special_event    | Indicates whether a special event occurred                      |
| past_waste_kg    | Food waste generated in the previous cycle                      |
| staff_experience | Staff experience level                                          |
| waste_category   | Category of food waste                                          |
| food_waste_kg    | Target variable (available only in train.csv)                   |

---

## Work Completed

### 1. Dataset Exploration

* Reviewed all columns
* Identified data types
* Located formatting inconsistencies
* Understood the target variable

### 2. Cleaned Numeric Columns

**Columns cleaned:**

* `meals_served`
* `kitchen_staff`

**Tasks performed:**

* Removed extra spaces using **TRIM()**
* Converted text values into numeric format

### 3. Converted Day Codes to Weekday Names

The `day_of_week` column stored weekdays as numbers.

Using the **IFS()** function, I created a new column that converts the numeric codes into weekday names, making the dataset easier to read during analysis.

### 4. Standardized Categories

The `waste_category` column contained inconsistent capitalization (for example, `MeAt`, `MEAT`, and `dairy`).

Using Excel filters, I standardized the category names so identical values are represented consistently.

### 5. Outlier Detection

Calculated the **Interquartile Range (IQR)** to detect potential outliers.

Tasks performed:

* Calculated Q1 and Q3
* Calculated the IQR
* Determined lower and upper bounds
* Applied Conditional Formatting to highlight extreme values

Outliers have been identified but not removed.

---

## Excel Skills Practiced

* Data exploration
* TRIM()
* IFS()
* Converting text to numbers
* Filtering
* Data standardization
* Conditional Formatting
* Quartiles
* Interquartile Range (IQR)
* Outlier detection

---

## Next Steps

* Clean remaining formatting issues
* Validate suspicious values
* Handle missing values (if necessary)
* Create descriptive statistics
* Build charts and visualizations
* Explore relationships between variables
* Prepare the dataset for predictive modeling

---

## Tools Used

* Microsoft Excel
* Kaggle
* Google
* YouTube

---

## Project Status

🚧 **In Progress**

This repository will be updated as I continue cleaning, analyzing, and exploring the dataset.

