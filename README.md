power-bi-desktop-projects Manufacturing-BI-Solution

End-to-end Business Intelligence solution simulating ERP data for global manufacturing operations using Python, SQL, and Power BI. This project simulates an end-to-end Business Intelligence (BI) solution for a global manufacturing enterprise. It mirrors how real organizations use ERP systems (such as Microsoft Dynamics 365 or SAP) to track plant-level performance, production orders, machine downtime, inventory movement, quality control, and cost tracking across regions.

 Project Status: In Progress — dataset generation complete; data modeling and dashboards in development.

Table of Contents

Project Overview

Data Generation

Data Model Schema

Power BI Dashboards

Technologies Used

Folder Structure

Next Steps

 Project Overview

This solution aims to replicate a realistic manufacturing BI scenario by:

Creating large, relational datasets representing production, inventory, cost, machine events, and quality logs

Modeling ERP-style schema in SQL

Building intuitive Power BI dashboards for executive, plant-level, and operational users

🧪 Data Generation

Synthetic data was generated using Python (faker, pandas, numpy). Tables include:

Dimension tables: Plants, Products, Operators, Machines, Fault Types, Shifts, Calendar Dates

Fact tables: Production Orders, Quality Logs, Machine Downtime Events, Cost Journals, Inventory Movements

The data generator script is located in the /notebooks directory under 01_data_generation.ipynb.

Output files are saved in the /datasets/ folder.

🗃️ Data Model Schema

A star-schema model with 7 dimensions and 5 fact tables.

SQL schema file (under /sql/schema.sql) is optimized for Azure SQL or PostgreSQL

Foreign key constraints and indexing for performance and joins

Schema highlights best practices in ERP BI data warehousing. Business Intelligence Dashboards

The final dashboard will include:

Production Efficiency Overview

Cost vs. Standard Cost Analysis

Machine Downtime & Fault Diagnosis

Quality Defect Heatmaps & Trends

Inventory Movement by Plant & Product

Files will be available in the /powerbi folder as .pbix or .pbit templates.

Technologies Used

Python – Data generation with Faker, Pandas, NumPy

SQL – Schema modeling and queries

Power BI – Dashboards and KPI visualizations

Jupyter Notebook – Interactive scripting and documentation

GitHub – Version control and delivery
