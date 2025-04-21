# Steam Games Dashboard 🎮

This repository contains a Power BI report analyzing Steam games data.

🔗 **Live Dashboard**: [View Power BI Report](https://mateuszmachowina.github.io/power-bi/)  
_(Requires access to the author's Power BI organization - SGH Warsaw School of Economics)_

📁 **Data & Report Files** (PBIX & CSV):  
[Google Drive Folder](https://drive.google.com/drive/folders/1Smgei-yGqcSntVgs0tvGWv3of1qJM29V?usp=sharing)

📄 **Original Dataset**:  
[Steam Games Dataset on Kaggle by Mexwell](https://www.kaggle.com/datasets/mexwell/steamgames)

## Files in this Repository

- `steam-games-dashboard-overview.pdf` – Screenshots with dashboard overview
- `index.html` – Embeds the published Power BI dashboard (via iframe)

## Setup Instructions

1. **Download files** from the [Google Drive Folder](https://drive.google.com/drive/folders/1Smgei-yGqcSntVgs0tvGWv3of1qJM29V?usp=sharing)
   - `steam-games-dashboard.pbix`
   - `\data\games.csv`
   _Note: You can also download the dataset from the [original source on Kaggle](https://www.kaggle.com/datasets/mexwell/steamgames), but if the author changes the column layout, it may cause issues with the report._

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
   - **KPI Indicators** for key metrics like peak concurrent players, playtime and more.
   - **Tooltips** that show additional information when hovering over specific elements in the charts.
   - **Tree Maps, Bar Charts and Pie Charts** displaying data about the most popular games, genres and other relevant metrics.

![Steam Dashboard Demo](assets/steam-games-dashboard-overview.gif)

