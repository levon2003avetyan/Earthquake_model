# Earthquake_model
Earthquake Data Analysis Project
Project Overview

This project analyzes earthquake data obtained from the U.S. Geological Survey (USGS). The USGS monitors and reports earthquakes globally, providing real-time scientific information. The dataset contains details of all earthquakes recorded in the last 30 days, including magnitude, depth, location, and other relevant attributes.

The goal of this project is to perform exploratory data analysis (EDA), data cleaning, and feature engineering to understand earthquake patterns and distributions.

Dataset Description

Source: USGS Earthquake Catalog (link
)

Update frequency: Weekly (data originally updated every 15 minutes)

Number of records: 9639 earthquakes

Key columns:

time – date and time of the earthquake

latitude / longitude – geographic coordinates

depth – depth below the surface (km)

mag – magnitude of the earthquake

place – description of location

magType – method used to calculate magnitude

state – extracted from the place column for regional analysis

Steps Performed

Data Cleaning

Removed or imputed missing values in critical columns.

Filtered out invalid entries where necessary.

Exploratory Data Analysis (EDA)

Visualized the distribution of magnitudes using histograms.

Analyzed earthquake depth distribution and created depth categories (Shallow, Intermediate, Deep).

Plotted magnitude vs depth scatter plots.

Created geographical plots using latitude and longitude.

Generated frequency distributions for states and magnitude categories.

Feature Engineering

Created a new column depth_category:

Shallow: 0–70 km

Intermediate: 70–300 km

Deep: >300 km

Extracted state from the place column to analyze regional patterns.

Key Findings

Most earthquakes occur in shallow depths (<70 km), especially near tectonically active regions.

Magnitude distribution shows a majority of small earthquakes; large-magnitude events are rare.

Certain regions (e.g., California, Alaska) experience more frequent earthquakes.

3D visualization highlights clusters of earthquakes by latitude, longitude, and depth, with magnitude intensity represented by color.

Tools & Libraries

Python 3

Pandas – data cleaning and manipulation

NumPy – numerical operations

Matplotlib & Seaborn – visualization

Scipy – interpolation for 3D plots

Repository Structure

Earthquake_EDA.ipynb – main Jupyter notebook with all analysis and visualizations

data/earthquakes.csv – raw earthquake dataset

README.md – project description and methodology

How to Run

Clone the repository.

Install required packages:

pip install pandas numpy matplotlib seaborn scipy


Open Earthquake_EDA.ipynb in Jupyter Notebook.

Run all cells to reproduce the analysis and plots.

Notes

This analysis focuses on data visualization, exploration, and feature engineering.

All plots are included in the notebook, with professional and exam-ready explanations.

The project can be extended to include predictive modeling or interactive visualizations using Plotly or Dash.



# Conclusion

In this project, we analyzed earthquake data from the USGS for the last 30 days. The main steps included data cleaning, exploratory data analysis (EDA), and feature engineering. Key observations and insights are as follows:

1. Most earthquakes occur at **shallow depths (<70 km)**, concentrated in tectonically active regions such as California and Alaska.  
2. The **magnitude distribution** shows that small earthquakes are common, while strong earthquakes are rare.  
3. Creating the `depth_category` and `state` columns allowed for **categorical analysis** and easier interpretation of earthquake patterns.  
4. 3D and geographic analyses revealed **clusters and hotspots** of earthquakes, showing how magnitude, latitude, longitude, and depth interact.  
5. Columns representing measurement uncertainty (`horizontalError` and `depthError`) were examined but **not used in modeling**, as they describe data reliability rather than earthquake characteristics.  

Overall, this analysis demonstrates how cleaning, feature engineering, and careful visualization can help understand earthquake patterns and identify high-risk regions. The notebook is prepared to be easily extended for **predictive modeling or interactive visualization** in the future.
