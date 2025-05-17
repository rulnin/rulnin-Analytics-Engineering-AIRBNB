# 🏠 Airbnb Analytics Engineering Project – Berlin

This project showcases an end-to-end data pipeline designed by an Analytics Engineer to extract, transform, and load Airbnb listing data for Berlin using Snowflake and dbt (data build tool). The data source is from [Inside Airbnb](https://insideairbnb.com/berlin/).

## 🚀 Overview

As an Analytics Engineer at Airbnb, the goal of this project is to:

- Ingest raw Airbnb data from [Inside Airbnb](https://insideairbnb.com/berlin/)
- Load the data into Snowflake
- Perform data modeling and transformation using dbt
- Store the clean, analytics-ready data back into Snowflake for downstream analysis and dashboards

## Data entry scheme
![DBT2](https://github.com/user-attachments/assets/da21b3b2-0574-437a-8ee6-d441aae1f6ef)

## Transformation data flow
![dbt](https://github.com/user-attachments/assets/197d73f0-6834-4a90-8503-30790e850e43)


## 🧱 Tech Stack

- **Snowflake**: Cloud data warehouse for scalable data storage and querying
- **dbt**: Transformation and modeling of raw data using SQL-based pipelines
- **Python** *(optional)*: For orchestration or loading scripts
- **Inside Airbnb Dataset**: Open-source Airbnb data for Berlin

## 📊 Data Source

All data is sourced from the public dataset provided by [Inside Airbnb – Berlin](https://insideairbnb.com/berlin/). This dataset includes listings, calendar availability, and reviews for Berlin Airbnb properties.

## 🔄 Workflow

1. **Extract & Load**  
   Download the Berlin dataset and load it into a Snowflake raw schema (e.g., `RAW.LISTINGS`).

2. **Transform**  
   Use dbt to:
   - Clean and structure the raw data in staging models
   - Create analytics-friendly models in the marts layer
   - Add documentation and tests to ensure data quality

3. **Analytics Ready**  
   The final dbt models reside in a Snowflake schema (e.g., `ANALYTICS.LISTINGS_MART`) and are ready to power BI tools or ad-hoc analysis.

## ✅ Features

- Modular dbt models following best practices
- Data quality checks using dbt tests
- Version-controlled transformations
- Easily extensible to other cities or datasets from Inside Airbnb

## 📈 Example Use Cases

- Analyze trends in Airbnb availability and pricing
- Explore distribution of listings by neighborhood
- Identify seasonal occupancy patterns
