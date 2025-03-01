# Health Monitoring System

## Overview
The **Health Monitoring System** is a data analytics project designed to analyze and visualize patient health data using various data science tools and technologies. The system reads patient data, calculates average health parameters, and presents the results using interactive dashboards.

## Tech Stack
- **Python**: Primary programming language
- **Pandas**: Data manipulation and analysis
- **PySpark**: Distributed data processing
- **Seaborn**: Statistical data visualization
- **Plotly**: Interactive data visualization
- **Dash**: Web-based dashboard
- **Google Colab**: Platform for running code online


## Prerequisites
- Install required libraries:
```bash
!pip install pyngrok dash plotly pyspark seaborn
```

## File Upload
The system expects a CSV file named `patients.csv` containing patient health data. The file can be uploaded using Google Colab's file upload functionality.

### Example CSV Columns:
- BP
- Sugar_Level
- Cholesterol
- Haemoglobin

## How It Works
1. **Initialize Spark Session**: Creates a Spark session for distributed data processing.
2. **Load Data**: Reads the patient data using Pandas.
3. **Convert Data**: Transforms the Pandas DataFrame into a Spark DataFrame.
4. **Data Overview**: Prints the schema and sample data.
5. **Average Calculation**: Calculates average values for key health parameters using PySpark.
6. **Visualization**:
    - Seaborn for static bar plots.
    - Plotly and Dash for interactive dashboards.

## Running the Project
1. Upload `patients.csv` using Google Colab.
2. Run all cells in the notebook.

## Folder Structure
```plaintext
.
├── patients.csv        # Patient health data
├── app.py             # Main script
└── README.md          # Documentation
```

## Output
- Console Output:
  - Total patient count
  - Data schema
  - Sample patient data
- Visualizations:
  - Static bar plot (Seaborn)
  - Interactive dashboard (Dash + Plotly)

## Notes
- Ensure that the column names in the CSV file match the expected schema.
- The dashboard can be extended with additional health metrics and visualizations.

