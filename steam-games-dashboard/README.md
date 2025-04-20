# Steam Games Dashboard

## Overview
This is a Power BI dashboard that visualizes various statistics of Steam games. The data comes from the [Steam Games Dataset on Kaggle](https://www.kaggle.com/datasets/mexwell/steamgames). The report includes various key performance indicators (KPIs) such as average playtime, peak concurrent players, and more, displayed through interactive charts and tooltips.


🔗 **Live Dashboard**: [View Power BI Report](https://mateuszmachowina.github.io/power-bi/)  
_(Requires access to the author's Power BI organization - SGH Warsaw School of Economics)_

## Files Included
- **steam-games-dashboard.pbix**: The main Power BI report file.
- **steam-games-dashboard-overview.pdf**: A PDF overview of the dashboard with screenshots of the key visuals.
- **data/**: A folder containing the `games.csv` file, which is the main data source for the dashboard.

## Setup Instructions

1. **Download the Dataset**  
   The data is sourced from Kaggle. To get the data, download the `steamgames.csv` file from the following link:  
   [Steam Games Dataset on Kaggle](https://www.kaggle.com/datasets/mexwell/steamgames)

2. **Folder Path Configuration in Power BI**  
   The Power BI report uses a parameter called **FolderPath** to point to the location of the `games.csv` file. To make the report work on your machine:
   
   - Open the **steam-games-dashboard.pbix** file in Power BI Desktop.
   - Go to the **Home** tab and click on **Transform Data** to open Power Query Editor.
   - In Power Query Editor, locate the **FolderPath** parameter.
   - Change its value to the path where you saved the `games.csv` file on your computer. For example, on your machine, the current value is:
     ```
     C:\Users\NAME\Desktop\power-bi\steam-games-dashboard\data\
     ```
     Update this to match your local path to the `games.csv` file.

3. **Refresh Data**  
   Once the **FolderPath** is updated, you can refresh the data by clicking **Refresh** in Power BI Desktop.

4. **Visualizing the Data**  
   The dashboard includes several interactive visualizations:
   - **KPI Indicators** for key metrics like peak concurrent players, playtime, and more.
   - **Tooltips** that show additional information when hovering over specific elements in the charts.
   - **Tree Maps, Bar Charts, and Pie Charts** displaying data about the most popular games, genres, and other relevant metrics.
