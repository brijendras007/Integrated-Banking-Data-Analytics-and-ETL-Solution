# Integrated Banking Data Analytics and ETL Solution

## Project Overview

This project demonstrates an end-to-end Data Science solution focused on integrating and analyzing banking customer data. The aim is to create a comprehensive **Master Table** that consolidates multiple datasets into a single source of truth, providing a unified view of all client-related information. This table will support various analyses, reporting, and decision-making processes.

## Problem Statement and Business Goals

To streamline data management and improve data accessibility, this project aims to:
1. Store real-time raw data in a staging area (Database).
2. Perform ETL (Extract, Transform, Load) operations to clean, transform, and integrate data.
3. Create a **Master Table** that unifies multiple data sources, enabling deeper analysis and insights into bank operations and customer interactions.

## Datasets Description

The data consists of various relations detailing aspects of clients, their accounts, transactions, loans, credit cards, and demographic information:

- **Account Data (`ACCOUNT.ASC`)** - 4500 records describing static characteristics of bank accounts.
- **Client Data (`CLIENT.ASC`)** - 5369 records describing client characteristics.
- **Disposition Data (`DISP.ASC`)** - 5369 records mapping the rights of clients to operate accounts.
- **Permanent Order Data (`ORDER.ASC`)** - 6471 records describing characteristics of payment orders.
- **Transaction Data (`TRANS.ASC`)** - 1,056,320 records detailing transactions on accounts.
- **Loan Data (`LOAN.ASC`)** - 682 records describing loans granted for accounts.
- **Credit Card Data (`CARD.ASC`)** - 892 records describing credit cards issued to accounts.
- **Demographic Data (`DISTRICT.ASC`)** - 77 records describing demographic characteristics of various districts.

## Data Relationships

- Each account has static characteristics (e.g., date of creation, branch address) from the "account" dataset and dynamic characteristics (e.g., transactions, balances) from "transaction" and "order" datasets.
- "Client" data describes individuals who can manipulate accounts. Multiple clients can be associated with a single account and vice versa. This relationship is mapped in the "disposition" dataset.
- "Loan" and "credit card" data provide details on banking services. A single account may have multiple credit cards, but only one loan at most.
- "Demographic data" provides additional context such as unemployment rates and other public information about districts, adding depth to client analysis.

## Methodology

### 1. Data Preparation

- **Data Import:** Load all datasets (`ACCOUNT.ASC`, `CLIENT.ASC`, `DISP.ASC`, `ORDER.ASC`, `TRANS.ASC`, `LOAN.ASC`, `CARD.ASC`, `DISTRICT.ASC`) into the staging area.
- **Data Cleaning:** 
  - Identify and handle missing values.
  - Remove duplicate records.
  - Ensure data consistency and accuracy.

### 2. Data Integration

- **Entity Mapping:** Map relationships between datasets based on common identifiers (e.g., client IDs, account IDs).
- **Master Table Creation:** Integrate all datasets to form a Master Table, ensuring all client IDs and related data are included.

### 3. Data Analysis

- **Exploratory Data Analysis (EDA):** Analyze data distributions, patterns, and relationships using visualizations.
- **Feature Engineering:** Identify and transform relevant features, handle outliers, and encode categorical variables.

### 4. ETL Process

- **Extract:** Extract data from various sources.
- **Transform:** Clean and format the data to ensure uniformity.
- **Load:** Load the transformed data into the Master Table.

### 5. Model Building and Validation

- **Build Models:** Validate the completeness and accuracy of the Master Table.
- **Check Data Quality:** Ensure data consistency and correctness against business rules.
- **Testing:** Run queries and generate reports to confirm the table's functionality.

### 6. Model Output and Documentation

- **Save the Master Table:** Store the final table in an appropriate format (e.g., CSV, Excel).
- **Documentation:** Provide thorough documentation of processes, transformations, and results.

## Results and Conclusions

- Successfully integrated and consolidated multiple datasets into a single Master Table.
- Ensured high data quality through a comprehensive cleaning and transformation process.
- The Master Table serves as a powerful resource for bank data analysis, supporting improved decision-making and reporting.

## Usage

### Prerequisites

- Python 3.8 or above
- Necessary libraries: pandas, numpy, matplotlib, seaborn

### Installation

Clone this repository and install the required packages:

```bash
git clone https://github.com/brijendras007/Integrated-Banking-Data-Analytics-and-ETL-Solution.git
cd Integrated-Banking-Data-Analytics-and-ETL-Solution
pip install -r requirements.txt
Running the Project
Import the datasets into your environment.
Follow the data cleaning, integration, and analysis steps as detailed in the Jupyter notebooks provided.
Testing
Test the Master Table using queries and sample data to verify its accuracy and completeness.
Contribution
Contributions are welcome! Feel free to fork the repository, raise issues, or submit pull requests to enhance the project.

License
This project is licensed under the MIT License - see the LICENSE file for details.
