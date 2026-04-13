# Real Estate Data Analysis: Madrid, Spain

An exploratory data analysis project using a real-world web-scraped dataset from Fotocasa, one of Spain's largest real estate platforms, to uncover pricing trends across municipalities in and around Madrid.

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Analysis Workflow](#analysis-workflow)
- [Key Findings](#key-findings)
- [Tech Stack](#tech-stack)
- [Author](#author)

---

## Overview

This project applies data cleaning, statistical analysis, and visualization techniques to a real estate dataset containing listings from multiple Madrid-area municipalities. A focus area is the "south belt" of Madrid — Fuenlabrada, Leganés, Getafe, and Alcorcón — where pricing, price per square meter, and geographic distribution are analyzed in depth.

See [`project.ipynb`](./project.ipynb) for the full walkthrough and all project work.

---

## Dataset

- **Source:** Fotocasa (scraped for academic purposes)
- **Size:** ~15,335 listings
- **Key columns:** `price`, `surface`, `rooms`, `bathrooms`, `address`, `level5` (municipality), `latitude`, `longitude`, `realEstate_name`

---

## Project Structure

---

## Analysis Workflow

**1. Data Loading & Inspection**
- Read semicolon-delimited CSV and inspect shape, columns, and data types
- Identify and handle missing values

**2. Descriptive Statistics**
- Most and least expensive listings (with address lookup)
- Largest and smallest properties by surface area
- Unique municipality count and listing distribution

**3. Municipality-Level Analysis**
- Mean price in Arroyomolinos with histogram and distribution commentary
- Price comparison between Valdemorillo and Galapagar (overall and per square meter)

**4. South Belt Deep Dive (Fuenlabrada, Leganés, Getafe, Alcorcón)**
- Median and mean price bar charts
- Sample mean and variance for price, rooms, surface, and bathrooms
- Most expensive listing per municipality
- Normalized price histograms across all four populations
- Price per square meter comparison (Getafe vs. Alcorcón)
- Bar chart of average price per square meter across all four towns

**5. Geographic Visualization**
- Interactive map using `ipyleaflet` with color-coded markers by municipality

**6. Surface vs. Price Relationship**
- Scatter plot with outlier filtering and best-fit line overlay

---

## Key Findings

- Getafe and Alcorcón carry the highest median home prices in the south belt; Fuenlabrada is the most affordable.
- Despite Getafe's higher overall price, Alcorcón commands roughly 8% more per square meter.
- There is a moderate positive correlation between surface area and price across the dataset.
- Price distributions within the south belt are fairly clustered after normalization, suggesting limited extreme outliers within this submarket.
- Madrid Capital contains the most listings in the dataset by a wide margin (6,235).

---

## Tech Stack

- Python
- Pandas, NumPy
- Matplotlib
- ipyleaflet

---

## Author

Taylor Clements, PhD
