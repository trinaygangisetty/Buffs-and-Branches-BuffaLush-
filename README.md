# Buffs and Branches: Data Cleaning & Environmental Impact 🌍

## Project Overview
This project is a **comprehensive analysis of trees on CU Boulder’s historic campus**, focusing on **canopy coverage, growth dynamics, and environmental sustainability**. It involves meticulous **data cleaning, feature engineering, and storytelling through data visualization**. The project is part of the **Buffalization Data Visualization Challenge 2025** and aims to uncover the **ecological significance of urban forestry**.

---

## Project Structure
- **`tree_data_cleaning.html`** – Code documentation for the data cleaning pipeline.
- **`cleaned_trees_dataset.csv`** – The refined dataset post-cleaning.
- **`CU_Boulder_Tree_Analysis.pdf`** – The complete project report with insights, calculations, and visualizations.

---

## Data Cleaning Process
The dataset contained **777 trees**, requiring rigorous preprocessing to ensure **accuracy and reliability**. The following steps were taken:

### Handling Missing Values
- Conducted a **thorough assessment** of missing values in key fields (Canopy Spread, Height, Species).
- **Mean imputation** was applied where feasible to maintain dataset integrity.
- Records with **critical missing values** were removed to preserve data quality.

### Removing Duplicates
- Checked for duplicates using **Species, Height, Canopy Spread, and Location Coordinates**.
- Eliminated redundant records to prevent **data skewing**.

### Outlier Detection & Removal
- Used **Z-score analysis** to detect anomalies in **Height and Canopy Spread**.
- Verified outliers manually to **preserve biologically valid data**.
- Removed erroneous values while **maintaining ecological accuracy**.

 **Final dataset saved as `cleaned_trees_dataset.csv`**.

---

## Feature Engineering & Calculated Fields
To **enhance the dataset**, several calculated metrics were introduced:

| Feature | Formula | Purpose |
|---------|---------|---------|
| **Canopy Area** | π × (Canopy Spread / 2)² | Measures total ground coverage of a tree’s canopy. |
| **Canopy Volume** | (2/3) × π × (Canopy Spread / 2)³ | Estimates total airspace occupied. |
| **Canopy Density** | Canopy Volume / Canopy Area | Assesses foliage compactness. |
| **Canopy Height Ratio** | Canopy Spread / Height | Evaluates tree proportions. |
| **Bio Mass** | Height × Canopy Spread | Approximates tree biomass. |
| **Carbon Absorbed** | Bio Mass × 0.5 | Estimates carbon sequestration capacity. |
| **Slenderness Index** | Height / sqrt(Canopy Spread) | Identifies structural vulnerability. |
| **Growth Stage Classification** | Height-based categorization | Classifies trees into Sapling, Maturing, Mature, or Ancient. |

---

## Key Insights & Visualizations
This project tells a **data-driven story** about CU Boulder’s trees through **compelling analytics and visualizations**:

### **Canopy Coverage & Carbon Sequestration**
- Trees with **expansive canopies** contribute significantly to **carbon absorption**, mitigating climate impact.
- The **Canopy Coverage Map** highlights high-density foliage areas.

### **Growth Stages & Structural Insights**
- A large portion of trees fall in the **Maturing and Mature categories**, supporting long-term **ecosystem stability**.
- **Slenderness Index Analysis** identifies trees with **potential structural risks** for proactive maintenance.

### **Tree Diversity & Distribution**
- The **Tree Distribution Map** showcases biodiversity across CU Boulder’s campus.
- The **Top N Analysis** highlights trees with exceptional **carbon absorption rates**.

---

## Why This Matters?
Urban forestry plays a **critical role in sustainability**—beyond aesthetics, trees are **natural carbon sinks** that enhance **air quality, biodiversity, and ecological balance**. By **leveraging data science**, this project provides **actionable insights** that aid in **campus planning, conservation efforts, and sustainability policies**.

---

##  Author
📌 **Trinay Gangisetty**  
🏆 **Buffalization Data Visualization Challenge 2025**
