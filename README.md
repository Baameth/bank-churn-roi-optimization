# 🏦 Prédiction du Churn Bancaire & Optimisation du ROI

## 📌 Présentation du Projet
Ce projet vise à prédire le départ des clients (*churn*) d'un établissement bancaire à partir d'un jeu de données de 10 000 clients. 
L'objectif central est d'évaluer **l'impact financier réel (ROI)** généré par une campagne de rétention ciblée pilotée par le Machine Learning.

## 🛠️ Stack Technique
* **Langage & Environnement** : Python 3, Jupyter Notebook
* **Manipulation & SQL** : Pandas, SQLite3 (requêtes d'extraction et transformation)
* **Machine Learning** : Scikit-Learn (Logistic Regression, Random Forest Classifier)
* **Data Visualization** : Seaborn, Matplotlib

## 📊 Résultats & Impact Business
En comparant une approche Baseline (Régression Logistique) à un modèle d'ensemble (Random Forest), les résultats sur le jeu de test (2 000 clients) ont démontré une nette amélioration de la détection et des gains financiers :

| Modèle | Recall (Churn) | Precision (Churn) | Gain Net Généré (€) |
| :--- | :---: | :---: | :---: |
| **Régression Logistique** | 8% | 37% | 1 230 € |
| **Random Forest** | **42%** | **67%** | **12 330 €** |

> 💡 **Hypothèses Métier retenues :**
> * **Manque à gagner par client parti** : 300 €
> * **Coût de l'offre de rétention** : 30 € / client ciblé
> * **Taux de conversion** : 40% des vrais départs détectés sont conservés

## 📁 Structure du Projet
* `churn_client_banque.ipynb` : Notebook complet avec requêtes SQL, modélisation et fonction d'automatisation ROI.
* `Bank Customer Churn Prediction.csv` : Dataset source des clients de la banque.
