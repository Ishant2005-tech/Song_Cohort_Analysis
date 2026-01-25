# Song Cohort Analysis

This project explores how songs can be grouped into meaningful cohorts using their audio features. 
The goal was to understand patterns in music data and apply unsupervised learning techniques in a practical way.


## Project Overview

This project performs exploratory data analysis, feature engineering, PCA dimensionality reduction, and K-means clustering on a song dataset to identify distinct cohorts of songs with similar audio characteristics.

## Why this project

I built this project to practice a complete data analysis workflow on a real-world style dataset.
It focuses on understanding audio features, applying PCA, and using clustering to uncover patterns
that could be useful for music recommendation or playlist grouping.

## Directory Structure

```
song-cohort-analysis/
│
├── data/
│   ├── raw/                    # Original, untouched dataset
│   │   └── songs.csv
│   │
│   ├── processed/              # Cleaned / feature-engineered data
│   │   ├── songs_cleaned.csv
│   │   └── songs_pca.csv
│
├── notebooks/                  # Jupyter notebooks (experiments)
│   ├── 01_data_loading.ipynb
│   ├── 02_eda.ipynb
│   ├── 03_feature_engineering.ipynb
│   ├── 04_pca.ipynb
│   ├── 05_clustering.ipynb
│   └── 06_cohort_analysis.ipynb
│
├── src/                        # Reusable Python scripts
│   ├── __init__.py
│   ├── data_preprocessing.py
│   ├── eda.py
│   ├── pca_utils.py
│   ├── clustering.py
│   └── cohort_analysis.py
│
├── images/                     # All plots & visual outputs
│   ├── eda/
│   │   ├── popularity_dist.png
│   │   └── danceability_vs_energy.png
│   │
│   ├── clustering/
│   │   ├── elbow_curve.png
│   │   ├── silhouette_score.png
│   │   └── cluster_visualization.png
│   │
│   └── cohort/
│       └── cohort_heatmap.png
│
├── models/                     # Saved ML models
│   └── kmeans_model.pkl
│
├── reports/                    # Final outputs
│   └── song_cohort_analysis_report.pdf
│
├── README.md                   # Project documentation
├── requirements.txt            # Python dependencies
├── .gitignore                  # Files to ignore
└── LICENSE                     # License information
```

## Getting Started

### Prerequisites

- Python 3.8 or higher
- pip or conda

### Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd song-cohort-analysis
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

### Usage

1. **Data Loading**: Start with `notebooks/01_data_loading.ipynb` to load and inspect the raw data
2. **EDA**: Run `notebooks/02_eda.ipynb` for exploratory data analysis
3. **Feature Engineering**: Execute `notebooks/03_feature_engineering.ipynb` to create features
4. **PCA**: Apply dimensionality reduction in `notebooks/04_pca.ipynb`
5. **Clustering**: Perform K-means clustering in `notebooks/05_clustering.ipynb`
6. **Analysis**: Generate cohort analysis in `notebooks/06_cohort_analysis.ipynb`

## Key Scripts

- `src/data_preprocessing.py` - Data cleaning and preparation
- `src/eda.py` - Exploratory data analysis functions
- `src/pca_utils.py` - PCA-related utilities
- `src/clustering.py` - K-means clustering utilities
- `src/cohort_analysis.py` - Cohort analysis and reporting

## Outputs

- **Processed Data**: `data/processed/` contains cleaned and feature-engineered datasets
- **Visualizations**: All plots and charts are saved in `images/`
- **Models**: Trained models are saved in `models/`
- **Reports**: Final analysis report is in `reports/`

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Key Insights

- Songs naturally formed distinct clusters based on energy, tempo, and danceability
- PCA helped reduce feature complexity while preserving most of the variance
- Some clusters represented high-energy tracks, while others were calmer and more acoustic

## Author

Ishant Raj Kashyap
