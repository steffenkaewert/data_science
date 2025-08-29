# Content-Based Track Recommendation Machine for DJs using Audio Features 🎶

In this project, I develop a content-based recommendation system for music tracks using Spotify’s audio features. The goal is to apply clustering methods to identify tracks in the genres of electronic dance music (EDM) that harmonize well together.

## 📊 Project Overview

**Problem statement:** 
DJs often face the challenge of selecting suitable tracks for a coherent set. Although streaming services already provide recommendations, these are often too general (e.g., based on genre or collab-based) and do not consider specific musical characteristics such as energy, key, or tempo, which are crucial for mixability.

**Goal:** 
The aim of this project is to develop a content-based recommendation system that groups music tracks according to their audio features and recommends tracks that go well together.

**Methods:** 
- **Exploratory data analysis (EDA) for investigating musical features
- **Feature engineering for DJ-specific constraints (harmonic mixing, vocal/instrumental sequencing, popularity weighting)
- **Clustering methods (e.g., K-Means, DBSCAN) for grouping similar tracks
- **Similarity calculations (e.g., cosine similarity)
- **Visualizations (e.g., PCA, heat maps) for representing music landscapes and relationships between tracks

## 🎧 Motivation  

Having worked for years in Procurement and Supply Chain Management, I’ve developed a strong analytical mindset and a keen eye for patterns. Now, as a Data Science graduate, I want to apply these skills to a personal passion: DJing.
For a DJ, selecting tracks that harmonize and flow seamlessly is crucial for an engaging set. This project goes beyond standard music recommendations by analyzing musical characteristics, aiming to provide deeper, data-driven insights into track selection.

## 🎯 Key Findings

<!-- Hier deine wichtigsten Erkenntnisse in 3-5 Bullet Points -->
- 📈 **Findings 1:** Kurze Beschreibung
- 🔍 **Findings 2:** Kurze Beschreibung  
- 💡 **Findings 3:** Kurze Beschreibung

## 📁 Repository Structure

```
├── data/
│   ├── raw/                    # Original data
│   └── processed/              # Cleaned data
├── notebooks/                  # Jupyter Notebooks
│   └── 01_exploration.ipynb    # Data exploration
├── src/dpp                     # Python modules
├── test/                       # Unit tests
├── pyproject.toml              # Project configuration
└── docs/                       # Additional documentation
```

## 🔧 Technologies used

**Programming Languages:**
Python

**Libraries & Frameworks:**
- **pandas** – data manipulation & preprocessing  
- **numpy** – numerical operations  
- **scikit-learn** – clustering (K-Means, DBSCAN), similarity measures, PCA  
- **matplotlib** & **seaborn** – data visualization  
- **scipy** – additional similarity/distance calculations  
- **plotly** – interactive visualizations (optional)

**Tools:**
- **Jupyter Notebook** – development & experimentation  
- **Git & GitHub** – version control & portfolio presentation
- **uv** – package management & reproducible environments 
- **Docker** *(optional)* – reproducible project environment  
- **VS Code** – IDE for project structuring  

## 📊 Data

**Data sources:** 
https://www.kaggle.com/datasets/maharshipandya/-spotify-tracks-dataset

This dataset provides detailed insight into over 114,000 Spotify tracks with 21 features, including acousticity, danceability, energy, instrumentality, and tempo. Ideal for analyzing music trends, clustering songs, or building recommendation systems.

**Dataset size:** 
20.12 MB

**Key features:** 
duration_ms, explicit, danceability, energy, key, loudness, mode, speechiness, instrumentalness, acousticness, liveness, valence, tempo, time_signature, track_genre

## 🤖 Methodology

### Data Preprocessing
- Delete Unnamed: 0, set index
- Transform explicit to int
- One-hot encode (OHE) of artists depending on count
- Scale loudness and tempo to [0, 1]
- Transform key + mode to Camelot-ID for harmonic mixing
- Filter time_signature = 4 for EDM tracks
- Filter track_genre on EDM-relevant genres, apply OHE
- Feature engineering: club Factor = danceability × energy, groove = tempo × time_signature

### Constraints
- Off-topic tracks allowed at beginning/end of sets
- Last third of set can feature more popular tracks (popularity)
- After a track with vocals (high speechiness, low instrumentalnes), at least two tracks without vocals (vice versa) should follow in order to avoid confusing the audience.
- Set structure: Opening, Highlight, Popularity, Closing Tracks considered; system suggests tracks based on remaining duration and segment rules

### Modeling Approach
Clustering (K-Means, DBSCAN) for track grouping
Cosine similarity and distance measures for track recommendations
PCA and heatmaps for visual representation of music landscape
Recommendation logic incorporates DJ constraints (vocal sequencing, harmonic mixing, popularity weighting, segment-based track types)

### Evaluation
Evaluate cluster cohesion and separation
Test recommendation logic against DJ rules (vocal/instrumental sequencing, harmonic mixing, popularity weighting, segment-based track allocation)

## 📈 Results

**Model Performance:**
<!-- Deine besten Metriken (Accuracy, RMSE, etc.) -->

**Key Visualizations:**
<!-- Verweis auf Key-Plots in deinen Notebooks -->

## 🚀 Reproducibility

### Setup
```bash
# Clone repository
git clone https://github.com/steffenkaewert/data_science.git
cd data_science
uv init

# Install dependencies
uv sync
```

### Execution
```bash
# Run notebooks in this order:
# 1. notebooks/01_exploration.ipynb
# 2. notebooks/02_preprocessing.ipynb  
# 3. notebooks/03_modeling.ipynb
# 4. notebooks/04_results.ipynb
```

## 🎓 About this Project

**Context:** 
StackFuel Data Science Portfolio Project Training 

**Timeframe:** 
25 Aug - 14 Sep 2025

**Author:** 
Steffen Käwert

## 📞 Contact

**GitHub:** [@steffenkaewert](https://github.com/steffenkaewert)  
**E-Mail:** steffen.kaewert@gmail.com  
**LinkedIn:** [Steffen Käwert](https://linkedin.com/in/steffen-käwert-532ba51a4)


## 🙏 Acknowledgements

Mentoren der StackFuel GmbH

---

**⭐ If you like this project, feel free to give it a star!**