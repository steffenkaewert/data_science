# DJ Track Recommendation System using Spotify Audio Features 🎶

In this project I develop a recommendation system for music tracks based on Spotify track data. The goal is to use clustering methods to identify music tracks that go well together.

## 📊 Projektübersicht

**Problemstellung:** 
DJs often face the challenge of selecting suitable tracks for a coherent set. Although streaming services already offer recommendations, these are often too general (e.g. based on genre oir likes) and do not take into account specific musical characteristics that are crucial for mixability. Genre- or like-based recommendations are often insufficient because they doesn't consider different energy levels, moods, keys, or BPM shich are crucial for an attracive set.

**Ziel:** 
The goal of the project is to develop a recommendation system that groups music tracks based on their musical characteristics and recommends tracks that go well together.

**Methoden:** 
- **Exploratory data analysis (EDA) for investigating musical features
- **Clustering methods (e.g. K-Means, DBSCAN) for grouping similar tracks
- **Similarity calculations (e.g. cosine similarity)
- **Visualizations (e.g. PCA, heat maps) for representing music landscapes and relationships between tracks

## 🎧 Motivation  

As a DJ, choosing tracks that harmonize well is key to create an engaging set.  
This project aims to go beyond standard recommendations and instead leverage musical characteristics to provide more meaningful suggestions. 

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
git clone [DEIN-REPO-LINK]
cd [REPO-NAME]

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
StackFuel Data Science Training Portfolio Project 

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
