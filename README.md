# Objective
Create a Data Warehouse (DWH) to extract AWS reviews for products/categories and provide average ratings per category, along with analysis/trends of review ratings per brand in each category.

# Goals
## Business Goals
1. Query metrics:
   - Average review rating per category per month.
   - Analysis of review ratings per brand per month.

## Technical Goals
1. Implement ETL scripts to extract, transform, and load the data into the DWH.

# Measures and Targets
1. Success will be measured by the ability to run the required queries and obtain results within 5 seconds.
2. Completion of the DWH model, ETL scripts, and data quality checks.

# Requirements
## Functional Requirements
1. The DWH must support querying average review ratings per category and brand.
2. ETL scripts must handle data extraction from CSV files and load it into the DWH.
3. Data quality checks must be implemented to ensure data integrity.

## Non-Functional Requirements
1. **Performance**: Queries must return results in under 5 seconds.
2. **Scalability**: The system should handle a 10x increase in data volume.
3. **Reliability**: The DWH should be available 99.9% of the time.

# How to Do It
## Technical Instructions
*Instructions to be defined here...*

# Tech-Stack Choices
1. **Extraction Tool**: Yet to decide [Not a core Requirement]
2. **PostgreSQL for DWH**
   - a. Physical Model
   - b. Logical Model
   - c. ERD
   - d. Data Modelling
   - e. Meta Data Management
   - f. Schema Evolution
   - g. Change Data Capture
     - i. SCD 1, 2
     - ii. Incremental Loads
     - iii. Full Loads
   - h. Facts and Dimensions
   - i. Data Quality Checks
3. **Reporting**: Yet to decide [Not a core Requirement]

---

# Relevance
The DWH and ETL processes will support business intelligence and analytics for the Clothing, Shoes, and Jewelry category, providing valuable insights for decision-making.

---

# Time-Bound: 4 Days
## Day 1
### Half Day
- **Requirement Analysis**
- **Problem Solving Framework** (SMART)
- **High-Level Design**
  - Data Requirements
    - Physical & Logical Modelling
    - ERD diagram
    - Modelling
    - Facts and Dimensions
  - Technical Requirements
    - ETL Tool choice
    - Database Choice
    - Presentation Choice
  - Quality Checks
  - Meta Data Management

### Next Half
1. Flow Diagram
2. Segregation of Functional and Non-Functional Requirements
3. Architecture
4. Tech-stack (choice made)

---

## Day 2: Design and Code
### Design
1. Extraction of data
2. Load
3. Testing on load failures
4. DWH - CDC, SCD 1, 2 Implementation Using Kimball
5. Data Quality Checks
6. Testing
7. Business Requirements
   1. Query: Average Review (Join Product Table with Product Details)
   2. Query: Analysis Review (Join Product Table with Product Details, Brand Table with Brand Details)
