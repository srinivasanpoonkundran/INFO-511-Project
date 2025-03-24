# FBI Crime Data Analysis

## Project Title:
**Data Visualization of FBI Crime Data Agencies**

## Author:
Srinivasan Poonkundran  

## Research Question:
- How do agency types vary across different states in the USA?
- What percentage of agencies in each state participate in NIBRS reporting?
- Are there observable trends in NIBRS adoption over time?

## Dataset:
- **Source:** [TidyTuesday - 2025-02-18](https://github.com/rfordatascience/tidytuesday/tree/main/data/2025/2025-02-18)
- **Description:**  
  Agency-level data for all 50 U.S. states.  
  Includes details on law enforcement agencies submitting data to the FBI’s Uniform Crime Reporting (UCR) Program, visible on the Crime Data Explorer (CDE).

### Key Variables (agencies.csv):
| Variable         | Type       | Description                                                             |
|------------------|-----------|-------------------------------------------------------------------------|
| ori              | character | Unique ID to identify an agency                                         |
| county           | character | County linked to the agency’s jurisdiction within a state               |
| latitude         | double    | Approximate latitude of the agency’s location                           |
| longitude        | double    | Approximate longitude of the agency’s location                          |
| state_abbr       | character | Two-letter state abbreviation                                           |
| state_name       | character | Full state name                                                         |
| agency_name      | character | Name of the law enforcement agency                                      |
| agency_type_name | character | Type of agency (e.g., city police, sheriff's office)                     |
| nibrs_start_date | date      | Date when the agency began NIBRS participation                          |
| nibrs            | logical   | Whether the agency participates in NIBRS (TRUE/FALSE)                   |

## Project Workflow:

1. **Data Cleaning:**  
   Handled missing values, corrected column types, and filtered unnecessary data.
   
2. **Exploratory Data Analysis (EDA):**  
   - Count of agency types per state
   - Percentage of NIBRS participation by state
   - Trends in NIBRS adoption over the years

3. **Visualizations:**
   - Bar charts for agency types distribution
   - Heatmaps to show NIBRS participation across states
   - Line graphs for trend analysis

## Tools Used:
- Python (Pandas, Matplotlib, Seaborn)
- Jupyter Notebook

## How to Run:
1. Clone this repository.
2. Install dependencies:
   ```
   pip install pandas matplotlib seaborn notebook
   ```
3. Open and run `fbi_crime_data_analysis.ipynb` in Jupyter Notebook.

## Insights:
- Significant variation in agency types by state.
- Some states have higher NIBRS participation.
- Steady increase in NIBRS adoption over time.
