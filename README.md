## San Francisco Crime Analysis and Prediction
Overview
This repository contains a comprehensive analysis and predictive modeling of crime data in San Francisco. The project includes:

Data cleaning and preprocessing of raw crime records

Exploratory data analysis with visualizations

Feature engineering for temporal and spatial patterns

Multiple machine learning models for crime category prediction

Interactive maps and dashboard visualizations

Dataset
The dataset used is from the SF Crime Classification competition, containing:

878,049 crime records (after cleaning)

Features include:

Crime category (target variable)

Police district

Location coordinates (X, Y)

Date and time features

Crime description

Resolution status

Key Features
Data Cleaning
Handling missing values

Removing duplicate records

Filtering invalid spatial coordinates

Temporal feature extraction (hour, day, month, etc.)

Exploratory Analysis
Crime frequency by time (hour, day, month)

Spatial distribution of crimes

Most common crime categories

District-wise crime patterns

Machine Learning
Multiple models implemented:

Random Forest

Decision Tree

K-Nearest Neighbors

Naive Bayes

Feature importance analysis

Model performance comparison

Visualizations
Interactive heatmaps of crime locations

Temporal patterns dashboard

Model performance charts

Feature importance plots

File Structure
sf-crime-analysis/
├── data/
│   ├── train.csv                # Raw data
│   └── sf_crime_cleaned.csv     # Cleaned data
├── notebooks/
│   └── SF_Crime_Analysis.ipynb  # Main analysis notebook
├── visualization/
│   ├── crime_by_day.png         # Crime frequency by day
│   ├── crime_by_hour.png        # Crime frequency by hour
│   ├── crime_by_month.png       # Crime frequency by month
│   ├── crime_spatial_distribution*.png  # Spatial plots
│   ├── coordinates_boxplot*.png # Coordinate distributions
│   ├── sf_crime_dashboard.png   # Summary dashboard
│   ├── sf_crime_heatmap.html    # Interactive heatmap
│   └── sf_crime_map.html        # Interactive crime map
├── models/
│   └── [saved_model_files].pkl  # Trained model files
├── README.md                    # This file
└── requirements.txt             # Python dependencies
Usage
Install dependencies:

bash
pip install -r requirements.txt
Run the Jupyter notebook:

bash
jupyter notebook SF_Crime_Analysis.ipynb
For prediction with preprocessed input:

python
# Example prediction code included in notebook
Key Findings
Random Forest achieved the best prediction accuracy

Temporal patterns show clear daily/weekly cycles

Spatial analysis reveals crime hotspots

Feature importance highlights key predictors

Dependencies
Python 3.7+

pandas, numpy

scikit-learn

matplotlib, seaborn

folium (for interactive maps)

jupyter

License
This project is licensed under the MIT License.

Acknowledgements
Data source: SF Crime Classification
