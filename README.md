# Traffic Collision Analysis and Dashboard

## Project Overview
This project focuses on analyzing traffic collision data to uncover actionable insights that can help improve road safety. By leveraging Python for data processing, SQLite for data storage, and Power BI for visualization, the project implements an end-to-end ETL (Extract, Transform, Load) pipeline. The final output includes a dynamic, interactive BI dashboard that highlights trends, patterns, and critical factors contributing to road traffic collisions.

---

## Key Objectives
- **Data Cleaning and Transformation**: Address inconsistencies, missing values, and redundant information in raw datasets to ensure reliability and accuracy.
- **Data Warehouse Development**: Implement a star schema for efficient querying and reporting.
- **Data Analysis**: Extract insights on collision trends, casualty severity, environmental factors, and vehicle involvement.
- **Data Visualization**: Build an interactive Power BI dashboard to present insights effectively.

---

## Project Features

### ETL Pipeline
Comprehensive process to extract, clean, transform, and load data into a structured format.

### Star Schema Design
A central fact table connected to six dimension tables:
- **Location**
- **Date**
- **Road**
- **Vehicles**
- **Conditions**
- **Casualties**

### Interactive Dashboard
Power BI visualizations for dynamic exploration of collision data, including:
- Collision trends over time
- Geospatial analysis of accident hotspots
- Environmental and road condition impacts
- Casualty severity and demographic analysis
- Vehicle involvement patterns

---

## Technologies Used
- **Python**: Data cleaning, transformation, and preparation using libraries such as `pandas`, `numpy`, and `sqlite3`.
- **SQLite**: Lightweight database for data storage and querying.
- **Power BI**: BI tool for creating dynamic dashboards and visualizations.
- **CSV and JSON**: Data file formats for raw input and intermediate transformations.

---

## Dataset
- **Source**: Synthetic datasets simulating traffic collisions for 2019 and 2020.
- **Structure**:
  - **2019 Data**: CSV format with detailed collision records.
  - **2020 Data**: JSON format representing additional collision data.

---

## Key Files

### ETL Process
- **`data_cleaning.py`**: Script for data cleaning and transformation.
- **`schema_creation.sql`**: SQL script for creating the star schema in SQLite.
- **`data_loading.py`**: Script for populating tables with cleaned data.

### Data Files
- **`Accidents-2019.csv`**: Raw collision data for 2019.
- **`CalderdaleCollisions2020.json`**: Raw collision data for 2020.
- **`Casualties_Dimension.csv`**: Cleaned dimension table for casualties.
- **`Collisions_Fact.csv`**: Cleaned fact table.

### Visualization
- **`PowerBI_Dashboard.pbix`**: Power BI dashboard file.

---

## How to Run the Project

### Step 1: Set Up the Environment
1. Clone this repository:
    ```bash
    git clone https://github.com/yourusername/traffic-collision-analysis.git
    cd traffic-collision-analysis
    ```
2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

### Step 2: Execute the ETL Process
1. Run `data_cleaning.py` to clean and transform raw datasets:
    ```bash
    python data_cleaning.py
    ```
2. Create the SQLite database and schema using `schema_creation.sql`.
3. Populate tables with cleaned data using `data_loading.py`.

### Step 3: Visualize Data
1. Open `PowerBI_Dashboard.pbix` in Power BI.
2. Explore interactive visualizations and insights.

---

## Key Insights
- **Seasonal Trends**: Traffic collisions peaked during winter months, particularly on weekdays.
- **Weather Impact**: Rain and snow significantly increased the likelihood of accidents.
- **Casualty Severity**: Pedestrians and motorcyclists experienced a higher rate of serious injuries.
- **Geospatial Hotspots**: Urban areas with high traffic density emerged as collision hotspots.

---

## Future Work
- Integrate real-time data feeds for dynamic updates.
- Incorporate predictive analytics for forecasting accident trends.
- Enhance dashboard functionality for mobile accessibility.

---

## Contributing
Contributions are welcome! If you have ideas for improvement or new features, feel free to fork the repository and submit a pull request.

---

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## Acknowledgments
- The datasets used are synthetic and designed for educational purposes.
- Special thanks to the open-source tools and libraries that made this project possible.



