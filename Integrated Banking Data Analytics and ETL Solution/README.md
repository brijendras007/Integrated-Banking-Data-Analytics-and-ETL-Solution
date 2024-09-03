# Bank Customer Data Analysis and Master Table Creation

## Background Information

This project involves analyzing real-time data from a bank to create a comprehensive Master Table. The data consists of multiple relations detailing various aspects of client and account interactions. The goal is to store the raw data in a staging area, perform ETL (Extract, Transform, Load) operations, and prepare a Master Table that consolidates all related information.

## Problem Statement and Business Goals

The task is to develop a Master Table by integrating several datasets related to clients, accounts, transactions, loans, credit cards, and demographic data. This Master Table will provide a unified view of all client-related information, helping in various data analyses and decision-making processes. The project aims to streamline data management and improve accessibility for further analytics.

## Methodology

### Data Preparation

1. **Data Import:**
   - Import the raw datasets: `ACCOUNT.ASC`, `CLIENT.ASC`, `DISP.ASC`, `ORDER.ASC`, `TRANS.ASC`, `LOAN.ASC`, `CARD.ASC`, `DISTRICT.ASC`.

2. **Data Cleaning:**
   - Check for missing values and handle them appropriately.
   - Remove any duplicate records.
   - Ensure data consistency and accuracy.

### Data Integration

1. **Entity Mapping:**
   - Map the relationships between the datasets based on common identifiers (e.g., client IDs, account IDs).

2. **Master Table Creation:**
   - Create a Master Table that integrates information from all datasets.
   - Ensure all client IDs are included and all related tables are considered.

### Data Analysis

1. **Exploratory Data Analysis (EDA):**
   - Perform EDA to understand data distributions, relationships, and patterns.
   - Visualize data using graphs and interpret the results.

2. **Feature Engineering:**
   - Identify relevant features and perform transformations as needed.
   - Encode categorical variables and handle outliers.

### ETL Process

1. **Extract:**
   - Extract data from various sources and staging areas.

2. **Transform:**
   - Apply necessary transformations to clean and format the data.

3. **Load:**
   - Load the transformed data into the Master Table.

### Model Building

- Develop models to validate the completeness and accuracy of the Master Table.
- Use appropriate metrics to assess data quality and consistency.

### Model Validation

1. **Check Data Quality:**
   - Validate the Master Table against expected outcomes and business rules.

2. **Model Testing:**
   - Test the Master Table by running queries and generating reports to ensure it meets the required specifications.

### Model Output Saving

1. **Save Master Table:**
   - Save the final Master Table in an appropriate format (e.g., Excel, CSV) for further use.

2. **Documentation:**
   - Document the process, transformations, and results.

## Conclusions

- The Master Table successfully integrates data from multiple sources, providing a unified view of client and account information.
- The data cleaning and integration process ensured high data quality and consistency.
- The final Master Table will support various analyses, reporting, and decision-making processes.

## Model Results

- The integrated Master Table serves as a comprehensive resource for analyzing client and account data.
- All related datasets have been successfully consolidated, providing a holistic view of bank operations and customer interactions.

## Test Data

- Test the Master Table with various queries and reports to ensure its functionality and accuracy.

## Contribution

- This project demonstrates the end-to-end process of data integration and master table creation, showcasing skills in data management, ETL processes, and data analysis.

Feel free to contribute further ideas or improvements to this project.

