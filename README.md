# DJ Track Recommendation System using Spotify Audio Features 🎶

In this project, I develop a content-based recommendation system for music tracks using Spotify’s audio features. The goal is to apply clustering methods to identify tracks that harmonize well together.

## 📊 Projektübersicht

**Problemstellung:** 
DJs often face the challenge of selecting suitable tracks for a coherent set. Although streaming services already provide recommendations, these are often too general (e.g., based on genre or user behavior) and do not consider specific musical characteristics such as energy, key, or tempo, which are crucial for mixability.

**Ziel:** 
The aim of this project is to develop a content-based recommendation system that groups music tracks according to their audio features and recommends tracks that go well together.

**Methoden:** 
- **Exploratory data analysis (EDA) for investigating musical features
- **Clustering methods (e.g., K-Means, DBSCAN) for grouping similar tracks
- **Similarity calculations (e.g., cosine similarity)
- **Visualizations (e.g., PCA, heat maps) for representing music landscapes and relationships between tracks

## 🎧 Motivation  

Having worked for years in Procurement and Supply Chain Management, I’ve developed a strong analytical mindset and a keen eye for patterns. Now, as a Data Science graduate, I want to apply these skills to a personal passion: DJing.
For a DJ, selecting tracks that harmonize and flow seamlessly is crucial for an engaging set. This project goes beyond standard music recommendations by analyzing musical characteristics, aiming to provide deeper, data-driven insights into track selection.

## 🎯 Key Findings

<!-- Hier deine wichtigsten Erkenntnisse in 3-5 Bullet Points -->
- 📈 **Erkenntnis 1:** Kurze Beschreibung
- 🔍 **Erkenntnis 2:** Kurze Beschreibung  
- 💡 **Erkenntnis 3:** Kurze Beschreibung

## 📁 Repository Struktur

```
├── data/
│   ├── raw/                    # Originaldaten
│   └── processed/              # Bereinigte Daten
├── notebooks/                  # Jupyter Notebooks
│   └── 01_exploration.ipynb    # Datenexploration
├── src/dpp                     # Python Module
├── test/                       # Unit Tests
├── pyproject.toml              # Projektkonfiguration
└── docs/                       # Zusätzliche Dokumentation
```

## 🔧 Verwendete Technologien

**Programmiersprachen:**
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

## 📊 Daten

**Datenquelle:** 
https://www.kaggle.com/datasets/maharshipandya/-spotify-tracks-dataset

This dataset provides detailed insight into over 160,000 Spotify tracks with 21 features, including acousticity, danceability, energy, instrumentality, and tempo. Ideal for analyzing music trends, clustering songs, or building recommendation systems.

**Datensatz-Größe:** 
20.12 MB

**Wichtige Features:** 
<!-- Beschreibung der wichtigsten Variablen -->

## 🤖 Methodik

### Data Preprocessing
<!-- Kurze Beschreibung deiner Datenbereinigung -->

### Modeling Approach  
<!-- Welche Modelle hast du getestet? -->

### Evaluation
<!-- Wie hast du die Ergebnisse bewertet? -->

## 📈 Ergebnisse

**Model Performance:**
<!-- Deine besten Metriken (Accuracy, RMSE, etc.) -->

**Wichtigste Visualisierungen:**
<!-- Verweis auf Key-Plots in deinen Notebooks -->

## 🚀 Reproduzierbarkeit

### Setup
```bash
# Repository klonen
git clone https://github.com/steffenkaewert/data_science.git
cd data_science
uv init

# Dependencies installieren
uv sync
```

### Ausführung
```bash
# Notebooks in dieser Reihenfolge ausführen:
# 1. notebooks/01_exploration.ipynb
# 2. notebooks/02_preprocessing.ipynb  
# 3. notebooks/03_modeling.ipynb
# 4. notebooks/04_results.ipynb
```

## 🎓 Über dieses Projekt

**Kontext:** 
StackFuel Data Science Portfolio Project Training 

**Zeitraum:** 
25 Aug - 14 Sep 2025

**Autor:** 
Steffen Käwert

## 📞 Kontakt

**GitHub:** [@steffenkaewert](https://github.com/steffenkaewert)  
**E-Mail:** steffen.kaewert@gmail.com  
**LinkedIn:** [Steffen Käwert](https://linkedin.com/in/steffen-käwert-532ba51a4)


## 🙏 Danksagungen

Mentoren der StackFuel GmbH

---

**⭐ Wenn dir dieses Projekt gefällt, gib gerne einen Star!**
