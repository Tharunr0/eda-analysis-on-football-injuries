# Player Injuries Impact on Match Performance

## Project Overview
This project performs an exploratory data analysis (EDA) on a dataset that contains player injury information and its potential impact on match performance. The goal is to investigate how injuries influence player statistics, performance ratings (FIFA ratings), and other factors such as age and position.

## Data Description
The dataset used in this analysis contains information about various player injuries, including injury type, date of injury, date of return, and player-related data such as FIFA ratings, age, and position. The analysis seeks to understand:
- The types and frequencies of injuries.
- The impact of injury duration on FIFA ratings and performance.
- Relationships between player age, position, and injury impacts.

## Steps Involved

### 1. Loading and Inspecting the Data
The data is first loaded into a pandas DataFrame, followed by an inspection of its structure and summary statistics.

### 2. Data Cleaning
- **Handling Missing Values**: Missing values are handled, and `NaN` values are replaced with 'N.A.'.
- **Standardizing Injury Names**: Injury names are standardized to avoid inconsistencies (e.g., "hamstring injury" is replaced with "hamstring").
- **Data Type Conversion**: Columns are converted to appropriate data types (e.g., `Age`, `FIFA rating`, and date columns).
- **Removing Duplicates**: Any duplicate rows are removed.

### 3. Exploratory Data Analysis (EDA)
- **Summary Statistics**: A summary of the data is generated to get an overview of the player injuries and their statistics.
- **Correlation Analysis**: A correlation matrix is calculated to explore potential relationships between numeric columns.

### 4. Visualization
Several visualizations are generated to present the data:
- **Distribution of Player Ages**: A histogram and kernel density estimate (KDE) plot to show the distribution of player ages.
- **FIFA Rating by Position**: A boxplot to explore how FIFA ratings vary across player positions.
- **Top Injuries by Count**: A bar plot showing the top 20 most common injury types.
- **Injury Duration vs. FIFA Rating**: A scatter plot to explore the relationship between the injury duration and FIFA rating.

## Installation

To run this analysis, you'll need the following Python libraries:
- pandas
- numpy
- matplotlib
- seaborn

You can install them using pip:

```bash
pip install pandas numpy matplotlib seaborn
