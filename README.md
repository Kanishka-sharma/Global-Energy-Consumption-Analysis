# Global Energy Consumption and Its Economic–Demographic Drivers (1996-2022)

## Overview

This repository presents a comprehensive **statistical analysis of global energy consumption** from 1996 to 2022, focusing on how **economic output (GDP)** and **population** influence total energy demand.  
The study integrates **exploratory data analysis (EDA)**, **statistical modeling**, and **visual interpretation** to uncover structural relationships and regional variations in global energy systems.

All analyses were performed in **R**, using the **tidyverse** ecosystem for data handling and visualization.

---

## Objectives

- Quantify global and regional **energy consumption patterns** over time.  
- Assess **data completeness and quality** across countries.  
- Examine **statistical relationships** between GDP, population, and energy use.  
- Evaluate **regional energy compositions** (fossil, nuclear, renewables).  
- Conduct comparative **country case studies** (Japan vs. South Korea).  

---

## Dataset Description

| Attribute | Description |
|------------|-------------|
| **Source** | Aggregated from multiple open global energy datasets (1996–2022) |
| **Observations** | ~4,300 country-year records |
| **Variables** | `country`, `year`, `population`, `gdp`, `primary_energy`, `fossil_fuel`, `nuclear`, `renewables` |

### **Data Preparation**
- Missing values handled via **pairwise complete observations**.  
- **Log-transformations** applied to right-skewed variables (`gdp`, `population`, `primary_energy`).  
- GDP categorized into quartiles to assess **energy intensity by economic tier**.  

---

## Analytical Workflow

### **1. Data Quality & Structure**
- Evaluated variable distributions and missing data patterns.  
- Identified **non-random missingness** in lower-income countries.  

### **2. Global Energy Composition (2010 Snapshot)**
- Extracted year 2010 to visualize global **energy mix** across regions.  
- Found **fossil dominance** in Asia & North America, **renewable diversification** in Europe & South America.  

### **3. Economic & Demographic Drivers**
- Created a focused subset (`energy_econ`) with GDP, population, and energy data.  
- Applied correlation and quartile-based analyses.  

#### **Statistical Results**
| Relationship | Correlation (r) | Interpretation |
|---------------|-----------------|----------------|
| GDP ↔ Primary Energy | **0.97** | Very strong positive correlation |
| Population ↔ Primary Energy | **0.69** | Moderate-strong correlation |
| GDP Quartile vs Energy | Increasing trend | Energy rises sharply with GDP |

---

## Key Statistical Insights

- **Economic scale** is the dominant determinant of total energy demand.  
- **Population size** amplifies demand but has a weaker direct effect than GDP.  
- **High-income economies** show greater energy use but improved **efficiency trends**.  
- **Regional heterogeneity** reflects differences in industrial composition and energy policy.  
- **Missing data bias** remains concentrated in lower-income countries.  

---

## Technical Stack

| Category | Tools / Packages |
|-----------|------------------|
| **Language** | R (≥ 4.3) |
| **Data Manipulation** | `dplyr`, `tidyr`, `readr` |
| **Visualization** | `ggplot2`, `ggcorrplot`, `VIM`, `scales` |
| **Statistical Analysis** | `cor()`, `lm()`, log-transformation, variance analysis |
| **Reproducibility** | R Markdown (`.Rmd`) / Quarto (`.qmd`) |



