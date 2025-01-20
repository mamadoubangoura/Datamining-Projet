
# Projet Data Mining pour l’éducation : Prédiction de la performance des apprenants

## Auteurs  
- Mamadou BANGOURA  
- Ibrahima Youssouf KEITA  
- Odilon LOUA  

**Date :** 16 Janvier 2025  

---

## Table des matières
1. Introduction  
2. Objectifs du projet  
3. Description du Dataset  
4. Architecture et Processus  
    1. Intégration des données  
    2. Sélection et Nettoyage des données  
    3. Transformation des données  
    4. Modélisation et Exploration (Data Mining)  
    5. Évaluation et Visualisations  
    6. Présentation des connaissances (Rapport)  
5. Comment exécuter le notebook  
6. Livrables  
7. Perspectives d'amélioration  
8. Dépendances et Installation  
9. Utilisation et Prédiction sur de Nouveaux Cas  
10. Conclusion  

---

## Introduction
Ce projet vise à construire un modèle prédictif des performances (notes) des apprenants dans le domaine de l’éducation. Le modèle prédit la note de l’apprenant en fonction de plusieurs paramètres, tels que :  
- **Statut économique**,  
- **Nombre moyen d’heures d’étude**,  
- **Nombre moyen d’heures de sommeil**,  
- **Pourcentage de présence en classe**.

Le projet suit un processus complet de Data Mining : intégration, préparation des données, modélisation, évaluation et présentation des résultats.

---

## Objectifs du projet
- **Prédire les notes des apprenants :** En utilisant des modèles de machine learning.
- **Visualiser et analyser les données :** Fournir des graphiques tels que des distributions, des corrélations, et la distribution des erreurs de prédiction.

---

## Description du Dataset
Le dataset utilisé est un fichier CSV contenant les colonnes suivantes :
- **Socioeconomic Score :** Statut socio-économique de l'élève.
- **Study Hours :** Nombre moyen d'heures d'étude par jour.
- **Sleep Hours :** Nombre moyen d'heures de sommeil par jour.
- **Attendance (%) :** Pourcentage de présence en classe.
- **Grades :** Notes obtenues (sur 100).

**Taille :** 1 388 lignes.

---

## Architecture et Processus
### 1. Intégration des données
- Chargement du dataset avec `pandas.read_csv`.  
- Visualisation initiale (aperçu des données, statistiques descriptives).  

### 2. Sélection et Nettoyage des données
- **Sélection :** Colonnes pertinentes sélectionnées grâce à une matrice de corrélation.  
- **Nettoyage :**  
  - Suppression des doublons.  
  - Gestion des valeurs manquantes.  

### 3. Transformation des données
- Renommage des colonnes :  
  - `Socioeconomic Score` → **statut socioeconomique**  
  - `Study Hours` → **nmheure detude par jour**  
  - `Attendance (%)` → **presence en classe (%)**  
  - `Grades` → **notes obtenues/100**  
- Standardisation des valeurs numériques.  

### 4. Modélisation et Exploration
Deux algorithmes de machine learning ont été utilisés :  
- **Linear Regression**  
- **Random Forest**  

### 5. Évaluation et Visualisations
- **Mesures de performance :** Score R², F1-score.  
- **Visualisations :**  
  - Distribution des erreurs.  
  - Heatmaps de corrélation entre variables.  

### 6. Présentation des connaissances
L'algorithme **Random Forest** a obtenu un score R² de **0.9776**, indiquant une très haute précision dans les prédictions.

---

## Comment exécuter le notebook
1. **Installer les dépendances :**  
   Assurez-vous d’avoir Python (3.7+) et les librairies listées dans la section "Dépendances".  
2. **Ouvrir le notebook :**  
   Utilisez Jupyter Notebook.  
3. **Exécuter les cellules :**  
   Suivez les étapes séquentielles pour reproduire le processus.

---

## Livrables
- Notebook complet (`.ipynb`).  
- Dataset (`data.csv`).  
- Fichier Readme (ce fichier).  

---

## Perspectives d'amélioration
- Augmenter la taille du dataset pour renforcer le modèle.  
- Tester d’autres algorithmes (ex. Gradient Boosting, SVM).  

---

## Dépendances et Installation
Librairies requises :  
- Python 3.7 ou supérieur  
- `numpy`  
- `pandas`  
- `matplotlib`  
- `seaborn`  
- `scikit-learn`  

---

## Utilisation et Prédiction sur de Nouveaux Cas
Le modèle peut être utilisé pour prédire les performances d’apprenants à partir de nouveaux ensembles de données similaires.

---

## Conclusion
Ce projet démontre l’efficacité des approches de Data Mining pour prédire les performances éducatives. Les résultats obtenus avec Random Forest ouvrent la voie à une personnalisation accrue dans l'éducation.

---
