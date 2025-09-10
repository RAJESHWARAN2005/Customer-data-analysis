Project Overview

This project was developed during my internship to showcase how raw data can be transformed into meaningful insights using Power BI. The dashboard highlights key business metrics through interactive visuals, enabling data-driven decision-making.

🔎 Stepwise Process
1. Define Objectives

Set project goals and KPIs (e.g., Total Sales, Revenue Growth, Customer Trends).

2. Data Collection

Collected data from multiple sources (Excel/CSV/SQL).

Connected sources into Power BI Desktop.

3. Data Cleaning & Transformation

Used Power Query to clean and prepare data.

Fixed data types, removed nulls, merged tables, and standardized fields.

4. Data Modeling

Built a star schema (fact & dimension tables).

Added a Date Table and created relationships.

5. DAX Calculations

Created calculated measures to track KPIs. Example:

Total Sales = SUM('Sales'[SalesAmount])

YoY Growth % =
VAR Current = [Total Sales]
VAR Previous = CALCULATE([Total Sales], SAMEPERIODLASTYEAR('Date'[Date]))
RETURN DIVIDE(Current - Previous, Previous)

6. Dashboard Design

Designed pages for:

Overview Dashboard – High-level KPIs

Trends Dashboard – Sales over time

Product Analysis – Best/worst performing items

Customer Insights – Demographics & behavior

Geography Insights – Regional performance

7. Interactivity

Added slicers, drillthrough pages, bookmarks, and navigation buttons.

8. Validation & Optimization

Validated KPIs with source data.

Optimized model by removing unnecessary columns and using efficient DAX.

9. Deployment

Published to Power BI Service.

Enabled scheduled refresh and configured access permissions.

🛠️ Tools & Technologies

Power BI Desktop

Power Query (M Language)

DAX (Data Analysis Expressions)

ETL Concepts

📂 Repository Structure
├── README.md                   # Project documentation  
├── Internship project 1.pbix    # Power BI dashboard file  
├── data/                        # Sample dataset (optional)  
├── docs/                        
│   ├── screenshots/             # Dashboard screenshots  
│   └── model_diagram.png        # Data model visualization  
├── measures.md                  # List of DAX measures  
└── HOW_TO_RUN.md                # Instructions to run the PBIX file 
