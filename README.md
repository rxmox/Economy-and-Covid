# COVID-19 Economic Impact Analysis

An interactive Python application that analyzes the economic impact of COVID-19 across US states, combining public health data with economic indicators to reveal pandemic trends and regional disparities.

## Overview

This data analysis tool processes and visualizes multi-source datasets to help understand how the COVID-19 pandemic affected different states economically. By integrating COVID-19 statistics with unemployment rates, income data, and demographics, the application provides comparative insights through interactive visualizations.

## Key Features

### COVID-19 Analysis
- **Comprehensive Statistics**: View total cases, deaths, confirmed vs. probable cases for any US state
- **Population-Based Metrics**: Calculate infection and mortality rates relative to state population
- **Comparative Visualizations**: Automatic bar chart comparisons with states having highest/lowest case counts
- **Real-Time Context**: Displays last updated date for COVID data

### Economic Impact Analysis
- **Per Capita Income Tracking**: Compare 2019 vs. 2020 per capita personal income changes
- **Unemployment Trends**: Visualize unemployment rate shifts during the pandemic year
- **Year-over-Year Analysis**: Dual subplot graphs showing economic indicator trends
- **Impact Assessment**: Quantifies economic changes with percentage calculations

### User Experience
- **Flexible Input**: Accept state names or two-letter state codes
- **Interactive Terminal Interface**: Simple menu-driven navigation
- **Smart Validation**: Input validation with helpful error messages
- **Dynamic Visualizations**: Auto-generated matplotlib charts based on data patterns

## Technical Highlights

**Data Processing**
- NumPy array operations for efficient multi-file data manipulation
- Custom indexing algorithms for cross-referencing datasets
- Dynamic data type handling (string/numeric conversion)

**Object-Oriented Design**
- `Area` class encapsulating state information
- Modular helper functions for reusable data operations

**Visualization**
- Conditional plotting logic based on comparative analysis
- Matplotlib subplots for multi-metric visualization
- Custom formatting for improved readability

## Tech Stack

- **Python 3.x** - Core programming language
- **NumPy** - Array operations and numerical processing
- **Matplotlib** - Data visualization and plotting
- **Pandas** - Listed as dependency (available for extensions)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/covid-economic-impact-analysis.git
cd covid-economic-impact-analysis
```

2. Install required dependencies:
```bash
pip install numpy matplotlib pandas
```

3. Run the application:
```bash
python Final_project.py
```

## Usage

1. **Select a State**: Enter either the full state name (e.g., "California") or state code (e.g., "CA")
2. **Choose Analysis Type**:
   - **A** - COVID-19 statistics and health impact
   - **B** - Economic indicators and trends
3. **View Results**: The application displays statistics and generates comparison visualizations

### Example Session
```
Please select a US State: New York

***Requested Area Information***
State: New York
State Code: NY
Region: Northeast

Choose a letter corresponding to a topic:
    A - Covid
    B - Economics
```

## Data Sources

This project integrates data from authoritative public sources:

- **COVID-19 Data**: [NYTimes COVID-19 Dataset](https://github.com/nytimes/covid-19-data)
- **Unemployment Statistics**: [U.S. Bureau of Labor Statistics](https://www.bls.gov/lau/)
- **Demographics**: [USDA Economic Research Service](https://data.ers.usda.gov/)
- **Per Capita Income**: [FRED Economic Data](https://fred.stlouisfed.org/)
- **State Mapping**: [Kaggle US States Dataset](https://www.kaggle.com/)

## Dataset Structure

| File | Description | Key Columns |
|------|-------------|-------------|
| `covid.csv` | COVID-19 cases and deaths | date, state, cases, deaths, confirmed/probable breakdowns |
| `unemployment.csv` | Unemployment rates | state, 2019 rate, 2020 rate |
| `state_per_capita.csv` | Per capita personal income | state, 2019 income, 2020 income |
| `state_demographics.csv` | Population by decade | state, population (1990-2020) |
| `states_to_region.csv` | State metadata | state, code, region, division |

## Skills Demonstrated

- **Data Integration**: Merging multiple CSV datasets with different schemas
- **Statistical Analysis**: Calculating percentages, trends, and comparative metrics
- **Data Visualization**: Creating meaningful charts from complex datasets
- **User Interface Design**: Building intuitive terminal-based interactions
- **Input Validation**: Robust error handling and user guidance
- **Code Organization**: Clean, documented, maintainable code structure
- **Problem Solving**: Translating real-world questions into data queries

## Future Enhancements

- Add time-series analysis for COVID trends over multiple months
- Include vaccination rate data and correlations
- Export analysis reports to PDF/CSV
- Web-based dashboard interface
- Machine learning predictions for economic recovery
- Regional comparison views (e.g., all Western states)

## Project Context

Developed as a final project for ENDG 233 (Computing for Engineers) at the University of Calgary, Fall 2021. This project demonstrates proficiency in Python programming, data analysis, and visualization techniques applied to real-world pandemic data.

---

*Data accurate as of November 2021. This is an educational project showcasing data analysis and visualization capabilities.*
