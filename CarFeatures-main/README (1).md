# 🚗 Car Features — Data Science Final Project 2025

An end-to-end exploratory data analysis (EDA) of a car features dataset, covering data cleaning, descriptive statistics, visualisation, and insight extraction.

---

## 📋 Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Key Questions Explored](#key-questions-explored)
- [Main Findings](#main-findings)
- [Technologies Used](#technologies-used)
- [How to Run](#how-to-run)
- [Conclusions](#conclusions)

---

## Project Overview

This project follows the full data science workflow:

1. **Data Gathering** — Loading and inspecting the raw dataset
2. **Data Assessment** — Identifying missing values, incorrect types, and inconsistencies
3. **Data Wrangling** — Cleaning, transforming, and handling outliers
4. **Exploratory Data Analysis (EDA)** — Statistical summaries and visualisations
5. **Conclusions** — Summarising findings and limitations

---

## Dataset

- **File:** `Car Features.csv`
- **Size:** ~10,715 vehicles × 17 features
- **Key columns:**

| Column | Description |
|---|---|
| `make` | Car manufacturer |
| `model` | Car model name |
| `year` | Model year |
| `engine_hp` | Engine horsepower |
| `engine_cylinders` | Number of engine cylinders |
| `engine_fuel_type` | Fuel type (petrol, diesel, electric, hybrid, etc.) |
| `transmission_type` | Transmission type (automatic, manual, etc.) |
| `driven_wheels` | Drive type (FWD, RWD, AWD, etc.) |
| `vehicle_style` | Body style (sedan, SUV, coupe, etc.) |
| `vehicle_size` | Vehicle size category |
| `city_mpg` | Fuel efficiency in city driving |
| `highway_mpg` | Fuel efficiency on highways |
| `msrp` | Manufacturer's suggested retail price |
| `popularity` | Popularity score |

---

## Project Structure

```
├── Data_Science_Final_Project_2025_SIM_Car_Features.ipynb   # Main notebook
├── Car Features.csv                                          # Raw dataset
├── cleaned_car_data.xlsx                                     # Cleaned dataset (generated)
└── README.md
```

---

## Key Questions Explored

1. What are the numerical properties of the dataset?
2. How are numerical variables correlated?
3. What is the distribution of numerical features?
4. Are there outliers, and are they real or errors?
5. Is there a relationship between engine power and price?
6. Is fuel efficiency related to engine power?
7. How strongly are city and highway MPG correlated?
8. Which car brands are the most expensive on average?
9. How does engine power affect car price?
10. Are newer cars always more expensive?
11. Which fuel type provides the best fuel efficiency?
12. What is the relationship between vehicle style and number of doors?

---

## Main Findings

- **Engine power vs. price:** Strong positive correlation — more powerful cars are generally more expensive.
- **Fuel efficiency vs. engine power:** Negative relationship — higher horsepower typically means lower MPG.
- **City vs. highway MPG:** Strong positive correlation, indicating consistent efficiency behaviour across both environments.
- **Model year vs. price:** Only a weak positive relationship; year alone is not a strong price predictor.
- **Fuel type efficiency ranking:** Electric > Natural Gas > Diesel > Petrol.
- **Brand pricing:** Luxury and performance brands have significantly higher average MSRP compared to mass-market brands.
- **Vehicle style & doors:** Sedans and SUVs are mostly 4-door; coupes and convertibles are predominantly 2-door.

---

## Technologies Used

- **Python 3**
- `pandas` — data manipulation
- `numpy` — numerical operations
- `matplotlib` — plotting
- `seaborn` — statistical visualisation
- `openpyxl` — Excel export

---

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/car-features-eda.git
   cd car-features-eda
   ```

2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn openpyxl
   ```

3. Place `Car Features.csv` in the project root directory.

4. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

5. Open `Data_Science_Final_Project_2025_SIM_Car_Features.ipynb` and run all cells.

---

## Conclusions

This analysis explored a dataset of over 10,000 vehicles to understand the factors influencing car price, fuel efficiency, and popularity. Key takeaways:

- Vehicle price is primarily driven by **engine horsepower** and **brand**, not model year alone.
- **Electric vehicles** are the most fuel-efficient fuel type in the dataset.
- Outliers in price, MPG, and engine specs were retained as they represent real high-performance or specialty vehicles.
- Correlation patterns were identified, but **correlation does not imply causation** — further predictive modelling would be needed for causal claims.

---

> **Note:** This project was submitted as a final assignment for the Introduction to Data Science course (2025).
