
# ⭐ [LEPL1109] Hackathon 02 – Classification: Stars, Galaxies and Quasars

## 🎯 Objectif

Ce projet vise à développer un classificateur automatique permettant de distinguer les **étoiles**, **galaxies** et **quasars** à partir de leurs caractéristiques spectrales. Les données proviennent du **Sloan Digital Sky Survey (SDSS)** et comportent plus de **100 000 observations**.

---

## 🧠 Contenu

Le travail est structuré en 4 grandes parties, détaillées dans le notebook et dans le rapport PDF :

### 1. 📥 Chargement et Prétraitement des Données
- Exploration initiale du dataset (`star_classification.csv`)
- Suppression des features non pertinentes (basée sur la variance, les valeurs uniques, corrélations)
- Séparation du jeu de données (80% entraînement / 20% test)

### 2. 🔎 Analyse Exploratoire
- Étude des classes cibles et déséquilibres (stars, galaxies, quasars)
- Calcul et visualisation de la matrice de corrélation
- Normalisation des données (MinMaxScaler)

### 3. 🤖 Sélection de Modèles
- Implémentation manuelle des scores : précision, rappel, F1
- Évaluation via K-Fold Cross-Validation (k=5)
- Comparaison des performances de :
  - **Régression Logistique**
  - **Régression Linéaire**
  - **K-Nearest Neighbors (KNN)**
- Meilleur modèle sélectionné : **Régression Logistique (C=1000)**

### 4. ✅ Évaluation Finale
- Précision sur données test : **94.2%**
- Analyse des courbes Precision-Recall par classe
- Le modèle se généralise bien sur les données non vues

---

## 📁 Fichiers fournis

- `classification_hackathon02.ipynb` : Notebook Jupyter contenant tout le code
- `precision_recall_curve_STAR.pdf`, `GALAXY.pdf`, `QSO.pdf` : Visualisations
- `star_classification.csv`

---

## ⚙️ Outils & Librairies

- Python 3.10
- NumPy, Pandas, Matplotlib, Seaborn
- Scikit-learn
- Astropy (visualisation céleste)

---

## 👥 Auteurs

- Projet encadré par **Prof. D. Hainaut** et **Prof. L. Jacques**
